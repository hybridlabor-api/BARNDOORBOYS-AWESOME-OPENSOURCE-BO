# ⚡ AOS 5.5 Master Architecture & Model Routing Catalog

> **Synthese aller 14 Systemarchitekturen, Topologien und Modell-Routings aus über 80 Bildnachweisen**  
> *Für autonome Agenten (Claude Code, Antigravity, OpenCode, Codex CLI, GLM, DeepSeek).*

---

## 📑 Inhaltsübersicht der 14 Schemas
1. [Frontier Tri-Model Setup (Sonnet / Haiku / Opus)](#1-frontier-tri-model-setup-sonnet-drives-haiku-scouts-opus-signs-off)
2. [Inverted Tree: Fable 5.1 Advisor / Opus 5.5 Works](#2-inverted-tree-fable-51-on-call--opus-55-works)
3. [Context Shielding Architecture (-412k Tokens)](#3-context-shielding-architecture--412k-tokens-gespart)
4. [OpenRig: Cross-Harness YAML Rig (Claude Code + Codex)](#4-openrig-cross-harness-yaml-rig-claude-code--codex)
5. [Multi-Harness Cross-Agent BugHunter Pipeline](#5-multi-harness-cross-agent-bughunter-pipeline)
6. [Blackbit Multi-Model Tiering Architecture](#6-blackbit-multi-model-tiering-architecture)
7. [Token & Cost Optimization Pipeline (8-Stufig)](#7-token--cost-optimization-pipeline-8-stufig)
8. [The Self-Evolving Agent Harness (4 Layers)](#8-the-self-evolving-agent-harness)
9. [Andrew Ng: Graph Engineering vs. Loop Engineering](#9-andrew-ng-graph-engineering-vs-loop-engineering)
10. [Ultra Lab & Anthropic: 15 AI Agent Design Patterns](#10-ultra-lab--anthropic-15-ai-agent-design-patterns)
11. [Autonomous 4-Eyes Software Factory Pattern](#11-autonomous-4-eyes-software-factory-pattern)
12. [High-Throughput Ticket Waiting Room (20k req/s)](#12-high-throughput-ticket-waiting-room-20k-reqs-system-design)
13. [Paperthin: Cross-Harness Reflex Injection](#13-paperthin-cross-harness-reflex-injection)
14. [REA Studio: 20 Repos Clean-Room Loop](#14-rea-studio-20-repos-clean-room-loop)

---

## 1. Frontier Tri-Model Setup: Sonnet Drives, Haiku Scouts, Opus Signs Off
*Quellen: `IMG_7229.PNG`, `IMG_7230.PNG`, `IMG_7365.PNG`, `IMG_7494.jpg` (@mirku21 & @rvaniaaa)*

### Grundsatz
> *"Stop burning Opus 5.5 context on tasks Haiku 5.5 can swarm, while Sonnet 5.5 builds."*

```bash
$ claude --model sonnet --advisor opus --subagents haiku
```

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│ [HAIKU 5.5 EXPLORE / SWARM]                                                            │
│ * Scouts repo & docs read-only (15 files read, 0 docs pulled).                         │
│ * High speed: 340 tok/s. Kosten: bis zu 40x weniger als Opus.                          │
└────────────────────────────────────────┬───────────────────────────────────────────────┘
                                         ▼ (Fast Findings)
┌────────────────────────────────────────────────────────────────────────────────────────┐
│ [SONNET 5.5 THE DRIVER - MAIN SESSION]                                                 │
│ * Drives the session on high effort.                                                   │
│ * Edits source code, runs build & test suites, builds components.                      │
└────────────────────────────────────────┬───────────────────────────────────────────────┘
                                         ▼ (Checkpoints)
┌────────────────────────────────────────────────────────────────────────────────────────┐
│ [OPUS 5.5 ADVISOR - ON CALL] (Re-reads session, signs off, advises)                    │
│ Gerufen an EXAKT DREI PUNKTE:                                                          │
│   1. Before locking a plan or schema.                                                  │
│   2. When the same test / build error occurs TWICE.                                    │
│   3. Before saying 'done' (pre-flight diff review).                                    │
│ Ruht sonst komplett (0 Waits, kein Context-Pollution).                                 │
└────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 2. Inverted Tree: Fable 5.1 On Call / Opus 5.5 Works
*Quelle: `IMG_7011.PNG` (Claude Code Agent Tree)*

```
CLAUDE CODE AGENT TREE - OPUS 5.5 WORKS - FABLE 5.1 ON CALL
CLI Befehl: /advisor fable

┌───────────────────────────────────────┐         ┌───────────────────────────────────────┐
│ FABLE 5.1 - ADVISOR                   │         │ OPUS 5.5 - MAIN SESSION               │
│ * On call - reads it all.             │ <-----> │ * Runs primary execution on high.     │
│ * Writes zero lines of code.          │         │ * Writes core logic, runs compilers.  │
│ * Steelsmans specs & enforces checks. │         │                                       │
└───────────────────────────────────────┘         └───────────────────┬───────────────────┘
                                                                      │
                    ┌─────────────────────────────────────────────────┴────────┐
                    ▼                                                          ▼
   ┌─────────────────────────────────┐                       ┌─────────────────────────────────┐
   │ JEV FORK LAYER                  │                       │ SUBAGENTS (MEDIUM)              │
   │ Deterministische Tiny Choices   │                       │ Parallelisierte Worker          │
   │ (which file / which tool <0.5s) │                       │ (UI, Tests, Specs)              │
   └─────────────────────────────────┘                       └─────────────────────────────────┘
```

---

## 3. Context Shielding Architecture (-412k Tokens Gespart)
*Quellen: `IMG_7361.PNG`, `IMG_7362.jpg` (@damkina7)*

```
                               ┌──────────────────────────────────────────────┐
                               │ OPUS 5.5 HIGH - MAIN SESSION ARCHITECT       │
                               │ Context: 14k clean tokens | Designs Topology │
                               └──────────────────────┬───────────────────────┘
                                                      │
         ═════════════════════════════════════════════╪═══════════════════════════════════════════
         CONTEXT SHIELD (Absorbiert 412k Tokens Rauschen: AST, Specs, Build-Logs, Git-Trees)
         ═════════════════════════════════════════════╪═══════════════════════════════════════════
                                                      │
                        ┌─────────────────────────────┼─────────────────────────────┐
                        ▼                             ▼                             ▼
         ┌────────────────────────────┐┌────────────────────────────┐┌────────────────────────────┐
         │ ComponentBuilder           ││ MotionAndTest              ││ BuildWorker                │
         │ Sonnet 5.5 (Medium)        ││ Haiku 5.5 (Medium)         ││ Haiku 5.5 (Medium)         │
         │ Assembles schemas, routes  ││ Compiling 60 FPS spring    ││ Headless bundle typecheck  │
         │ & React UI.                ││ physics, AST checks.       ││ Zero log pollution to main.│
         └────────────────────────────┘└────────────────────────────┘└────────────────────────────┘
```

---

## 4. OpenRig: Cross-Harness YAML Rig (Claude Code + Codex)
*Quelle: `IMG_7008.PNG` (mvschwarz/rig)*

```yaml
# RigSpec.yaml - Multi-Agent Fleet
name: bdb-production-rig
agents:
  architect:
    harness: claude-code
    model: claude-3-7-sonnet
    role: system-planning
  backend_core:
    harness: codex-cli
    model: o3-mini
    role: rust-tauri-engine
  auditor:
    harness: antigravity
    model: gemini-2.5-pro
    role: verification-gate
```

* `$ rig up`: Bootet alle tmux-Sessions mit einem Befehl.
* `$ rig status`: Topologie-Graph TUI.
* `$ rig broadcast "GO"`: Synchroner Befehl an alle Agenten.

---

## 5. Multi-Harness Cross-Agent BugHunter Pipeline
*Quelle: `IMG_6909.PNG` (Claude-BugHunter)*

```
                ┌────────────────────────────────────────────────────────┐
                │ 6-PHASEN MULTI-HARNESS SECURITY PIPELINE               │
                │ Unterstützt: Claude Code, OpenCode, Codex CLI, Hermes  │
                └───────────────────────────┬────────────────────────────┘
                                            ▼
┌──────────────────────────────┐┌──────────────────────────────┐┌──────────────────────────────┐
│ 1. Recon & Attack Surface    ││ 2. Tool Ports & Burp MCP     ││ 3. 7-Fragen Validierungs-Gate│
│ Codex TOML / Claude YAML     ││ OpenCode JSON / Burp Suite   ││ Tötet False-Positives        │
│ Frontmatter-Validierung      ││ Interceptor Schnittstellen   ││ VOR dem Report-Schreiben     │
└──────────────────────────────┘└──────────────────────────────┘└──────────────────────────────┘
```

---

## 6. Blackbit Multi-Model Tiering Architecture
*Quellen: `IMG_7306.PNG`, `IMG_6911.jpg` (blackbit.sh / CyrilXBT)*

```
                 [Incoming User Request]
                            │
                            ▼
           [Opus 5.5: Task Decomposition & Master Plan]
                            │
         ┌──────────────────┼──────────────────┐
         ▼                  ▼                  ▼
  [DeepSeek / GLM]    [Gemini Flash]    [Sonnet / Codex]
  Code Scaffolding    Fast Scraping     Complex Systems
  & Bulk Functions    & Text Parsing    & Refactoring
```

---

## 7. Token & Cost Optimization Pipeline (8-Stufig)
*Quelle: `IMG_7363.PNG` (@rvaniaaa)*

| Stufe | Tool / Engine | Mechanismus & Ersparnis |
|---|---|---|
| **1. Routing** | `claude-code-router` | Routet Grep und triviale Abfragen auf billigste Modelle; nur Hard Parts an Opus. |
| **2. Bash Pruning** | `rtk` | Kürzt rohe Terminal-Outputs (Test, Build, Git) um bis zu **90%**, bevor das LLM sie sieht. |
| **3. Symbol Lookup** | `token-savior` | Zielt exakt auf Symboldefinitionen statt ganze 2000-Zeilen-Dateien zu laden. |
| **4. Selective Memory** | `claude-mem` | Bringt nur exakt den für den aktuellen Task relevanten Teil aus alten Sessions zurück. |
| **5. Line Slicing** | `context-mode` | Lokale SQLite-DB; streamt nur die tatsächlich benötigten Codezeilen ins Fenster. |
| **6. Graph Navigation** | `code-review-graph` | Repräsentiert die Codebase als AST-Graph; verhindert vollständiges Rescannen. |
| **7. Micro Choices** | `jev-ultrafast` | Trifft Klick-, Retry- und Tool-Wahlen deterministisch in <0.5s ohne API-Aufruf. |
| **8. Telegraphic Style** | `caveman` | Zwingt das Modell zu knappen Antworten; Code bleibt identisch, spart Output-Tokens. |

---

## 8. The Self-Evolving Agent Harness
*Quellen: `IMG_7486.PNG`, `View recent photos.png` (Rakesh Gohel @techwith.ram)*

```
                                      [Input Task]
                                           │
                                           ▼
                                 [Perception Layer]
                                           │
                                           ▼
                               [Reasoning Engine / LLM]
                             (Chain-of-Thought / ReAct)
                                           │
                                ┌──────────┴──────────┐
                     (Direct Answer?)             (Complex Goal?)
                                │                         │
                                ▼                         ▼
                            [Output]              [Planning Module]
                                                  (Step 1 -> 2 -> 3)
                                                          │
                                                          ▼
                                              [Protected Competence]
                                           Every update must earn its way in!
                                           ┌──────────────────────────────┐
                                           │ Gate 1: Quality Gate         │
                                           │ Gate 2: Performance Gate    │
                                           └──────────────┬───────────────┘
                                                          │
                                         ┌────────────────┴────────────────┐
                                     (REJECT)                          (ACCEPT)
                                         ▼                                 ▼
                                   [Rollback]                     [Self-Update Unit]
                                                                  (Self-Rewrite Prompts,
                                                                   Update Checkpoints,
                                                                   τ_fail Alignment)
```

---

## 9. Andrew Ng: Graph Engineering vs. Loop Engineering
*Quellen: `IMG_7502.PNG`, `IMG_7503.jpg` (Andrew Ng, DeepLearning.AI)*

```
[User] ──(In-Loop Feedback)──► [Architect Agent] ──(Shares Data)──► [AI Document / State Graph]
   ▲                                 │                                          ▲
   │                           (Handoff: Spec)                                  │
   │                                 ▼                                          │
   └──────(In-Loop Feedback)──► [TechLead Agent] ──(Handoff: Slices)────────────┤
   │                                 │                                          │
   │                           (Handoff: Task)                                  │
   │                                 ▼                                          │
   └──────(In-Loop Feedback)──► [Developer Agent] ──────────────────────────────┘
                                  (Analyzes & Responds to Shared State)
```

---

## 10. Ultra Lab & Anthropic: 15 AI Agent Design Patterns
*Quelle: `IMG_7490.PNG` (ultralab.tw & Anthropic)*

| Kategorie | Muster | Funktion |
|---|---|---|
| **Routing & Exec** | Routing, Orchestrator-Workers, Augmented LLM | Klare Rollenverteilung, RAG, Subtask-Dynamik. |
| **Parallelisierung** | Prompt Chaining, Sectioning, Voting | Deterministische Schritte, parallele Slices, Konfidenzabgleich. |
| **Zuverlässigkeit** | Mutex Lock, Quality Gate, Fail-Closed | Ressourcensperre, Abbruch bei 1 Fehler, Beweislastprinzip. |
| **Resilienz** | Retry with Backoff, Idempotency Key, Human-in-the-Loop | 5xx-Handhabung, doppelte Posts verhindern, Escalation bei 2 Fails. |
| **Transparenz** | Observability, Evaluator-Optimizer | Lückenloses Logging jedes Tokens, iterative Schärfung. |

---

## 11. Autonomous 4-Eyes Software Factory Pattern
*Quellen: `IMG_7417.jpg`, `IMG_7479.PNG` (zazencodes)*

```
Feature ──► Spec-Writer (Opus) ──► Builder (Opus)
                                        │
           ┌──────────────┬─────────────┴─────────────┬──────────────┐
           ▼              ▼                           ▼              ▼
     Security (Opus)   UX (Sonnet)            UI Design (Sonnet)  Code (Sonnet)
           │              │                           │              │
           └──────────────┴─────────────┬─────────────┴──────────────┘
                                        ▼
                            [Wait for ALL 4 in]
                                        │
                       (Changes?) ──────┴──────► Resume Builder (max 2 rounds)
                                │
                            (All PASS)
                                ▼
                         Approver (Opus) ──► [Merge to Main] / [Escalate]
```

---

## 12. High-Throughput Ticket Waiting Room (20k req/s System Design)
*Quelle: `IMG_7511.PNG` (goatengineer.com)*

```
[20,000 Fans/s] ──► [Load Balancer] ──► [Virtual Waiting Room (Redis Token Bucket / JWT)]
                                                     │
                             (Gedrosselter Traffic: exakt 500 req/s)
                                                     ▼
                                          [12x App Servers]
                                                     │
                             (Atomarer DECR in Redis Cache)
                                                     ▼
                                 [Async Worker Queue (Kafka / BullMQ)]
                                                     │
                                                     ▼
                                         [Single Tickets Database]
                                     Kein Row-Lock Timeout! 0 Fails.
```

---

## 13. Paperthin: Cross-Harness Reflex Injection
*Quelle: `IMG_7432.PNG` (LilMGenius/paperthin)*

```bash
$ npx skills add LilMGenius/paperthin --global --agent '*'
```
* Läuft identisch auf: **Claude Code, Codex CLI, OpenCode, Antigravity, Copilot, Cursor, Grok-Build, Pi, Hermes**.

---

## 14. REA Studio: 20 Repos Clean-Room Loop
*Quellen: `IMG_7497.PNG`, `IMG_7498.PNG`, `IMG_7499.PNG` (@morluto)*

```
Binary / APK / Target
        │
        ▼
[Decompile & Intercept] ──► Ghidra / REA / GhidraMCP / ida-pro-mcp / jadx / mitmproxy / frida
        │
        ▼
[Formalize Spec]        ──► SPEC.md (Typen, Interfaces, Crypto, State Machine)
        │
        ▼
[Clean-Room Rebuild]    ──► Neuer Quellcode ohne fremde Zeilen
        │
        ▼
[Oracle Verification]   ──► Parallel-Execution gegen Target bis 100% Match
```
