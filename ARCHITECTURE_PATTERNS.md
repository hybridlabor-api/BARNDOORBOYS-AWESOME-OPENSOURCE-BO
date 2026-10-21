# ⚡ AOS 5.5 System Architecture & Engine Blueprint

> **Kompaktes Handover-Dossier für autonome Agenten (Claude Code, Antigravity, OpenCode).**  
> *Synthese aus Screen-Captures, Whitepapers und System-Designs aus `Neuer Ordner mit Objekten 4` und den vorangegangenen Audit-Runden.*

---

## 1. Andrew Ng: Graph Engineering vs. Loop Engineering
*Quelle: Andrew Ng (DeepLearning.AI), July 2026 Compilation*

### Kernargument & Paradigmenwechsel
Ein einfaches Basis-Modell löst **48.1%** auf HumanEval (Zero-Shot). Im iterativen ReAct-Workflow steigt der Wert auf **95.1%**. Der Qualitätsgewinn durch Architektur übersteigt den Generationssprung des Modells.

* **ReAct-Loops:** externalisieren lediglich die *Revisionsschleife*.
* **Chains:** externalisieren die *Reihenfolge der Schritte*.
* **Networks/Swarms:** externalisieren *Rollen-Spezialisierungen*.
* **State Graphen (AOS 5.5 Ziel):** externalisieren **geteilten Zustand (Shared State) und Beziehungen**. Arbeiter müssen Fakten über Sessions hinweg erhalten, ohne gigantische Transkripte zu kopieren.

```
[User] ──(In-Loop Feedback)──> [Architect Agent] ──(Shares Data)──> [AI Document / State Graph]
   ▲                                 │                                          ▲
   │                           (Handoff: Spec)                                  │
   │                                 ▼                                          │
   └──────(In-Loop Feedback)──> [TechLead Agent] ──(Handoff: Slices)────────────┤
   │                                 │                                          │
   │                           (Handoff: Task)                                  │
   │                                 ▼                                          │
   └──────(In-Loop Feedback)──> [Developer Agent] ──────────────────────────────┘
                                  (Analyzes & Responds to Shared State)
```

---

## 2. The Self-Evolving Agent Harness
*Quelle: Rakesh Gohel (@techwith.ram / @rakeshgohel01)*

Ein Agent, der seine eigenen Fehler behebt, ohne funktionierenden Code oder Prompts zu zerstören.

### Das 4-Schichten-System
1. **Perception Layer & Planning:**
   * **Perceive:** Trennt rohen Input von strukturierten Intentionen.
   * **Planning Module:** Bricht komplexe Ziele atomar herunter: `Step 1 -> Step 2 -> Step 3`.
   * **Fast-Path:** Kann die Frage direkt beantwortet werden, erfolgt sofortiger Output ohne Subagent-Overhead.
2. **Protected Competence (2-Stufen-Gate):**
   * **Gate 1 (Quality Gate):** Prüft syntaktische und logische Korrektheit gegen Benchmarks.
   * **Gate 2 (Performance Gate):** Misst Latenz, Token-Verbrauch und Token-Weather.
   * **Reject:** Bei Regression sofortiges Rollback.
   * **Accept:** Update wird im Core persistiert.
3. **Self-Update Unit (Der Self-Improvement Loop):**
   * **Self-Rewrite:** Schreibt Prompts, Tools und Heuristiken selbstständig um.
   * **Update Checkpoints:** Transaktionale Snapshots vor jeder Mutation.
   * **Real Generalization:** Erkennt Muster statt Benchmark-Hacks. Clustert Fehler nach:  
     `Tool Usage Errors` | `Reasoning Mistakes` | `Planning / Premature Stop` | `One-off Case`.
4. **Observability & Error Signals:**
   * **τ_fail vs τ_ref:** Referenz-Alignment identifiziert den exakten Schritt der ersten Divergenz (nicht erst den finalen Crash).

---

## 3. Frontier Architecture Suite: Advisor, Swarms & Context Shielding
*Quelle: @damkina7 & @rvaniaaa*

### Die goldene Regel: *"Plan on High. Delegate on Medium. Keep Opus on Call."*

### Das 3-Ebenen-Routing
1. **Haiku 5.5 (Scouts & Swarm):**
   * Scoutet Repos, liest Dokumentation read-only. Kostet bis zu 40x weniger als Opus.
   * Erledigt schnelle Bash-, Git- und AST-Searches (340 t/s).
2. **Sonnet 5.5 (The Driver / Main Session):**
   * Führt den Hauptcode aus, editiert Dateien, baut Komponenten.
   * Niedrige Latenz, hohe Coding-Präzision.
