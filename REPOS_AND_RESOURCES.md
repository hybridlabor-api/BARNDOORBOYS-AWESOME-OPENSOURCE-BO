# Kuratierte Übersicht: Repos, Agent-Tools, Prompts & Cloud-Dienste

Diese Übersicht basiert auf der vollständigen Analyse aller Screenshots im Hauptordner `/Users/timrennings/Downloads/Interessante repos` sowie dem Unterordner `github maybe doppelt`. 

Die Strukturierung ist strikt nach Relevanz aufgebaut: **`AOS` (Agent OS, Multi-Agent Swarm, Coding-Harness, Skills & Design)** steht oben, und **`saasengine` (Cloud-Dienste, Flotten-Infrastruktur & Self-Hosted Services)** befindet sich am Ende der Datei.

---

## Inhaltsverzeichnis
1. [Kategorie 1: Direkt hochrelevant für `/bdb-dev AOS` (Agent OS, Harness, Skills, Supervision, QA)](#kategorie-1-direkt-hochrelevant-für-bdb-dev-aos)
2. [Kategorie 2: Frontend, Design-Skills & UI-Komponenten (Godmode UI/UX & WebGPU)](#kategorie-2-frontend-design-skills--ui-komponenten)
3. [Kategorie 3: Video & Creative Media Tech (Godmode Media / EventTech)](#kategorie-3-video--creative-media-tech)
4. [Kategorie 4: Gründer- & Strategie-Skills für Claude Code](#kategorie-4-gründer--strategie-skills-für-claude-code)
5. [Kategorie 5: Architektur-Blueprints, Agent-Muster & Intentional Prompts](#kategorie-5-architektur-blueprints-agent-muster--intentional-prompts)
6. [Kategorie 6: Interne Workspace-Snapshots & Event-Notizen](#kategorie-6-interne-workspace-snapshots--event-notizen)
7. [Kategorie 7: Relevant für `saasengine` (Cloud-Dienste, Flotte, Hosting)](#kategorie-7-relevant-für-saasengine)
8. [Kategorie 8: Neue Sammlung — 7. Okt 2026 (`github repos neue sammlung 7 okt/`)](#kategorie-8-neue-sammlung--7-okt-2026-github-repos-neue-sammlung-7-okt)
9. [Kategorie 9: Chrome-Tab-Sammlung — 10. Okt 2026](#kategorie-9-chrome-tab-sammlung--10-okt-2026)
10. [Kategorie 10: Neue Sammlung — Doom Scrolling (`NEW DOOM SCROLLING/`) — 10. Okt 2026](#kategorie-10-neue-sammlung--doom-scrolling-new-doom-scrolling--10-okt-2026)
11. [Kategorie 11: Frisch "Starred" auf GitHub (Oktober 2026)](#kategorie-11-frisch-starred-auf-github-oktober-2026)
12. [Kategorie 12: Motion-Design-Prüfung für AOS-Kernel & Creator Extension — 10. Okt 2026](#kategorie-12-motion-design-prüfung-für-aos-kernel--creator-extension--10-okt-2026)
13. [Kategorie 13: Neuzugänge aus Downloads (`Neuer Ordner mit Objekten 2/`) — 10. Okt 2026](#kategorie-13-neuzugänge-aus-downloads-neuer-ordner-mit-objekten-2--10-okt-2026)

---

## Kategorie 1: Direkt hochrelevant für `/bdb-dev AOS`
*Fokus: Coding-Agent-Harnessing, autonome Supervision, Token-Reduktion, MCP-Tools, Skill-Generierung, CI/CD-QA.*

| Name | GitHub / URL | Funktion & Relevanz für AOS | Screenshot-Quelle |
| :--- | :--- | :--- | :--- |
| **AutoHarness** | [github.com/tigerless-labs/autoharness](https://github.com/tigerless-labs/autoharness) | **Self-Learning Skill Layer für Claude Code**: Lernt automatisch neue Fähigkeiten direkt aus realen Arbeitssessions, führt Duplikate zusammen (`fold/reflector`) und bereinigt ungenutzte Skills selbstständig. | `IMG_6904.PNG` |
| **Foreman (ThruWire)** | [github.com/thruwire/foreman](https://github.com/thruwire/foreman) · [thruwire.ai](https://thruwire.ai) | **Autonomer Supervisor für Coding-Agenten**: Begleitet langsame Coding-Agenten (Claude, Cursor, Codex) mit schnellen, deterministischen System-1-Entscheidungen (via Jev-Modell). Erkennt Loops, Blockaden und prüft Arbeitsfortschritt. | `IMG_6962.PNG` |
| **Codebase Memory MCP** | [github.com/DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | **AST Knowledge-Graph MCP Server**: Parst Repositories via Tree-Sitter & LSP in eine lokale SQLite-Wissensdatenbank. Reduziert Kontext-Tokens bei Code-Recherche um bis zu **99%** (z.B. von 412k auf 3.4k Tokens). Direkte Synergie mit Synapse & memB. | `IMG_6981.PNG` |
| **Strix** | [github.com/usestrix/strix](https://github.com/usestrix/strix) | **Autonomer AI Penetration Testing Agent**: Testet Web-Apps und APIs wie ein echter Hacker. Validiert Schwachstellen, generiert PoC-Exploits und liefert Fixes. Go / Bubble Tea TUI. Ideal als Gate-Check vor Releases. | `IMG_6943.PNG` |
| **Pullfrog** | [github.com/pullfrog/pullfrog](https://github.com/pullfrog/pullfrog) | **BYOK CodeRabbit in GitHub Actions**: Autonome PR-Reviews, automatisches Beheben von CI-Fehlern, Merge-Konflikten und Issue-Triage direkt in CI/CD mit Claude, Codex, Grok oder OpenCode. | `IMG_6938.PNG` |
| **Claude-BugHunter** | [github.com/elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) | **Multi-Harness Red-Team & Security Pipeline**: Agent-Skill-Paket für Claude Code, OpenCode, Codex CLI und Antigravity mit Burp MCP Ports, 6-Phasen-Workflow und 7-Fragen-Validierungs-Gate gegen False Positives. | `IMG_6909.PNG` |
| **Coucou (Mochi)** | [github.com/Louis-CFM/coucou](https://github.com/Louis-CFM/coucou) | **MacBook-Notch Agent-Watcher**: Minimaler animierter Begleiter in der macOS-Notch, der Claude Code Sessions überwacht, Permissions einholt, Deploys trackt und schnelle Interaktion ohne Fensterwechsel erlaubt. | `IMG_6906.PNG`, `IMG_6967.jpg` |
| **Claude-Watch** | [github.com/taoufik123-collab/claude-watch](https://github.com/taoufik123-collab/claude-watch) | **Video-Analyse-Skill für Claude**: Ermöglicht Agenten das Verarbeiten von Videos über FFmpeg-Schnittstellenerkennung (Scene-Change), Whisper-Transkripte, 2-fps-Hook-Analyse und Markdown-Reports. | `IMG_6985.PNG`, `IMG_6986.PNG`, `IMG_6987.jpg` |
| **A2A Protocol** | [github.com/a2aproject/A2A](https://github.com/a2aproject/A2A) | **Agent-to-Agent Interoperability Protocol**: Offener Standard zur Kommunikation zwischen unterschiedlichen, isolierten Multi-Agenten-Systemen (Discovery, Modalitäten-Aushandlung, Task-Kollaboration). Ergänzt MCP auf Agent-Ebene. | `IMG_6959.PNG` |
| **Google Artemis** | [github.com/google/artemis](https://github.com/google/artemis) | **Android & Mobile UI Automation mit nativem MCP Server**: Ermöglicht Coding-Agenten das direkte Steuern und Testen von physischen/virtuellen Mobilgeräten via ADB & Computer-Use (Observe-and-Act Loop). | `IMG_6980.PNG` |
| **Mem0** | [github.com/mem0ai/mem0](https://github.com/mem0ai/mem0) | **Persistente Langzeit-Memory für Agenten**: Speichert Konversationen, Entscheidungen und Fakten über Sessions hinweg; verhindert Gedächtnisverlust bei Agenten-Neustarts. | `IMG_6952.PNG` |
| **CrewAI** | [github.com/crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) | **Rollenbasiertes Multi-Agenten-Framework**: Orchestrierung spezialisierter Agenten (Researcher, Writer, Reviewer) über strukturierte Konfigurationen. | `IMG_6950.PNG` |
| **LangChain** | [github.com/langchain-ai/langchain](https://github.com/langchain-ai/langchain) | **Connective Tissue Framework**: Standardisierte Ketten, Tools, Retriever und Gedächtniskomponenten für LLM-Anwendungen. | `IMG_6951.PNG` |
| **Composio** | [github.com/ComposioHQ/composio](https://github.com/ComposioHQ/composio) | **100+ Enterprise Tool-Integrations für Agenten**: Standardisierte Actions und MCP-Schnittstellen für Slack, Notion, GitHub, Salesforce, Gmail u.v.m. | `IMG_6947.PNG` |
| **Switch** | [github.com/flintai/switch](https://github.com/flintai/switch) · [flintai.dev](https://flintai.dev) | **Human-Agent Collaboration Framework**: Bindet KI-Agenten nativ in bestehende Team-Kanäle (Slack, Discord, Linear) ein, inklusive Console und Playground. | `IMG_6910.PNG` |
| **OpenBot** | [github.com/CopilotKit/openbot](https://github.com/CopilotKit/openbot) | **Self-Hosted AI Coworker Stack**: Open-Source-Plattform mit AG-UI, Browser- und Tool-Rechten auf eigener Infrastruktur für interne Mitarbeiter-Agenten. | `IMG_6907.PNG`, `IMG_6973.PNG` |
| **Rust Skills** | [github.com/actionbook/rust-skills](https://github.com/actionbook/rust-skills) | **AI-Powered Rust Development & Meta-Cognition Framework**: Claude Code Plugin & Skill-Suite (Ownership, Borrowing, Concurrency, Unsafe-Checker, Dynamic Skills aus `Cargo.toml`). Schließt die kritische Rust-Lücke in AOS und für den Tauri v2 Rust-Core. | Empfehlung / Neuzugang |

---

## Kategorie 2: Frontend, Design-Skills & UI-Komponenten
*Fokus: Anti-Slop, DTCG-Tokens, UI-Komponenten-Bibliotheken, WebGPU für Agenten & Design-Inspiration.*

| Name | URL / GitHub | Funktion | Screenshot-Quelle |
| :--- | :--- | :--- | :--- |
| **VGPU (Vercel Labs)** | [github.com/vercel-labs/vgpu](https://github.com/vercel-labs/vgpu) · [vgpu.sh](https://vgpu.sh) | **Agent-Ready WebGPU Library**: TypeScript-Framework für WebGPU, Shaders, 3D-Gaussian-Splatting und Raymarching. Speziell entwickelt für die einfache Steuerung durch KI-Coding-Agenten (CLI & MCP-Schnittstellen). | `IMG_6999.PNG` |
| **Transitions.dev** | [github.com/Jakubantalik/transitions.dev](https://github.com/Jakubantalik/transitions.dev) · [transitions.dev](https://transitions.dev) | **UI Transitions Skill für Coding-Agenten**: Kuratierte Sammlung eleganter UI-Transitions, die direkt per Agent-Skill (`npx transitions-dev add ...`) in Projekte eingebaut werden können. | `IMG_6996.PNG` |
| **Cult UI** | [github.com/nolly-studio/cult-ui](https://github.com/nolly-studio/cult-ui) · [cult-ui.com](https://cult-ui.com) | **78+ animierte Primitives & AI-Agent-Patterns**: Erweiterung für shadcn/ui mit Framer Motion, AI-SDK-Mustern und vorgefertigten interaktiven Blöcken. | `IMG_7003.PNG` |
| **Skiper UI** | [skiper-ui.com](https://skiper-ui.com) | 106+ animierte React/shadcn-Komponenten im "Single-File"-Ansatz (Image-Reveal, Hover-Effekte, Dynamic Island). | `IMG_7002.PNG` |
| **Watermelon UI** | [github.com/WatermelonCorp/watermelon-platform](https://github.com/WatermelonCorp/watermelon-platform) · [ui.watermelon.sh](https://ui.watermelon.sh) | 600+ freie Open-Source UI-Komponenten und Dashboards für Entwickler und Design-Teams. | `IMG_7004.PNG` |
| **Impeccable** | [github.com/pbakaus/impeccable](https://github.com/pbakaus/impeccable) | **AI-Design-Skill für Claude / Agenten**: Über 20 Befehle (`craft`, `critique`, `polish`, `audit`, `colorize`) zur Vermeidung von KI-Slop. Erstellt `PRODUCT.md` und `DESIGN.md`. | `IMG_6988.PNG`, `IMG_6989.PNG` |
| **Logo Design Skill** | [github.com/kaankiziltug/logo-design-skill](https://github.com/kaankiziltug/logo-design-skill) | 1.400+ SVG-Referenzen mit automatischen CLI-Prüfskripten (16px-Test, Squint-Test, Mirror-Test) für Claude. | `IMG_6908.PNG` |
| **Backgrounds Supply** | [backgrounds.supply](https://backgrounds.supply) | Hochwertige Texturen, Gradients und Mesh-Hintergründe für Hero-Sections und moderne Webseiten. | `IMG_6995.PNG` |
| **Animos** | [animos.app](https://animos.app) | Browserbasiertes Tool zur Erstellung und zum Export (MP4) von ansprechenden UI-Animationen und Produkt-Showcases. | `IMG_6997.PNG` |
| **Spline 3D** | [spline.design](https://spline.design) | Web-basiertes 3D-Design-Tool mit interaktiven Physik- und Kamera-Events, exportierbar nach React / Three.js / R3F. | `IMG_7001.PNG` |
| **Screenshot-to-Code** | [github.com/abi/screenshot-to-code](https://github.com/abi/screenshot-to-code) | Wandelt Screenshots, Figma-Mockups und Screencasts direkt in sauberen Tailwind-, React- oder Vue-Code um. | `IMG_6958.PNG` |
| **Uiverse.io** | [uiverse.io](https://uiverse.io) · [github.com/Garth-DB/uiverse](https://github.com/Garth-DB/uiverse) | Größte Open-Source-Bibliothek für interaktive CSS- & Tailwind-Elemente (Buttons, Checkboxen, Loader, Karten). | `IMG_6982.PNG` |
| **Readme.so** | [readme.so](https://readme.so) · [github.com/octokatherine/readme-so](https://github.com/octokatherine/readme-so) | Interaktiver visueller Markdown-Editor zum schnellen Zusammenklicken professioneller README-Dateien. | `IMG_6983.PNG` |
| **shadcn/ui** | [ui.shadcn.com](https://ui.shadcn.com) · [github.com/shadcn-ui/ui](https://github.com/shadcn-ui/ui) | Der de-facto Standard: Saubere, zugängliche Primitives zum direkten Kopieren in die Codebase. | `IMG_6960.jpg` |
| **21st.dev** | [21st.dev](https://21st.dev) | Großer Marktplatz für moderne React-Komponenten für individuelles Design abseits des Standard-KI-Looks. | `IMG_6960.jpg` |
| **Magic UI** | [magicui.design](https://magicui.design) · [github.com/magicuidesign/magicui](https://github.com/magicuidesign/magicui) | Spezialisiert auf Landing Pages: Animierte Texte, Marquees, Grids, Spotlight-Karten und Shader-Effekte. | `IMG_6960.jpg` |
| **Aceternity UI** | [ui.aceternity.com](https://ui.aceternity.com) | Hochwertige Micro-Interactions, 3D-Karten, animierte Hintergründe und Framer Motion Effekte (v2.0). | `IMG_6960.jpg`, `IMG_6998.PNG` |
| **Mantine** | [mantine.dev](https://mantine.dev) · [github.com/mantinedev/mantine](https://github.com/mantinedev/mantine) | 100+ React-Komponenten und Hooks für funktionale Web-Applikationen und komplexe Interfaces. | `IMG_6960.jpg` |
| **HeroUI (ex NextUI)** | [heroui.com](https://heroui.com) · [github.com/heroui-inc/heroui](https://github.com/heroui-inc/heroui) | Moderne, polierte React-Komponenten mit nativer Barrierefreiheit für Dashboards und SaaS-Frontends. | `IMG_6961.PNG` |
| **MUI** | [mui.com](https://mui.com) · [github.com/mui/material-ui](https://github.com/mui/material-ui) | Etabliertes Ökosystem für komplexe Enterprise-Dashboards, Datentabellen und Formularlandschaften. | `IMG_6961.PNG` |
| **Chakra UI** | [chakra-ui.com](https://chakra-ui.com) · [github.com/chakra-ui/chakra-ui](https://github.com/chakra-ui/chakra-ui) | Einfaches Styling-System mit modularen, zugänglichen Komponenten für schnelles Prototyping. | `IMG_6961.PNG` |
| **React Aria** | [react-spectrum.adobe.com/react-aria](https://react-spectrum.adobe.com/react-aria) | Headless UI-Primitives von Adobe mit vollständiger Barrierefreiheit und flexibler Styling-Hoheit. | `IMG_6961.PNG` |
| **Tremor** | [tremor.so](https://tremor.so) · [github.com/tremorlabs/tremor](https://github.com/tremorlabs/tremor) | Maßgeschneidert für Analytics: Charts, KPI-Karten und Datenvisualisierungen für Dashboards. | `IMG_6961.PNG` |
| **Mobbin** | [mobbin.com](https://mobbin.com) | Echte UI/UX-Screenflows aus populären Mobile- und Web-Apps zur Analyse von Navigationsmustern. | `IMG_6970.jpg` |
| **Saaspo** | [saaspo.com](https://saaspo.com) | Kuratierte Sammlung bester SaaS-Landing-Pages, Pricing-Grids und Komponenten-Patterns. | `IMG_6971.jpg` |
| **Pageflows** | [pageflows.com](https://pageflows.com) | Vollständige Video-Aufzeichnungen von User Flows (Onboarding, Checkout, Upgrades) aus realen Produkten. | `IMG_6972.jpg` |

---

## Kategorie 3: Video & Creative Media Tech
*Fokus: Programmatischer Videoschnitt, lokale ComfyUI-Generierung, Timeline-Editoren, Audio-Bereinigung.*

| Name | GitHub / URL | Funktion | Screenshot-Quelle |
| :--- | :--- | :--- | :--- |
| **OpenCut** | [github.com/OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) | **Open-Source CapCut Alternative**: Datenschutzfreundlicher, plattformübergreifender Videoeditor gebaut mit Rust, GPUI und React. Multi-Track-Timeline, Ripple-Edits und Keyframes ohne Cloud-Zwang. | `IMG_6968.PNG` |
| **fframes** | [github.com/fframes-studio/fframes](https://github.com/fframes-studio/fframes) · [fframes.studio](https://fframes.studio) | **GPU-beschleunigtes Video-Coding-Framework**: Rendert Videos programmatisch via Rust und SVG direkt auf der GPU, statt auf langsame Browser-Canvas-Renderer zu warten. Hohe Relevanz für Hyperframes/OpenMontage. | `IMG_6895.PNG` |
| **OpenChatCut** | [github.com/0xsl1ne/OpenChatCut](https://github.com/0xsl1ne/OpenChatCut) | **Lokaler Konversations-Videoeditor**: Steuerung der Multitrack-Timeline durch natürliche Sprache; fügt automatisch Untertitel, Übergänge und Musik hinzu. | `IMG_6940.PNG` |
| **Pixelle-Video** | [github.com/AIDC-AI/Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video) | **End-to-End KI-Videoengine via ComfyUI**: Erzeugt aus einem simplen Text-Prompt ein komplettes Kurzvideo inkl. Drehbuch, Bildgenerierung, Voiceover und Schnitt lokal auf der eigenen GPU. | `IMG_6905.PNG` |
| **Open-Generative-AI** | [github.com/Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | **Self-Hosted AI Studio mit 400+ Modellen**: Bündelt Bild- und Videomodelle (Flux, Kling, Sora, Wan) in einer filterfreien, selbst gehosteten Oberfläche. | `IMG_6944.PNG` |
| **Auto-Editor** | [github.com/WyattBlue/auto-editor](https://github.com/WyattBlue/auto-editor) | **Automatischer Stille- & Pause-Schneider**: CLI-Werkzeug, das Sprechpausen und stille Passagen aus Audio- und Videodateien automatisch herausschneidet. | `IMG_6945.PNG` |
| **ani-cli** | [github.com/pystardust/ani-cli](https://github.com/pystardust/ani-cli) | Leichtgewichtiges POSIX-Shell CLI-Tool zum schnellen Streamen und Scrapen von Anime im Terminal. | `IMG_6957.PNG` |
| **Video Arena Elo Ranking** | Artificial Analysis | Rangliste führender Video-Generierungsmodelle (Sep 2026: Wan 3.0, Utopai X, Seedance 2.5, MiniMax H3, Gemini Omni Flash 1.1). | `IMG_6942.PNG` |

---

## Kategorie 4: Gründer- & Strategie-Skills für Claude Code

| Name | GitHub / URL | Funktion | Screenshot-Quelle |
| :--- | :--- | :--- | :--- |
| **Claude Skills Founder (Pricing Strategy)** | [github.com/emotixco/claude-skills-founder](https://github.com/emotixco/claude-skills-founder) | **SaaS-Pricing & Founder Toolkit für Claude Code**: Befehle wie `/founder:pricing-strategy` zur systematischen Evaluierung von Preismodellen, Tier-Strukturen und Unit Economics direkt im Terminal. | `IMG_6994.PNG` |

---

## Kategorie 5: Architektur-Blueprints, Agent-Muster & Intentional Prompts
*Fokus: Methoden, die direkt in AOS-Regeln, Hooks oder Agent-Playbooks übernommen werden können.*

### 1. Das "Every Stage Commits a File" Playbook (`IMG_6991.jpg`)
Ein von Anthropic inspiriertes AI-SDLC-Vorgehen mit unveränderlichem Git-Audit-Trail:
```
AN IDEA  --->  01: intent.md  (Die Idee aufgeschrieben)       [Git Commit: a1c93f2]
         --->  02: spec.md    (Was das System können muss)     [Git Commit: 4e7b0d1]
         --->  03: plan.md    (Wie es konkret gebaut wird)     [Git Commit: 9f2ac58]
```
*Bedeutung für AOS:* Perfekt kompatibel mit unserem `production_artifacts/00_execution_plan.md` und dem `GO`-Gate-Protokoll.

### 2. Die 3-Schichten-Memory-Architektur (`IMG_6990.PNG`)
```
Layer 01: EPISODIC   -> "What happened"  (Konversationsverläufe, Sessions, Logs)
Layer 02: SEMANTIC   -> "What's true"    (Fakten, Architekturregeln, Wissensgraph)
Layer 03: PROCEDURAL -> "What works"     (Etablierte Skills, Patterns, Best Practices)
```
*Bedeutung für AOS:* Direkte Strukturierung für `memB` und `openwiki`.

### 3. Loop Engineering vs. Graph Engineering (`IMG_6902.PNG`)
* **Problem ("The Ceiling"):** Lineare sequentielle Schleifen (`Unit A -> Unit B -> Unit C`) warten unnötig aufeinander, selbst wenn keine Daten zwischen ihnen übergeben werden.
* **Lösung:** Echte Graphen (`Split -> Parallel Workers -> Merge -> Quality Gate`). Die goldene Regel: *„Wenn du die Variable nicht benennen kannst, die zwischen zwei Schritten fließt, existiert keine Edge – das Warten ist reine Verschwendung.“*

### 4. Die zwei Rückkopplungspfade ("Two Return Paths") (`IMG_6903.PNG`)
* **Kurzer Pfad (Correction Edge):** Feedback zurück an die fehlerhafte Unit im aktuellen Lauf (behebt das Problem jetzt).
* **Langer Pfad (Learning Edge):** Das akzeptierte Ergebnis wandert als neuer Constraint zurück in das Briefing des Splitters für alle zukünftigen Läufe (das System lernt dauerhaft dazu).

### 5. Intentional Frontend Design Prompts (Anti-AI-Look) (`IMG_6974` – `IMG_6977`)
Vier präzise Prompts zur Beseitigung des generischen "Vibe-Coded" Looks:
1. **Prompt 01 – Fix the Hierarchy:**  
   *„Audit typography, spacing, scale, alignment and CTA prominence. Redesign the hierarchy so users know what to look at first.“*
2. **Prompt 02 – Remove the AI Look:**  
   *„Remove generic gradients, excessive cards, pills and predictable layouts. Build a distinctive visual system instead.“*
3. **Prompt 03 – Fix the First 5 Seconds:**  
   *„Explain what it is, who it is for, why it matters and what to do next — above the fold.“*
4. **Prompt 04 – Do the Designer Pass:**  
   *„Review the running website. Find the 10 highest-impact design problems. Fix them, reopen the site, and review it again.“*

### 6. Claude Opus 5.5 Multi-Agent Ordnerstruktur (`IMG_6911.jpg`)
Ein erprobtes Setup für agentische Teams:
```
agent-team/
├── .claude/
│   ├── CLAUDE.md          # Globale Regeln & Guardrails
│   ├── settings.json
│   └── hooks/             # session-start, pre-tool-use, post-tool-use, stop
├── agents/                # Spezialisten mit frischem Kontext
│   ├── planner.md
│   ├── researcher.md
│   ├── builder.md
│   ├── reviewer.md
│   └── router.md
├── playbooks/             # Wiederholbare Prozesse (Content, Product, Growth)
├── skills/                # Reusable Agent Capabilities
└── memory/
    └── MEMORY.md          # Cross-Session Recall
```

---

## Kategorie 6: Interne Workspace-Snapshots & Event-Notizen
*Eigene Bildschirmaufnahmen und persönliche Notizen:*
* **`IMG_6893.PNG`**: Pull Request im internen Repo `hybridlabor-api/aos` (`fix(installer): write an agy-valid hook...`).
* **`IMG_6894.PNG`, `IMG_6897.PNG`, `IMG_6898.PNG`, `IMG_6900.PNG`, `IMG_6901.PNG`**: Tim's AO-Master-Session (Agent Orchestrator, ListAgents, Commit `2d64e8d`, Mode-Classifier-Diskussion, Subagent-Auftragsvergabe als Start-Prompt statt Peer-Message).
* **`IMG_6913.jpg`**: Privater Chat-Ausschnitt zu Bogotá / Event-Empfehlungen.
* **`IMG_6993.jpg`**: Event-Ticket / Gästeliste (`wyldhearts.guestlist.pro` – Kalif Storch Erfurt).

---

## Kategorie 7: Relevant für `saasengine`
*Fokus: Self-Hosted Cloud-Infrastruktur, Multi-Cloud Fleet (Oracle, Hetzner, GCP), Headless CMS, APIs, No-Code Tools, Serverless Jobs.*

| Name | GitHub / URL | Funktion & Relevanz für Saasengine | Screenshot-Quelle |
| :--- | :--- | :--- | :--- |
| **Coolify** | [github.com/coollabsio/coolify](https://github.com/coollabsio/coolify) · [coolify.io](https://coolify.io) | **Open-Source PaaS (Heroku / Vercel Alternative)**: Zentrale Orchestrierung für Bare-Metal- und Cloud-Server via SSH. Ideal für die BDB-Flotten-Bereitstellung von Apps, Datenbanken und Services ohne Vendor Lock-in. | `IMG_6978.PNG` |
| **Open SaaS** | [github.com/wasp-lang/open-saas](https://github.com/wasp-lang/open-saas) · [opensaas.sh](https://opensaas.sh) | **Fullstack SaaS Starter Kit (Wasp / React / Node / Prisma)**: Bringt Stripe-Abrechnung, Rollen/Auth, Background Jobs und E-Mail-Templates out-of-the-box mit. Ausgezeichnete Vorlage für Saasengine-Endprodukte. | `IMG_6946.PNG` |
| **Directus** | [github.com/directus/directus](https://github.com/directus/directus) | **Headless SQL-First Data Engine & CMS**: Stülpt sofort REST- und GraphQL-APIs über bestehende SQL-Datenbanken (Postgres/MySQL) mit granularer Rechteverwaltung und Web-Studio. | `IMG_6953.PNG` |
| **ToolJet** | [github.com/ToolJet/ToolJet](https://github.com/ToolJet/ToolJet) | **Low-Code Internal Tools Builder (Retool-Alternative)**: Schneller Bau von Admin-Dashboards, Datenbank-UIs und Kunden-Backends mit visuellen Komponenten und Anbindung an interne APIs. | `IMG_6954.PNG` |
| **Listmonk** | [github.com/knadh/listmonk](https://github.com/knadh/listmonk) | **Hochperformanter Self-Hosted Newsletter & Transaktions-Mailer**: Schneller Go-basierter E-Mail-Dienst (Mailchimp-Alternative) für Massen-Mails und System-Nachrichten bei minimalem Ressourcenverbrauch. | `IMG_6955.PNG` |
| **Outline** | [github.com/outline/outline](https://github.com/outline/outline) | **Team Knowledge Base & Wiki**: Schnelles, schickes Dokumentations- und Wissenssystem (Notion/Confluence-Alternative) für interne Teams und Kundenhandbücher. | `IMG_6956.PNG` |
| **Maxun** | [github.com/getmaxun/maxun](https://github.com/getmaxun/maxun) | **No-Code Web Scraping & Crawler Engine**: Wandelt Webseiten automatisch in strukturierte REST-APIs um. Unterstützt visuelles Extrahieren, Pagination und AI-Parsing. | `IMG_6939.PNG` |
| **Agentic Inbox** | [github.com/cloudflare/agentic-inbox](https://github.com/cloudflare/agentic-inbox) | **Serverless AI Email Client auf Cloudflare**: Vollständiger Mail-Client, der autonom E-Mails liest, kategorisiert und beantwortet. Läuft serverless auf Cloudflare Workers/Agents. | `IMG_6965.PNG` |
| **Shoutrrr / Shouter** | [github.com/coollabsio/shoutrrr](https://github.com/coollabsio/shoutrrr) | **Social Media Scheduler (Buffer / Typefully Alternative)**: Zentrales Verfassen und zeitgesteuertes Ausspielen von Beiträgen auf X, LinkedIn, Instagram und Bluesky. Self-hosted über Docker/Coolify. | `IMG_6941.PNG` |
| **Bento** | [github.com/nyblnet/bento](https://github.com/nyblnet/bento) · [bento.page](https://bento.page) | **Single-File Local-First Office Suite**: Das gesamte Dokumenten- und Präsentations-Tool passt in eine einzige HTML-Datei. Keine Cloud-Abhängigkeiten, KI-lesbares JSON-Format, Claude-Plugin. | `IMG_6968.PNG` |
| **Replicate API** | [replicate.com](https://replicate.com) | **Serverless GPU Model Execution**: Ausführen tausender Open-Source-Modelle (Flux, SDXL, Whisper, LLMs) per API ohne eigene GPU-Cluster-Wartung. | `IMG_6948.PNG` |
| **Tavily API** | [tavily.com](https://tavily.com) | **Real-Time AI Web Search API**: Speziell für LLM-Agenten optimierte Websuche mit strukturierten Quellen und bereinigtem Markdown-Content. | `IMG_6949.PNG` |
| **MuAPI** | [muapi.ai](https://muapi.ai) | **All-in-One Model Gateway & API Proxy**: Einheitlicher Zugang zu Multi-Model-APIs, Assistenten und Agenten-Workflows mit einheitlichem Abrechnungs- und Concurrency-Handling. | `IMG_6899.PNG` |

---

## Kategorie 8: Neue Sammlung — 7. Okt 2026 (`github repos neue sammlung 7 okt/`)
*40 neue Screenshots (IMG_7005 – IMG_7052), alle Links via Web-Recherche verifiziert. Einträge mit vorhandenem MD-Treffer sind am Ende der Datei im Duplikat-Log vermerkt.*

### 8.1 Agent-Harness, Orchestrierung & AOS-relevante Tools

| Name | GitHub / URL | Funktion & Relevanz | Screenshot |
| :--- | :--- | :--- | :--- |
| **OpenRig** | [github.com/mvschwarz/openrig](https://github.com/mvschwarz/openrig) · [openrig.dev](https://openrig.dev) | **Multi-Agent-Harness (Claude Code + Codex als ein System)**: Agent-Team in YAML (RigSpec) definiert, `rig up` bootet tmux-Sessions, Topologie-Graph-TUI, Sessions adoptieren, `rig send/broadcast/chatroom`, Snapshot/Restore. ~2k Stars, npm `@openrig/cli`. Konkurrenz/Synergie zu AO-Orchestrator. | `IMG_7008` |
| **GitBot** | [github.com/gitbot-hq/GitBot](https://github.com/gitbot-hq/GitBot) | **"Give your coding agents a home"**: Lokaler Server (Port 3000), der Claude Code/Codex/OpenCode aus dem Browser fernsteuert — wiederverwendbare Bots, persistente Threads, per-Bot Permissions. npm `@gitbot-hq/gitbot`. Vergleichbar mit Coucou/GitHub-Remote-Steuerung. | `IMG_7048` |
| **Warren** | [github.com/Dymyt-ry/warren](https://github.com/Dymyt-ry/warren) · [warren.golobokov.dev](https://warren.golobokov.dev/) | **"Agents are teammates now. Give them a room."**: Ein Baum aus Räumen für Menschen + Coding-Agenten; `@mention` landet direkt in der laufenden Session. Local-first (localhost:8790), MIT. | `IMG_7022` |
| **Raven (EverMind)** | [github.com/EverMind-AI/Raven](https://github.com/EverMind-AI/Raven) · [raven.evermind.ai](https://raven.evermind.ai/) | **"The Harness of Harnesses", gebaut für RSI (recursive self-improvement)**: Host-Agent, der eigene + Third-Party-Agenten (Claude Code, Codex, OpenCode, Hermes, OpenClaw…) orchestriert; EverOS-Memory (Markdown-native, local-first), Evolver bewertet Harness-Änderungen gegen Benchmarks. 4.4k Stars, Apache-2.0, pre-alpha. | `IMG_7049` |
| **PRP-core (Wirasm)** | [github.com/Wirasm/prp](https://github.com/Wirasm/prp) | **PRP-Methodik (Product Requirement Prompts = PRD + Codebase-Intelligence + Runbook)**: Plugin mit `/prp-core:prp-prd`, `/prp-core:prp-plan`, `/prp-core:prp-implement`, `/prp-loop` (headless plan→implement→PR→review Loop). 2.2k Stars. Direkt vergleichbar mit unserem Plan-Cycle. | `IMG_7020` |
| **Watch Skill · DeepWatch** | [github.com/oxbshw/watch-skill](https://github.com/oxbshw/watch-skill) | **"Give AI agents eyes, ears, and verifiable results"**: Video/Audio/Screenshots → persistenter, timestamped Evidence-Index (OCR, Whisper, 1800+ Quellen); 39 MCP-Tools + CLI + REST; THE LOOP (capture→critique→fix→verify) prüft Agentenarbeit deterministisch. Functional twin von Claude-Watch (s. Kat. 1) — andere Codebasis. | `IMG_7021` |
| **Hermarchy (Omarchy-Theme)** | [github.com/archer-clawbot/omarchy-hermarchy-theme](https://github.com/archer-clawbot/omarchy-hermarchy-theme) | **Research-Workstation-Theme für Omarchy** mit optionalem Hermes-Agent-Status-Panel (Quickshell-Plugin). ~86 Stars. Interessant als Aesthetic-Referenz ("cyan is semantic, not decorative") für eigene Agent-UIs. | `IMG_7007` |
| **Jev Engineering Tree (@polydao)** | [x.com/polydao](https://x.com/polydao) | **Prompt-Methodik (kein Repo)**: Claude-Code-Agent-Tree mit Fable-Advisor (liest alles, schreibt nie), Jev-Fork-Layer (deterministische which-file/which-tool/retry-Entscheidungen < 0,5s statt Opus-Aufrufen), 3 Subagenten (medium effort), Review+Verify vor Ship. Passgenau zu unserer Harness-/Token-Einspar-Diskussion. | `IMG_7011` |
| **Claude Code Mods (News)** | ClaudeDevs (X) | **News-Impuls**: Claude Code ist jetzt moddable — Mods aus TypeScript in Plugins (`/plugin`), UI-Verhalten, Statuslines (z.B. "Token Weather") austauschbar. Relevant für AOS-Plugin-Strategie. | `IMG_7033` |
| **Glitch Orchestra** | @kemb_glitch (Instagram) — **noch nicht released** | **"A Claude Code Mod"** vom Glitch Cat Club: Pixel-Arbeiter (conductor/frontend/copy/tests) orchestrieren Claude-Code-Sessions mit Live-Status. Experimental, "sharing soon" — Watchlist-Eintrag. | `IMG_7029`, `IMG_7043`–`IMG_7047` |

### 8.2 Frontend, Design & UI

| Name | GitHub / URL | Funktion | Screenshot |
| :--- | :--- | :--- | :--- |
| **designlang** | [github.com/Manavarya09/design-extract](https://github.com/Manavarya09/design-extract) · [designlang.app](https://designlang.app) | **`npx designlang <url>` extrahiert komplette Design-Systeme von Live-Websites**: W3C-DTCG-Tokens (primitive/semantic/composite), Tailwind-Config, Figma-Variablen, shadcn-Theme, Brand-Book-PDF, MCP-Server für Claude Code/Cursor, WCAG-Remediation. ~4k Stars, MIT. Passt exakt zu DTCG-/Token-Disziplin von Godmode UI/UX. | `IMG_7051` |
| **Componentry** | [github.com/harshjdhv/componentry](https://github.com/harshjdhv/componentry) · [componentry.dev](https://componentry.dev) | Animierter React-Component-Library (Partikel-Typografie, Liquid-Glass, WebGL-Gradients, Kinetic Text); Install via `npx shadcn @latest add @componentry/...` + MCP. Vercel-OSS-backed. | `IMG_7031` |
| **Space UI** | [spaceui.one](https://www.spaceui.one) (by @adrielzimbril) | 101+ interaktive Komponenten für Next.js/Base UI & Tailwind — Liquid-Switches, Morphing-Controls, Shaders, Tactile Microinteractions; MIT, shadcn-CLI-Install. | `IMG_7032` |

### 8.3 Video & Creative Media Tech

| Name | GitHub / URL | Funktion | Screenshot |
| :--- | :--- | :--- | :--- |
| **onetake** | [github.com/feitangyuan/onetake](https://github.com/feitangyuan/onetake) | **Claude Agent Skill für "One-Continuous-Take"-Motion-Films**: Launch-Films/Teaser, wo jeder Beat aus dem vorherigen wächst statt PPT-artiger Szenen-Stack; Continuity-Oracle misst Carry-Score; klingt wie eine direkte Konkurrenz/Inspiration zu Hyperframes/OpenMontage. PolyForm-Noncommercial, ~1.3k Stars. Install: `git clone ... ~/.claude/skills/onetake`. | `IMG_7012` |
| **Luma-Dream-Machine-Pro-Premium-Edition** | [github.com/Dragonkrebaza](https://github.com/Dragonkrebaza) | Prompt-/Presets-Sammlung für Luma Dream Machine (Video-Generierung). Qualität unklar — tief priorisiert. | `IMG_7052` |

### 8.4 Skill-Sammlungen: Legal, Marketing & Prompts

| Name | GitHub / URL | Funktion | Screenshot |
| :--- | :--- | :--- | :--- |
| **Lawve · awesome-legal-skills** | [github.com/lawve-ai/awesome-legal-skills](https://github.com/lawve-ai/awesome-legal-skills) · [lawve.ai](https://lawve.ai) | **70+ kuratierte Agent-Skills für Legal-Work** (NDA-Review, GDPR, Due-Diligence, Commercial Law), beigesteuert von Praktikern; portable Standards statt proprietärer Formate. ~700 Stars. | `IMG_7013` |
| **social-ai-team** | [github.com/stevenflanagan1/social-ai-team](https://github.com/stevenflanagan1/social-ai-team) | **Komplettes AI-Social-Team für SMBs als Claude-Code-Skills** (10 Skills): Brand-Onboarding, Content-Calendar, Caption-Writer, Creative-Designer (Nano Banana), LinkedIn-Writer, Performance-Review. | `IMG_7052` |
| **everything-claude-marketing** | [github.com/brainbytes-dev/everything-claude-marketing](https://github.com/brainbytes-dev/everything-claude-marketing) | **Komplettes Marketing-Intelligence-System für Claude Code**: 18 Agents, 72 Skills, 22 Commands (Strategist, SEO, Paid Ads, Growth-Hacker, PR, CRO …). | `IMG_7052` |
| **creative-director-skill** | [github.com/smixs/creative-director-skill](https://github.com/smixs/creative-director-skill) · [cd-skill.com](https://cd-skill.com) | **"World-class creative director in a skill"**: Ideation via SIT/TRIZ/Lateral Thinking + Cannes-Lions-Evaluations-Engine, kalibriert gegen 571 legendäre Kampagnen (Originalitäts-Cap gegen Pattern-Sättigung). ~235 Stars, CC-BY-4.0. | `IMG_7052` |
| **Prompsy** | [prompsy.com](https://prompsy.com) | **"The prompt operating system"**: Prompts speichern/organisieren/optimieren, Bakeoffs (gleicher Prompt × 6 Modelle + Auto-Judge), Snap-&-Mirror (Screenshot → Smart Prompt), Chrome-Extension `/prompsy` überall, Flows-Canvas. SaaS, kein OSS-Repo bekannt. | `IMG_7006` |

### 8.5 Duplikat-Log (Abgleich gegen bestehende MD-Einträge)

| Screenshot | Fund | Status |
| :--- | :--- | :--- |
| `IMG_7050` | **Coucou for iPhone** ([github.com/Louis-CFM/coucou](https://github.com/Louis-CFM/coucou)) | ⚠️ **Doppelt** — Repo steht bereits in Kategorie 1 (Coucou/Mochi). Neu: iPhone-App mit Face-ID-Approval, "Message your session" → VS Code, Widgets/Live Activity, private iCloud — Kurzbeschreibung in Kat. 1 ggf. erweitern. |
| `IMG_7021` | watch-skill vs. **Claude-Watch** (Kat. 1) | 🔁 **Ähnlich, nicht identisch** — gleiche Zweckklasse (Video→Evidence für Agenten), verschiedene Repos. Beide behalten. |
| `IMG_7005` | Instagram-Reel "Someone Open-Sourced an Entire AI Company — 250+ agents" (theautomationguy.ai) | ❓ **Repo nicht auflösbar** aus dem Screenshot (kein Repo-Name sichtbar). Falls bekannt, nachtragen. |
| `IMG_7018` | htx_studio "Auto-aiming Trash Can" (Reel) | ⏭️ Kein Repo-Eintrag — Hardware-Funprojekt. |
| `IMG_7010` / `IMG_7014` | Glassy Dashboard / "30k Particles, Zero Spinners" (louis_rlee) | 🎨 Nur Design-Inspiration, kein greifbares Repo. |

### 8.6 Interne Screenshots & Notizen (Kategorie 6 Fortsetzung)

* **`IMG_7030`**: Claude Code 2.1.289 Changelog (3. Okt) — `agent.spawn` für Teammates, `$.agent.list()` idle/waiting States.
* **`IMG_7034`**: GitHub-Actions-Budget E-Mail `hybridlabor-api` — 2.000/2.000 Minuten aufgebraucht, Reset 1. Nov 2026, Budget-Gate setzen!
* **`IMG_7035`–`IMG_7037`**: Mem0-Token-Sparstrategien (Top-K reduzieren, Graph-Memory-Konsolidierung, Metadata-Filter, nur letzte 1–2 Messages extrahieren, lokale Embeddings via Ollama/HF).
* **`IMG_7038` / `IMG_7040`**: Eigene Tools — BDB AO Orchestrator "Studio Floor" (festivalpos, 9 Agents aktiv) und Plan Canvas Roadmap (`01_full_roadmap.html`).
* **`8d57ee0f…JPG` / `8dac7934…JPG`**: WinSCP-/SSH-Connect-Troubleshooting auf `awsbdb2.rcentry.pro` (LatamJ) — Ops-Notiz, kein Repo.
* **`ScreenRecording_10-03-2026….MP4`**: Screen Recording vom 3. Okt — noch nicht ausgewertet (kann bei Bedarf sequenziell gelesen werden).

---

## Kategorie 9: Chrome-Tab-Sammlung — 10. Okt 2026
*12 offene Tabs aus Chrome ("Sammlung"). Beschreibungen stammen aus den Seitentiteln der Tabs; die Repos wurden nicht im Detail geprüft.*

### 9.1 Video-Analyse (relevant für Kampagnen-Analyse)

| Name | GitHub / URL | Funktion & Relevanz |
| :--- | :--- | :--- |
| **claude-video** | [github.com/bradautomates/claude-video](https://github.com/bradautomates/claude-video) | **"Give Claude the ability to watch any video"**: `/watch` lädt das Video, extrahiert Frames, transkribiert und übergibt alles an Claude. Dritter Kandidat neben Claude-Watch und Watch Skill (Kat. 1 / 8.1). **README geprüft (MIT):** voll lokal mit `local`-Engine (Python 3.10+, ffmpeg, yt-dlp, WhisperX; ca. 3 GB Platz, 8 GB RAM); Gemini/Groq/OpenAI sind optionale Cloud-Wege (Gemini lädt Videos zu Google hoch). Instagram Reels sind in der README nicht erwähnt — yt-dlp kann sie evtl. laden, ungetestet. |
| **video-to-markdown** | [github.com/marcomontalbano/video-to-markdown](https://github.com/marcomontalbano/video-to-markdown/tree/main) | Videos in Markdown-Dateien einbetten (Vorschaubild + Link). Nützlich für Reports mit Video-Referenzen. README geprüft: braucht einen Cloudinary-Account und pnpm, anonyme Analytics (Simple Analytics) — für lokalen Einsatz ungeeignet. |

### 9.2 Agent-Skills, Gateways & Security

| Name | GitHub / URL | Funktion & Relevanz |
| :--- | :--- | :--- |
| **OmniRoute** | [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | **Freies MIT-AI-Gateway**: ein Endpoint, 359 Provider (150+ gratis), 1200+ Modelle; Quota-aware Auto-Fallback, RTK+Caveman-Kompression (15–95 % Token-Ersparnis), MCP/A2A. Läuft mit Claude Code, Codex, Cursor, OpenCode, Cline, Copilot. |
| **golive-skill** | [github.com/mikehasa/golive-skill](https://github.com/mikehasa/golive-skill) | **Agent-Skill + Node-CLI (ohne Abhängigkeiten)**: bringt ein Agent-Produkt live (Hosting, DB, Domain, E-Mail, Payments) auf eigenen Accounts; Ablauf detect → plan → approve → apply → verify. Kein Backend, keine Telemetrie. README geprüft (MIT): Zugangsdaten liegen im Klartext in `~/.config/golive/credentials` (Modus 0600); braucht Accounts bei Vercel/Netlify, Supabase/Neon, Registrar, Resend, Stripe. |
| **security-audit-skill (Cloudflare)** | [github.com/cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | Coding-Agent-Skill für mehrphasige Security-Audits mit unabhängig verifizierten, maschinenlesbaren Findings. Vergleichbar mit Strix / Claude-BugHunter (Kat. 1). |
| **second-brain-os** | [github.com/undefined-ui/second-brain-os](https://github.com/undefined-ui/second-brain-os) | Selbstpflegende AI-Wissensdatenbank für Claude Code + Obsidian: Guide, Starter-Vault, Agent-Skills, Skripte. Vergleichbar mit memB / OpenWiki. |
| **mattpocock/skills v1.3.1** | [github.com/mattpocock/skills/releases/tag/v1.3.1](https://github.com/mattpocock/skills/releases/tag/v1.3.1) | **Changelog v1.3.1 geprüft:** 1. `resolving-merge-conflicts` ersatzlos entfernt (Agenten lösen das nativ). 2. Konvention `CONTEXT.md` zu `GLOSSARY.md`/`GLOSSARY-MAP.md` umbenannt (für `domain-modeling`, `grill-with-docs`, etc.). 3. Cross-Skill-Aufrufe standardisiert auf expliziten Aufruf `Call the Skill tool with "<name>"` statt `/skill`-Syntax (harness-neutral). 4. `grilling`: Trennlinien (`---`) zwischen aufeinanderfolgenden Fragen ergänzt. |
| **inertia-ai 0.1.0** | [github.com/nettanvirdev/inertia](https://github.com/nettanvirdev/inertia/releases/tag/v0.1.0) | Erstes Release von inertia-ai. README geprüft (MIT): Desktop-Workspace für lokale AI-Agenten (Tauri 2, React 19), nur Windows getestet; API-Keys liegen unverschlüsselt, die Shell läuft mit Nutzerrechten. |

### 9.3 Design, Tools & offene Fragen

| Name | URL | Hinweis |
| :--- | :--- | :--- |
| **ascii.rest** | [ascii.rest](https://ascii.rest/) | Animierte ASCII-Art für Webseiten (von @bas3line). Design-Inspiration. |
| **Morphy** | [get.appmorphy.com](https://get.appmorphy.com/) | "Early access"-Seite, Funktion aus dem Titel nicht ersichtlich. |
| **yanliudesign (Yan Liu)** | [github.com/yanliudesign](https://github.com/yanliudesign) | GitHub-Profil eines Designers; relevante Repos noch nicht ermittelt. |
| **Promix (X-Post)** | [x.com/Promixyz/status/2102424036416348494](https://x.com/Promixyz/status/2102424036416348494) | Post mit einem Kurzlink; Inhalt unklar, Repo nicht aufgelöst. |

---

## Kategorie 10: Neue Sammlung — Doom Scrolling (`NEW DOOM SCROLLING/`) — 10. Okt 2026
*96 neue Screenshots ausgewertet (IMG_7114 – IMG_7234). Alle GitHub-Repositories und URLs wurden via GitHub-API verifiziert. Duplikate zu vorherigen Sammlungen sind im Duplikat-Log ausgewiesen.*

### 10.1 Agent OS, Harnessing, Multi-Agent Swarms & Supervision

| Name | GitHub / URL | Funktion & Relevanz für AOS | Screenshot |
| :--- | :--- | :--- | :--- |
| **Claude Code Mods** | [github.com/nateherkai/claude-code-mods](https://github.com/nateherkai/claude-code-mods) | **4 unverzichtbare UI-Mods für Claude Code**: 1. `CacheKeeper` (Echtzeit-Timer für 5-Min-Cache-Expiry, Token-Kosten-Warnung), 2. `Goal Tracker` (visueller Fortschrittsbalken & Subtask-Liste), 3. `Collision Guard` (erkennt Datei-Konflikte bei mehreren parallelen Sessions, Worktree-Prompt), 4. `Next Steps` (Aktionsvorschläge nach jedem Turn). | `IMG_7153`–`IMG_7157`, `IMG_7194` |
| **Council of High Intelligence** | [github.com/0xNyk/council-of-high-intelligence](https://github.com/0xNyk/council-of-high-intelligence) | **Multi-Perspektiven-Beratung für harte Entscheidungen**: Lässt 18 historische und technische Denker (Socrates, Feynman, Munger, Lovelace, Rams, Musashi, Torvalds, Karpathy, Aurelius) gegeneinander debattieren, bevor Code geschrieben wird. Für Claude Code, Codex, Gemini CLI und OpenCode. | `IMG_7115`, `IMG_7116` |
| **Herdr** | [github.com/herdrdev/herdr](https://github.com/herdrdev/herdr) · [herdr.dev](https://herdr.dev) | **"The runtime your coding agents live on"**: Isolierte Ausführungsumgebung und lokales Sandboxing für Coding-Agenten. ~33k Stars, Apache-2.0. | `IMG_7142` |
| **Agents Observe** | [github.com/simple10/agents-observe](https://github.com/simple10/agents-observe) | **Echtzeit-Observability-Dashboard für Claude Code & Codex**: Lokales Web-Dashboard (`localhost:5173`) mit Multi-Agenten-Filterung, Session-Replay, Suchfunktion und genauer Token-Kostenanalyse. | `IMG_7160` |
| **Headroom** | [github.com/headroomlabs-ai/headroom](https://github.com/headroomlabs-ai/headroom) · [github.com/gglucass/headroom-desktop](https://github.com/gglucass/headroom-desktop) | **Kontext-Kompressions-Layer für KI-Agenten**: Reduziert Input-Tokens um bis zu **57%** (bei JSON/RAG 60–95%) durch intelligentes Pruning, behält aber kritische Logs (z.B. FATAL-Zeilen) byte-genau bei. Desktop-App (`Glance Switch / AG`) läuft lokal auf macOS ohne Cloud-Uploads. | `IMG_7161`, `IMG_7189` |
| **Repowise** | [github.com/repowise-dev/repowise](https://github.com/repowise-dev/repowise) | **AST Codebase Intelligence & Health MCP**: Parst Dependency Graphs, Git-Historie, Tests und Architekturentscheidungen. Verhindert, dass Agenten bei jedem Prompt teuer die gesamte Codebase neu durchsuchen müssen. AGPL-3.0. | `IMG_7166` |
| **REA (Reverse Engineer Anything)** | [github.com/morluto/rea](https://github.com/morluto/rea) | **Reverse Engineering MCP für Agenten**: Ermöglicht Coding-Agenten das automatisierte Analysieren und Decompilieren von Binärdateien, Web-APIs und App-Interna. #3 Trending Repo of the Day. | `IMG_7182` |
| **Whiteboard** | [github.com/devdotfast/whiteboard](https://github.com/devdotfast/whiteboard) | **Open-Source Canvas für Mensch-Agent-Design**: Desktop-App mit SDK für Claude Code und Codex, auf dem Agenten Systemarchitekturen, Flussdiagramme und UI-Konzepte visuell live aufzeichnen können. MIT. | `IMG_7192` |
| **Bops** | [github.com/OrgoAI/bops](https://github.com/OrgoAI/bops) · [bops.bot](https://bops.bot) | **Autonome Business-Ops Bot-Flotte**: Mac-App, bei der jeder Bot einen eigenen Orgo-Cloud-Computer mit 4 Bildschirmen hat. Zugriff auf 1000+ Tools via Composio, Langzeitgedächtnis via Honcho und Computer Use via Codex. FSL-1.1. | `IMG_7124` |
| **AI Employees** | [github.com/markfulton/ai-employees](https://github.com/markfulton/ai-employees) | **8 vordefinierte Rollen mit 60 automatisierten Routinen**: Läuft auf Claude Code und 10 weiteren Harnesses. Führt Browser- und Business-Aufgaben selbstständig aus und lernt mit jedem Lauf dazu. MIT. | `IMG_7234` |
| **TablePlus VMPal** | [vmpal.app](https://vmpal.app) · [github.com/TablePlus/VMPal-issue-tracker](https://github.com/TablePlus/VMPal-issue-tracker) | **Leichtgewichtige VM-App für Apple Silicon & KI-Agenten**: Sichere, isolierte Sandboxes für Coding-Agenten auf macOS. | `IMG_7170` |
| **AG-UI Protocol** | [ag-ui.org](https://ag-ui.org) | **Offener UI-Standard für Agent-Oberflächen**: Einheitliche Protokoll-Events (`RUN_STARTED`, `TOOL_CALL_START`, `TEXT_MESSAGE_CONTENT`, `RUN_FINISHED`) für beliebige Agenten und Frontends. | `IMG_7197` |
| **i-have-adhd** | [github.com/ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | **ADHD-freundlicher Output-Skill für Claude Code & Codex**: Zwingt den Agenten dazu, ausschweifende Erklärungen wegzulassen und sofort die prägnante, handlungsrelevante Antwort zu liefern. | `IMG_7114` |
| **Alexaiupdates 9-Skill Suite** | @alexaiupdates | **Prompt- & Workflow-Skills für Claude**: `/prompt-master` (Clean Spec), `/grill-me` (Fragen stellen bis Klarheit herrscht), `/how-to`, `/optimizer` (Opus-Polishing), `/fable`, `/personal-voice`, `/anti-ai` (KI-Phrasen entfernen), `/write-a-skill`, `/handoff`. | `IMG_7162` |

### 10.2 Frontend, UI-Komponenten & Anti-Slop Design

| Name | GitHub / URL | Funktion | Screenshot |
| :--- | :--- | :--- | :--- |
| **diagram-design** | [github.com/cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | **Redaktioneller Diagramm-Skill für Claude Code / Codex**: Erzeugt 42 Diagramm-Typen als sauberes, schattenfreies HTML + SVG. Kein generisches Mermaid-Layout, hohe visuelle Eleganz. | `IMG_7209` |
| **Hairline** | [github.com/lucasmarkes/hairline](https://github.com/lucasmarkes/hairline) · [hairline.lucasmarkes.com](https://hairline.lucasmarkes.com) | **Feine isometrische Linien-Figuren**: Reagiert interaktiv auf Mausbewegungen. Für React und reines DOM. Inklusive Claude-Skill `hairline-create`. | `IMG_7206` |
| **genart-skill** | [github.com/camilleroux/genart-skill](https://github.com/camilleroux/genart-skill) | **Generative Art Skill für Claude Code**: Bringt Agenten Best Practices für Three.js, WebGL, p5.js, Hash-Seeding und deterministische Grafikgenerierung bei. MIT. | `IMG_7167` |
| **Anime.js (v4)** | [github.com/juliangarnier/anime](https://github.com/juliangarnier/anime) · [animejs.com](https://animejs.com) | **Modernes Web-Animationsframework**: Performante Keyframe-, SVG- und Morphing-Engine mit 73.4k Stars. | `IMG_7145` |
| **Lucide Icons** | [github.com/lucide-icons/lucide](https://github.com/lucide-icons/lucide) · [lucide.dev](https://lucide.dev) | **Community-Standard Icon-Bibliothek**: Über 1.000 konsistente Icons mit Figma-Plugin und nativer Integration für alle JS-Frameworks. | `IMG_7193` |
| **Jiro.build** | [jiro.build](https://jiro.build) | 1.200+ kuratierte UI-Design-Prompts für Webseiten und Dashboards. | `IMG_7126` |
| **Navbar Gallery** | [navbar.gallery](https://navbar.gallery) | Spezialisierte Referenzsammlung für moderne, interaktive Navigationsleisten. | `IMG_7126` |
| **Footer Design** | [footer.design](https://footer.design) | Inspirationsquelle für kreative und funktionale Footer-Layouts. | `IMG_7126` |
| **CTA Gallery** | [cta.gallery](https://cta.gallery) | Kuratierte Calls-to-Action mit Fokus auf Conversion und Typografie. | `IMG_7126` |
| **Kojima Generator** | [kojima-san.vercel.app](https://kojima-san.vercel.app) | Retro-Futuristische UI- & Sci-Fi-HUD-Komponenten vom Macher von HeroKit. | `IMG_7200` |
| **Liquid Glass / Liquid Logo** | Demo-Referenzen | Shader-gestützte interaktive Flüssigglas- und Logo-Verzerrungseffekte für moderne Landing Pages. | `IMG_7186`, `IMG_7187` |

### 10.3 Video, Generative Media & Creative EventTech

| Name | GitHub / URL | Funktion | Screenshot |
| :--- | :--- | :--- | :--- |
| **Hyperframes (HeyGen)** | [github.com/heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | **"Write HTML. Render video. Built for agents."**: Offizielles HeyGen-Framework zur programmatischen Generierung von Videos via TypeScript & WebGL. Keine Cloud-Farmen nötig; perfekte Basis für Video-Agenten. 55k Stars. | `IMG_7118`, `IMG_7119` |
| **twozero (TouchDesigner MCP)** | [github.com/404dotzero/twozero-td-mcp](https://github.com/404dotzero/twozero-td-mcp) · [twozero.ai](https://twozero.ai) | **"Vibe noding for TouchDesigner"**: Von @404.zero × @setupdesigns. Generiert TouchDesigner-Netzwerke via Claude Code & MCP direkt per Chat. Native Echtzeit-Visuals und Lichtshow-Steuerung. | `IMG_7158` |
| **EffectCraft** | [github.com/storytold/effectcraft](https://github.com/storytold/effectcraft) | **Open-Source After Effects Reimplementation**: Clean-Room Neubau von Adobe After Effects für Motion Graphics, Compositing und VFX. | `IMG_7149` |
| **Awesome Seedance** | [github.com/LearnPrompt/awesome-seedance](https://github.com/LearnPrompt/awesome-seedance) | **Evidenzbasierte Prompt-Bibliothek für Seedance 2.5 / 2.0**: 600+ überprüfte Prompts, 260+ Cross-Model-Runs, 25 Templates und 50 installierbare Video-Skills. | `IMG_7225` |
| **Recordly** | [github.com/webadderallorg/Recordly](https://github.com/webadderallorg/Recordly) · [recordly.dev](https://recordly.dev) | **Open-Source Desktop Screen Recorder**: Erstellt ohne Videoschnitt-Kenntnisse professionelle Produkt-Demos mit Cursor-Zoom, Auto-Framing und Studio-Export. 31.8k Stars. | `IMG_7201` |
| **image-blaster** | [github.com/neilsonnn/image-blaster](https://github.com/neilsonnn/image-blaster) | **Single-Photo-to-3D Skill für Claude**: Erzeugt aus einem 2D-Bild ein 3D-Asset/Mesh im Terminal. | `IMG_7221` |
| **Swishy** | [swishy.ai](https://swishy.ai) | AI-gestützter Motion Designer zur schnellen Erstellung von Web- und Social-Media-Animationen. | `IMG_7144` |
| **Reel Automation Suite** | Multi-Skill Setup | Trio aus `/reel-analyzer` (Hook-, Struktur- und Pacing-Analyse), `/reel-builder` (Skript, Voiceover, Untertitel & Musik) und `/content-factory` (End-to-End Automatisierung). | `IMG_7169`, `IMG_7196` |
| **TikTok 5.6B Dataset** | [huggingface.co/datasets/datasocial/tiktok-5.6B-videos](https://huggingface.co/datasets/datasocial/tiktok-5.6B-videos) | Riesiger Trainings- und Analyse-Datensatz für virale Videoformate, Hooks und Metadaten. | `IMG_7195` |

### 10.4 Architektur-Blueprints, Prompts & Best Practices

#### 1. Anthropic Swarm Architecture: Opus Advisor + Sonnet Builder + Haiku Swarm (`IMG_7229`, `IMG_7230`, `IMG_7233`)
* **Befehl:** `claude --advisor opus --subagents haiku`
* **Arbeitsteilung:**
  * **Opus 5.5 (`/advisor`):** Fungiert als Systemarchitekt auf Abruf. Liest Dokumentation, plant Module und trifft Richtungsentscheidungen, schreibt aber selbst keinen Code — hält seinen Kontext schlank und sauber.
  * **Sonnet 5.5:** Treibt die primäre Coding-Session mit tiefem Fokus auf Architektur und Implementierung voran.
  * **Haiku 5.5:** Schwärmt parallel im Hintergrund mit 340 Tok/s für Tests, Lints, Dateisuchen und Chores aus.
* **Ergebnis:** Bis zu **80% Einsparung** bei API-Kosten und Kontext-Verbrauch.

#### 2. Boris Cherny's Core Guardrails für Claude Code (`IMG_7232`)
* **Regel 1 — Der persistente Feedback-Loop:** *"Update your CLAUDE.md so you don't make that mistake again."* Jede Korrektur muss sofort in die permanenten Agentenregeln einfließen.
* **Regel 6b — Der Eleganz-Pass:** *"Knowing everything you know now, scrap this and implement the elegant solution."* Nach einem funktionierenden Prototyp den Code nicht weiter verkomplizieren, sondern mit dem neu gewonnenen Verständnis sauber neu aufsetzen.

#### 3. Meaghan Choi's Explainer Motion Studio Prompt (`IMG_7222`)
* Erzeugt aus einem Thema eine vollständige animierte Videoerklärung.
* Rendert über Headless Chrome mit 60 fps direkt in eine FFmpeg-Pipe (`libx264`), inklusive Captions, Audiomischung und Quellcode-Export.

#### 4. Hub & Spoke Memory Architecture (`IMG_7171`)
* Dokumentation darf den Kontext nicht fluten.
* **Hub:** `SSOT.md` als schlanker Single Source of Truth mit Kern-Architekturregeln.
* **Spokes:** Modulare `feature_*.md` Dateien, die nur bei Bedarf von Agenten punktuell referenziert werden.

#### 5. Physisches Design-System-Prinzip (`IMG_7172`)
* *"One light source from above. Everything is either raised (cards, keys) or pressed in (fields, tracks, trays). Nothing is flat and nothing floats without a surface under it."* Verleiht Web-UIs greifbare Haptik und Tiefe.

### 10.5 Saasengine, Datenbanken, Desktop & Cloud-Tools

| Name | GitHub / URL | Funktion & Relevanz für Saasengine | Screenshot |
| :--- | :--- | :--- | :--- |
| **DBX** | [github.com/t8y2/dbx](https://github.com/t8y2/dbx) | **Universeller 25-MB Datenbank-Client**: Unterstützt 100+ Datenbanken (MySQL, Postgres, SQLite, Redis, Mongo, DuckDB) in einer übersichtlichen Oberfläche. Mit integriertem MCP-Server, CLI und AI-Assistent. | `IMG_7214` |
| **OpenSEO** | [openseo.so](https://openseo.so) · [github.com/TahaHachana/OpenSEO](https://github.com/TahaHachana/OpenSEO) | **Open-Source SEO Alternative zu Semrush & Ahrefs**: Keyword-Research, Backlink-Audits und offizieller Google Search Console (GSC) MCP Server. | `IMG_7121`, `IMG_7178` |
| **Refine** | [github.com/refinedev/refine](https://github.com/refinedev/refine) · [refine.dev](https://refine.dev) | **React-Framework für Enterprise CRUD & Dashboards**: Die Brücke zwischen Low-Code und Custom Code für interne Tools und B2B-Apps mit dediziertem AI Agent. | `IMG_7185` |
| **Kestra** | [github.com/kestra-io/kestra](https://github.com/kestra-io/kestra) · [kestra.io](https://kestra.io) | **Deklarative Event-Driven Orchestrierung**: Alternative zu Airflow für daten- und codegetriebene Workflows via YAML. 26k Stars. | `IMG_7127` |
| **MiniCPM (OpenBMB)** | [github.com/OpenBMB/MiniCPM](https://github.com/OpenBMB/MiniCPM) | **SOTA On-Device Multimodal LLMs**: Extrem effiziente Bild- und Sprachverarbeitung direkt auf Endgeräten und Edge-Servern. 17.5k Stars. | `IMG_7128` |
| **GithubSignals** | [github.com/giovancarl444/githubsignals](https://github.com/giovancarl444/githubsignals) · [githubsignals.com](https://githubsignals.com) | Modulares Release- und Aktivitäts-Monitoring für Open-Source-Repositories. | `IMG_7226` |
| **AnyPS5** | [github.com/boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) | Automatisches Porting- und Relinking-Tool für Executables auf Linux und Windows. | `IMG_7198`, `IMG_7199` |
| **Muro** | [github.com/MrRockySL/Muro](https://github.com/MrRockySL/Muro) | Schlanke, native Live-Wallpaper-Engine für macOS 14+ mit minimalem RAM- und CPU-Verbrauch. | `IMG_7150` |
| **Offizielle Cloud MCP Server** | Provider-Verzeichnis | Vercel (`vercel/next-devtools-mcp`), Cloudflare (`cloudflare/mcp-server-cloudflare`), GCP (`GoogleCloudPlatform/cloud-run-mcp`), Tencent Cloud & Hostinger. | `IMG_7147` |
| **System Design Primer** | [github.com/donnemartin/system-design-primer](https://github.com/donnemartin/system-design-primer) | Der Standard-Leitfaden für skalierbare Systemarchitektur (DNS, Load Balancer, Caching, Sharding). | `IMG_7223` |

### 10.6 Duplikat-Log & Interne Notizen

| Screenshot | Fund | Status |
| :--- | :--- | :--- |
| `IMG_7120` | **OpenCut** ([github.com/OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut)) | ⚠️ Bereits in Kategorie 3 (Zeile 83) und Kat. 8 vorhanden. |
| `IMG_7184` | **Impeccable** ([github.com/pbakaus/impeccable](https://github.com/pbakaus/impeccable)) | ⚠️ Bereits in Kategorie 2 (Zeile 54) vorhanden. |
| `IMG_7125` | **Inertia** ([github.com/nettanvirdev/inertia](https://github.com/nettanvirdev/inertia)) | 🔁 War in Kat. 9.2 vermerkt ("README prüfen") — durch Screenshot & GitHub-Star nun vollständig beschrieben. |
| `IMG_7159.jpg` | **AOS - BDB Agent OS** (v4.19.0) | 🏢 Interner Projekt-Snapshot: Tim's Agent-OS npm-Paket mit 264 Skills und 21 Subagenten. |
| `IMG_7215` / `IMG_7216` | **bdb-wave** (`hybridlabor-api/bdb-wave`) | 🏢 Interner Pull Request: Integration des AOS-Panels in bdb-wave. |
| `IMG_7218` | **Claude Code Session History** | 🏢 Interne Sessions: Coucou AOS, bdb wave, MASTER SESSION BDB. |
| `96218f76…JPG` / `f4947ff7…JPG` | **Chitubox Pro** | 🖨️ 3D-Druck Slicer Extraktions-Log — kein Repo. |

---

## Kategorie 11: Frisch "Starred" auf GitHub (Oktober 2026)
*Alle neu mit einem Stern markierten Repositories aus Tim's persönlichem GitHub-Profil (`github.com/stars`), die noch nicht in den vorherigen Abschnitten erfasst wurden.*

| Name | GitHub / URL | Funktion & Relevanz |
| :--- | :--- | :--- |
| **hark-pool** | [github.com/0xgetz/hark-pool](https://github.com/0xgetz/hark-pool) | **Headless Account Pooling & OpenAI Proxy**: Erstellt Hark-Accounts automatisiert und bündelt den gesamten Pool als einzelnen OpenAI-kompatiblen Provider für 9Router. Zero Dependencies, Round-Robin Session-Adapter. |
| **bug-bounty-hunting-prompts** | [github.com/mdpsec/bug-bounty-hunting-prompts](https://github.com/mdpsec/bug-bounty-hunting-prompts) | **Strukturierte Bug-Bounty-Prompts**: Verwandelt chaotisches Ausprobieren in einen evidenzbasierten Sicherheits-Workflow für LLMs und Security-Agenten. |
| **hallmark** | [github.com/Nutlope/hallmark](https://github.com/Nutlope/hallmark) | **Anti-AI-Slop Design Skill für Claude Code, Cursor & Codex**: Von Hassan El Mghari. Schützt davor, dass Coding-Agenten generische, langweilige Standard-Komponenten generieren. |
| **openvid** | [github.com/CristianOlivera1/openvid](https://github.com/CristianOlivera1/openvid) | **Browserbasierter Video- & 3D-Mockup-Creator**: Erstellt professionelle Produkt-Demos und interaktive 3D-Showcases in Sekunden direkt im Web. |
| **dagu** | [github.com/dagucloud/dagu](https://github.com/dagucloud/dagu) | **Leichtgewichtiger Single-Binary Workflow Orchestrator**: Führt deklarative YAML-Pipelines über bestehende Skripte, SSH-Befehle und Docker-Container aus. Keine Datenbank nötig, ideale Alternative zu Airflow und Cron für Saasengine-Flotten. |
| **Open-Higgsfield-AI** | [github.com/Autom8AI/Open-Higgsfield-AI](https://github.com/Autom8AI/Open-Higgsfield-AI) | **Open-Source Alternative zu Higgsfield AI**: Kostenloses Bild- und Video-Generierungsstudio mit 20+ Modellen (Flux, SDXL, Midjourney, Ideogram). Self-hosted & anpassbar. |
| **muapi-cli** | [github.com/SamurAIGPT/muapi-cli](https://github.com/SamurAIGPT/muapi-cli) | **Offizielles CLI & MCP Server für muapi.ai**: Generiert Bilder, Videos und Audio direkt aus dem Terminal oder aus Coding-Agenten heraus (14 KI-Modelle). |
| **open-agent-connector** | [github.com/Anil-matcha/open-agent-connector](https://github.com/Anil-matcha/open-agent-connector) | **Open-Source Alternative zu Composio & Nango**: Self-hosted Integrationen für GitHub, Slack, Hacker News und HTTP-Actions via MCP oder REST. |
| **ai-clipping-generator** | [github.com/SamurAIGPT/ai-clipping-generator](https://github.com/SamurAIGPT/ai-clipping-generator) | **AI Video Clipping SaaS-Starter**: Extrahiert virale Shorts, Reels und TikToks automatisch aus YouTube-Videos (Next.js, Stripe, Prisma). |
| **open-dots** | [github.com/Anil-matcha/open-dots](https://github.com/Anil-matcha/open-dots) | **Self-Hosted AI Agent Workspace**: Open-Source Alternative zu OpenAI Dots, Manus Cue und Claude Cowork mit Chat, Tool-Connectors und Computer Use. |
| **muapi-comfyui** | [github.com/SamurAIGPT/muapi-comfyui](https://github.com/SamurAIGPT/muapi-comfyui) | **ComfyUI Custom Nodes für 600+ Modelle**: Zugriff auf Seedance, Kling, Veo3, Flux, HiDream und Imagen4 über muapi.ai. |
| **ax (Google)** | [github.com/google/ax](https://github.com/google/ax) | **Google's Open Agentic Orchestration Runtime**: Offenes Framework von Google zur Multi-Agenten-Orchestrierung. |
| **playbooks** | [github.com/playbooks-ai/playbooks](https://github.com/playbooks-ai/playbooks) | **Semantisches Programmiersystem für KI-Agenten**: Standardisierte, ausführbare Playbooks zur Steuerung komplexer Agenten-Zyklen. |
| **autoshorts** | [JayWebtech/autoshorts](https://github.com/JayWebtech/autoshorts) | **Local-First Desktop App für 9:16 Videoclips**: Erkennt Highlights in Langformat-Videos per KI und schneidet vertikale Snippets mit viralem Ranking. |
| **brag** | [github.com/latent-spaces/brag](https://github.com/latent-spaces/brag) | **"You built it. Now brag."**: Verwandelt ein fertiges Softwareprojekt mit einem einzigen Terminalbefehl in ein knackiges Launch-Video. |
| **DeskcommCRM** | [github.com/melgarafael/DeskcommCRM](https://github.com/melgarafael/DeskcommCRM) | **Open-Source AI Sales OS mit WhatsApp (WAHA)**: Self-hosted CRM mit nativen KI-Agenten für Conversational Sales. MCP-ready, Multi-Tenant. |
| **Decepticon** | [github.com/BitterSecurity/Decepticon](https://github.com/BitterSecurity/Decepticon) | **Autonomer Hacking-Agent für Red Teams**: Vollautomatisierte Penetrationstests und Schwachstellensuche. |

---

## Kategorie 12: Motion-Design-Prüfung für AOS-Kernel & Creator Extension — 10. Okt 2026
*Ziel: Update für Videoerstellung, Skripting, Social Media und Motion Design. Alle Angaben stammen aus den READMEs (gelesen von Haiku-/Sonnet-Workern am 10. Okt), nichts davon wurde installiert oder ausgeführt. Vorhanden im AOS: `remotion`, `godmode-media-creation`, `threejs-skills`, `spline-3d-integration`, `brag`, `video-motion-assistant`; Creator Extension: OpenMontage, Video-Shotcraft, Palmier-Pro, TRELLIS, `comfyui-mcp`.*

### 12.1 Code → Video (Renderer)

| Name | GitHub | Methode | Lizenz | Lokal | Agent-fähig | Einordnung gegenüber Remotion |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Hyperframes (HeyGen)** | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | HTML+CSS → headless Chrome Frame-Capture → FFmpeg, deterministisch, mit Audio-Mixing (`npx hyperframes init`; Node 22+) | Apache-2.0 | ja | agent-first, Einbindung über Vercel Skills | **ergänzt** — gleiche Idee, anderer Ansatz; `brag` baut bereits darauf |
| **brag** | [latent-spaces/brag](https://github.com/latent-spaces/brag) | Claude-Skill, delegiert an Hyperframes; `/brag-slim` ohne Hyperframes (`npx skills add …`) | MIT | ja | Skill | **ergänzt** — im AOS schon als Skill vorhanden |
| **onetake** | [feitangyuan/onetake](https://github.com/feitangyuan/onetake) | Beat-getriebene HTML-Komposition mit Motion-Blur, Python-"Continuity-Oracle" | ⚠️ PolyForm Noncommercial | ja | Skill | **ergänzt** — **nicht für bezahlte Projekte** ohne Kauflizenz |
| **EffectCraft** | [storytold/effectcraft](https://github.com/storytold/effectcraft) | After-Effects-Nachbau, Rust-Encoder (H.264, ProRes, AV1…), kein FFmpeg nötig | MIT oder Apache-2.0 | ja | nein (GUI-Editor) | **Alternative zu After Effects**, kein Remotion-Ersatz; Agent-Anbindung müsste gebaut werden |
| **openvid** | [CristianOlivera1/openvid](https://github.com/CristianOlivera1/openvid) | Browser: FFmpeg.wasm + Three.js, Produkt-Demos und Mockups | ⚠️ nicht angegeben | teilweise (Supabase-Backup geplant) | nein | **ergänzt** — UI-Tool, nicht programmierbar |
| **fframes** | fframes-studio/fframes | — | — | — | — | ❌ **404** — Repo nicht auffindbar, Eintrag in Kat. 3 prüfen |

### 12.2 Three.js / WebGL / WebGPU / generativ

| Name | GitHub | Funktion | Lizenz | Agent-fähig | Einordnung |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **genart-skill** | [camilleroux/genart-skill](https://github.com/camilleroux/genart-skill) | Deterministisches Rendering, Hash-Seeding; Canvas 2D, p5.js, three.js/WebGL, SVG; erzeugt PNG-Frames, Contact-Sheets, Batch-Export (`/plugin install genart@camilleroux-genart`) | MIT | Claude-Plugin | Ergänzt `threejs-skills` um reproduzierbare Frames; kein Video-Encoding |
| **VGPU (Vercel Labs)** | [vercel-labs/vgpu](https://github.com/vercel-labs/vgpu) | Typisierte WebGPU-Shader-Bibliothek, headless in Node (Dawn), `frameLoop()` liefert Frame-Daten | MIT | laut Worker kein MCP | Low-Level-Baustein; Encoding wäre separat nötig |
| **twozero (TouchDesigner MCP)** | [404dotzero/twozero-td-mcp](https://github.com/404dotzero/twozero-td-mcp) | `.tox` in TouchDesigner 2025.32280+, MCP auf Port 40404 | ⚠️ nicht angegeben | MCP | Steuerung, kein Renderer; ergänzt die vorhandenen TD-MCPs |

### 12.3 KI-Video & Prompts

| Name | GitHub | Funktion | Lizenz | Lokal | Hinweis |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Pixelle-Video** | [AIDC-AI/Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video) | Thema → Skript → Bilder → Voiceover → Musik → Video (ComfyUI, ffmpeg, LLM-APIs; `uv run streamlit run web/app.py`) | Apache-2.0 | teilweise (LLM-/Bild-APIs nötig, ComfyUI optional lokal) | Nähe zur Creator Extension (`comfyui-mcp`) |
| **Awesome Seedance** | [LearnPrompt/awesome-seedance](https://github.com/LearnPrompt/awesome-seedance) | Laut README 815 Prompts, 27 Templates, 77 installierbare Skills für Seedance | Code MIT, Inhalt CC BY 4.0 | nein (Seedance-Cloud) | nur Prompt-Material, keine Engine |

### 12.4 Social Media, Skripting & Schnitt (Reel Automation Suite aufgelöst)

| Name | GitHub | Funktion | Lizenz | Lokal | Hinweis |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **claude-content-skills** | [Ootto-AI/claude-content-skills](https://github.com/Ootto-AI/claude-content-skills) | **Quelle der "Reel Automation Suite"**: 30+ Klartext-Skills; `reel-analyzer` (Frames+Transkript → Hook, Beats, Pacing), `reel-builder`, `content-factory`. 127 Sterne. Der Name "Reel Automation Suite" steht nicht im Repo. | MIT | ja (Prompts, Obsidian-Vault lokal) | Autopilot-Upsell ist kostenpflichtig, nicht nötig; Analyzer hängt an Claudes Frame-/Transkript-Analyse |
| **programmatic-reel** | [gurungabit/programmatic-reel](https://github.com/gurungabit/programmatic-reel) | Skript, Voiceover (Kokoro TTS), Musik, Rendering über Remotion | ⚠️ nicht angegeben (Remotion-Company-Lizenz beachten) | ja | 0 Sterne, ungeprüft; passt direkt zu `remotion` |
| **claude-reels** | [iamachilles/claude-reels](https://github.com/iamachilles/claude-reels) | Schnitt und Untertitel (ffmpeg, HyperFrames, mlx-whisper) | MIT | ja, nur Apple Silicon | 0 Sterne, ungeprüft |
| **autoshorts** | [JayWebtech/autoshorts](https://github.com/JayWebtech/autoshorts) | Desktop-App: 9:16-Clips aus Langvideos, Highlight-Ranking, Captions per FFmpeg | ⚠️ nicht angegeben | teilweise — **Deepgram-API (Cloud) nötig** | kein Offline-Fallback |
| **claude-video** | siehe Kat. 9.1 | `/watch`: Download, Frames, WhisperX lokal | MIT | ja | Analyse-Baustein |

### 12.5 Einschätzung für das Update (Empfehlung, keine Entscheidung)
* **Übernehmen/prüfen zuerst:** Hyperframes (schon über `brag` im Spiel — als zweiter Renderer neben Remotion dokumentieren), claude-content-skills (Skripting + Social, MIT), genart-skill (Three.js-Frames).
* **Als Vergleich nutzen:** programmatic-reel und claude-reels (kleine lokale Reel-Pipelines).
* **Mit Vorbehalt:** onetake (Lizenz), autoshorts (Cloud), openvid (Lizenz unklar).
* **Offen:** fframes (404), keine lokale Alternative zum `reel-analyzer`; claude-video könnte diese Lücke füllen.


---

## Kategorie 13: Neuzugänge aus Downloads (`Neuer Ordner mit Objekten 2/`) — 10. Okt 2026

*Auswertung der Screenshots `IMG_7234` bis `IMG_7245` und Neufunde für AOS v5, den AOS Store & Saasengine.*

| Name | GitHub / URL | Funktion & Relevanz für AOS | Screenshot-Quelle |
| :--- | :--- | :--- | :--- |
| **Rust Skills** | [github.com/actionbook/rust-skills](https://github.com/actionbook/rust-skills) | **AI-Powered Rust Development & Meta-Cognition Framework**: Claude Code Plugin & Skill-Suite (Ownership, Borrowing, Lifetimes, Concurrency, Unsafe-Checker, Dynamic Skills aus `Cargo.toml`). Schließt die klaffende Rust-Lücke in AOS und ist das Fundament für den Tauri v2 Rust-Core in Orchestrator 2.0. | Neuzugang / Empfehlung |
| **Claude Code Templates** | [github.com/davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | **Interactive Web Interface & 100+ Production-Ready Templates**: Multi-Agent Collaboration, Live-Visualisierung des Reasonings. Dient als direkter Blueprint zur Modernisierung der `aos store ui` (Port 4322) und des Launchpads (Port 7900) mit One-Click-Testlauf. | `IMG_7236.PNG` |
| **AI Employees** | [github.com/markfulton/ai-employees](https://github.com/markfulton/ai-employees) | **8 Open Source AI Employees & 60 Scheduled Routines**: Deckt die Domänen GTM, SEO, WebDev, Social, Ads, Sales, Support und Chief of Staff ab. Füllt die bisher schwächste Domäne in AOS (`saas-ops` / Business-Workflows) mit schlüsselfertigen Routinen, abgesichert über das AOS GO-Gate. | `IMG_7234.PNG` |
| **Motionmaxxing (FinalMotion)** | [github.com/Tejashmakwana/motionmaxxing](https://github.com/Tejashmakwana/motionmaxxing) · `@makwanatejas170` | **Looksmaxxing for Motion Graphics**: Verwandelt AI-Video-Slop in professionelles Motion-Design. 53 vermessene Momente, 12 Easing-Kurven, 150 Regeln, G0–G5 Mog-Checks via ffmpeg. Perfekter Qualitäts-Linter für den `video-motion-assistant` und die Creator Extension. | `IMG_7242.PNG` |
| **AWS Strands-Box** | [github.com/strands-agents/box](https://github.com/strands-agents/box) | **OS-Level Sandboxing für autonome Agenten**: Dogwood Policy Language (zeitliche & bedingte Regeln), External Secret Injection. Behebt das in AOS anerkannte Residual-Sicherheitsdefizit (H2: "Gate is not a sandbox") für ungetestete Agentenbefehle. | `IMG_7243.PNG` |
| **AGENTS.md Specification** | [github.com/agentsmd/agents.md](https://github.com/agentsmd/agents.md) | **Offener Standard für Coding-Agent-Instruktionen**: Standardisiertes Format für Copilot, Gemini CLI, Cursor, Claude Code. Dient als Referenz-Linter für `npm run validate` im AOS-Ökosystem. | `IMG_7241.PNG` |
| **Karakeep (ehem. Hoarder)** | [github.com/karakeep-app/karakeep](https://github.com/karakeep-app/karakeep) (`MohamedBassem`) | **Self-Hostable Bookmark-Everything App**: Automatische KI-Verschlagwortung, Volltextsuche, lokale Bild-/Link-Archivierung (auch mit Ollama). Bildet die visuelle Brücke zwischen Web-Recherche (`bdbrainstorm`) und memB Vektor-Gedächtnis. | `IMG_7238.PNG` |
| **Cutter** | [github.com/rizinorg/cutter](https://github.com/rizinorg/cutter) · [cutter.re](https://cutter.re) | **Free & Open-Source Reverse Engineering Platform**: Powered by Rizin / Radare2 mit Ghidra Decompiler. Erweitert das Security-Review-Portfolio (`security-reviewer`) um tiefe Binäranalyse und Disassembly. | `IMG_7244.PNG` |
| **Paperless-ngx** | [github.com/paperless-ngx/paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) | **Supercharged Document Management System**: Scannt, archiviert, taggt und durchsucht Rechnungen, Verträge und Belege automatisch per OCR. Relevante Backend-Infrastruktur für Agentur-Playbooks (`pb-invoice-check`). | `IMG_7237.PNG` |
| **Syncthing** | [github.com/syncthing/syncthing](https://github.com/syncthing/syncthing) | **Dezentraler Cross-Device Datei-Sync**: Peer-to-Peer, Ende-zu-Ende verschlüsselt ohne Cloud. Nützlich zur nahtlosen Replikation von `~/.aos/` Konfigurationen, Worktrees und memB Embeddings zwischen MacBook und stationärem GPU-Rig. | `IMG_7239.PNG` |
| **Send** | [github.com/timvisee/send](https://github.com/timvisee/send) (Community Fork von Firefox Send) | **Verschlüsselter Dateiversand mit automatischer Löschung**: Sicheres, flüchtiges Bereitstellen von Produktionsartefakten aus `production_artifacts/` an externe Partner mit Ablauf-Timer. | `IMG_7240.PNG` |
| **Officeverse** | [officeverse.id](https://officeverse.id) | Framework zur programmatischen Generierung von Office-Dokumenten (Word, PPT, Excel) für automatisierte Reportings und Präsentationen. | `IMG_7245.PNG` |