3. **Opus 5.5 (Advisor & System Architect):**
   * Läuft *on call* als Advisor: `claude --model sonnet --advisor opus`.
   * Wird nur an **3 definierten Checkpoints** gerufen:
     1. Vor dem Locken eines Plans / Schemas.
     2. Wenn derselbe Fehler zweimal auftritt.
     3. Vor dem finalen Ship / Pre-flight Diff Review.

### Context Shielding (-412k Tokens gespart)
* **Subagent Swarm:** Hohe AST-Searches, Spec-Recherche und Git-Worktrees laufen in isolierten Workern ab.
* **Context Shield:** 412k Tokens an flüchtigem Rauschen werden in Subagents absorbiert.
* **Main Context:** Bleibt kristallklar bei **14k Tokens**! Kein Context-Compacting, kein Halluzinieren.
* **Jev-Fork Layer:** Deterministische Entscheidungen (welche Datei, Retry, Tools) laufen in < 0.5s auf System-1-Ebene, statt teure LLM-Inferenz zu triggern.

---

## 4. 15 AI Agent Design Patterns (Ultra Lab & Anthropic)
*Quelle: Ultra Lab (ultralab.tw) & Anthropic (2024–2026)*

| # | Pattern | Ursprung | Architektonische Regel & Verhalten |
|---|---|---|---|
| **01** | **Routing** | Anthropic | Unterschiedliche Input-Typen werden strikt getrennt und an spezialisierte Agenten verteilt. |
| **02** | **Orchestrator-Workers** | Anthropic | Zentraler Orchestrator koordiniert dynamische Worker; Subtasks können vorab unvorhersehbar sein. |
| **03** | **Augmented LLM** | Anthropic | Basisbaustein: Inferenz angereichert mit Retrieval (RAG), Tools und Memory. |
| **04** | **Prompt Chaining** | Anthropic | Aufgabe wird sauber in deterministische, aufeinanderfolgende Schritte zerlegt. |
| **05** | **Sectioning** | Anthropic | Parallele Ausführung unabhängiger Subtasks zur massiven Latenzreduktion. |
| **06** | **Autonomous Agent** | Anthropic | Offene Probleme ohne festen Pfad; ReAct-Loop mit Umgebungs-Feedback. |
| **07** | **Mutex Lock** | Ultra Lab | Eine Ressource (z.B. GPU, Shared Database, Git Branch), viele Jobs: Strikte Queue, niemals paralleles Überschreiben. |
| **08** | **Evaluator-Optimizer** | Anthropic | Klare Kriterien; ein zweiter Agent bewertet und optimiert den Output messbar. |
| **09** | **Voting** | Anthropic | Mehrere parallele Durchläufe derselben Aufgabe zur Steigerung der Konfidenz. |
| **10** | **Quality Gate** | Ultra Lab | Jeder einzelne FAIL blockiert das Scheduling des nächsten Release-Schritts. |
| **11** | **Human-in-the-loop** | Ultra Lab | Blockiert oder 2x fehlgeschlagen: Sofortiges Anhalten und Übergabe an den Menschen. |
| **12** | **Fail-Closed** | Ultra Lab | Fehlen von Beweisen oder unvollständige Tests zählen ausnahmslos als FAIL. |
| **13** | **Retry with Backoff** | Ultra Lab | Netzwerk- oder 5xx-Fehler: Exponentielles Warten vor dem Wiederholungsversuch. |
| **14** | **Idempotency Key** | Ultra Lab | Wiederholte Ausführungen führen niemals zu doppelten Aktionen oder Posts. |
| **15** | **Observability** | Ultra Lab | Jeder einzelne Tool-Call wird lückenlos mit Tokens, Kosten und Turns protokolliert. |

---

## 5. Autonomous 4-Eyes Factory Pattern
*Quelle: zazencodes / claude-code-software-factory*

### Deterministischer Build- & Review-Zyklus
```
                  [Feature Request]
                          │
                          ▼
                 [Spec-Writer (Opus)]
                          │
                          ▼
                   [Builder (Opus)] <────────────────────────────┐
                          │                                      │
         ┌────────────────┼────────────────┬────────────────┐    │ (resume builder
         ▼                ▼                ▼                ▼    │  max 2 rounds)
    [Security]          [UX]          [UI Design]        [Code]  │
      (Opus)          (Sonnet)         (Sonnet)         (Sonnet) │
         │                │                │                │    │
         └────────────────┼────────────────┴────────────────┘    │
                          ▼                                      │
                [Wait for ALL 4 in] ──(Any Changes Needed)───────┘
                          │
                     (All PASS)
                          ▼
                   [Approver (Opus)]
                          │
            ┌─────────────┴─────────────┐
            ▼                           ▼
        (APPROVE)                   (ESCALATE)
            ▼                           ▼
     [Merge to Main]              [Needs-Human]
```

---

## 6. REA Studio: 20 Repos für Binary-to-Clean-Room Rebuilds
*Quelle: @morluto (Opus 5.5 + REA Studio)*

### Das Clean-Room Rebuild Pattern
1. **Decompile & Inspect:** Extraktion via Ghidra / REA / jadx / ILSpy.
2. **Traffic Sniffing:** Interception über `mitmproxy` & `frida`.
3. **Formalize Spec:** Erstellung einer `SPEC.md` mit allen Endpunkten, Structs und Zuständen.
4. **Clean-Room Implementation:** Rebuild ohne fremden Code zu kopieren.
5. **Oracle Verification:** Parallele Testläufe gegen das Original bis zu 100% Identität.

### Vollständige Werkzeug-Matrix für Agenten
| Domäne | Tool / Repo | Agenten-Nutzen & Funktion |
|---|---|---|
| **Analysis Core** | `morluto/rea` | Universal Reverse-Engineering MCP Server für Coding-Agenten. |
| **Analysis Core** | `NationalSecurityAgency/ghidra` | Open-Source Decompiler und Disassembler Suite der NSA. |
| **Analysis Core** | `LaurieWired/GhidraMCP` | Ermöglicht Agenten das autonome Steuern von Ghidra via MCP. |
| **Analysis Core** | `mrexodia/ida-pro-mcp` | Agent-Schnittstelle zu Hex-Rays IDA Pro. |
| **Mobile & Apps** | `skylot/jadx` | DEX/APK to Java Decompiler für Android-Binaries. |
| **Mobile & Apps** | `iBotPeaches/Apktool` | Zerlegt Android-APKs und baut sie nach Modifikation wieder zusammen. |
| **Mobile & Apps** | `frida/frida` | Dynamische Code-Injektion und Funktions-Hooking zur Laufzeit. |
| **Mobile & Apps** | `icsharpcode/ILSpy` | Open-Source .NET Decompiler & Assembly Analyzer. |
| **Binary & Low-Level** | `radareorg/radare2` | Terminal-natives UNIX Reverse-Engineering-Framework. |
| **Binary & Low-Level** | `x64dbg/x64dbg` | Nativer x64/x32 Windows Debugger. |
| **Binary & Low-Level** | `WerWolv/ImHex` | Hex-Editor mit eigener deklarativer Pattern-Sprache. |
| **Binary & Low-Level** | `angr/angr` | Symbolische Ausführungs-Engine zur automatischen Schwachstellensuche. |
| **Network & Runtime** | `mitmproxy/mitmproxy` | Interaktiver TLS-Proxy zur HTTP/HTTPS- und WebSocket-Analyse. |
| **Network & Runtime** | `dnSpyEx/dnSpy` | .NET Debugger und Assembly-Editor. |
| **Network & Runtime** | `rizinorg/rizin` | Performanter, modularer Radare2-Fork. |
| **Network & Runtime** | `EpicGames/raddebugger` | Extrem schneller nativer Multi-Process Debugger von Epic Games. |
| **Collections & Guides** | `zhuyansen/awesome-ai-reverse-engineering` | Kuratierte Liste von 122 AI-gestützten RE-Werkzeugen. |
| **Collections & Guides** | `morluto/awesome-reverse-engineering` | Offizielle kuratierte RE-Sammlung des REA-Autors. |

---

## 7. High-Throughput Ticket Waiting Room (System Design)
*Quelle: goatengineer.com (System Design 02)*

### Das Problem: 20.000 Requests/Sekunde & Distributed Lock Contention
Ein naives `UPDATE tickets SET left = left - 1 WHERE event = 42` erzeugt bei 20k req/s einen Datenbank-Kollaps: Ein einziger Row-Lock blockiert tausende Worker, 15.000 Transaktionen laufen ins Timeout.

### Die skalierbare Architektur
1. **Virtual Waiting Room / Token Bucket:** Nutzer erhalten eine signierte Queue-Nummer (JWT) im Redis Sorted Set.
2. **Traffic Slicing:** Nur die exakte Anzahl an Requests, die die Datenbank verarbeiten kann (z.B. 500 req/s), wird sequentiell an den Checkout-Service weitergeleitet.
3. **Optimistic Decoupling:** Bestände werden vorab in Redis dekrementiert (`DECR` atomar); die persistente DB-Schreibung erfolgt asynchron über Kafka/RabbitMQ-Worker.
