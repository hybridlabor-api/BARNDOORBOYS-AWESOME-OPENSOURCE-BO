# 🌟 BARNDOORBOYS Awesome Open Source & Agent Stack

> **Kuratierte, typisierte Wissens- & Tool-Sammlung für das BDB-Ökosystem**  
> *Fokus: Agent Operating System (AOS), Multi-Agent Swarms, Computer-Use, Creative Media & SaasEngine.*

[![Awesome](https://awesome.re/badge.svg)](https://github.com/sindresorhus/awesome)
[![Tools](https://img.shields.io/badge/Tools-256%20Kuriert-blue.svg)](#-inhaltsverzeichnis-nach-domänen)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![AOS](https://img.shields.io/badge/Ecosystem-BDB%20AOS%20v5-purple.svg)](https://github.com/barndoorboys)

---

## 🧭 Schnellfilter nach Typ

| Typ-Badge | Formfaktor & Nutzen | Anwendungsfokus |
| :--- | :--- | :--- |
| **`🧩 Skill`** | **Agent Skills & Prompts** | Direkt installierbar via `npx skills add`, MCP-Tools oder System-Prompts für Claude, Codex, OpenCode & Antigravity. |
| **`🎨 Design Lib`** | **UI- & Frontend-Libraries** | Web-Komponenten, Icon-Sets, CSS/Tailwind-Tokens, SVG-, Canvas- und WebGL-Visualisierungen. |
| **`🖥️ OSS App`** | **Desktop-Apps, TUIs & Tools** | Native macOS/Linux-Apps, TUIs, CLI-Utilities, Terminal-Emulatoren und lokale Sicherheits-Scanner. |
| **`☁️ Cloud / SaaS`** | **Cloud- & Self-Hosted Services** | Serverless Backends, DBs (Neon/Supabase), Headless CMS, Newsletter-Engines und Hosting-Infrastruktur. |
| **`⚙️ Framework`** | **Frameworks, Runtimes & Swarms** | Multi-Agenten-Orchestrierung, Test-Automatisierung (e2e), Kommunikationsprotokolle und Agent-Harnesses. |
| **`📐 Pattern`** | **Architektur & Leitplanken** | Senior-Workflow-Heuristiken (Boris Cherny), Multi-Agent-Review-Loops, System-Design-Guides und Spezifikationen. |
| **`🎨 Media Tech`** | **Creative Media & Motion** | Remotion-Pipelines, AI-Videogenerierung, 3D-Math-Animation (ManimGx) und Show-Control-Engines. |
| **`🖥️ Computer-Use`**| **OS- & Desktop-Steuerung** | Latenzarmes Window-Mirroring (Sill), entkoppelte Maus-/Keyboard-Agents (LCU) und Hardware-Bridges. |
| **`🛡️ Security`** | **Security & Hygiene** | AI-native SOAR (Tracecat), Local AppSec-Scanner (Zerra), AI-Wasserzeichen-Entferner & Pentesting. |
| **`🔍 Reverse Eng.`** | **Binär- & Code-Analyse** | NSA Ghidra Decompiler, Cutter und Disassembly-Pipelines. |

---

## 📑 Inhaltsverzeichnis nach Domänen

1. [1. AI Coding Harnesses, Workspaces & Agent Supervisions (AOS Core)](#1-ai-coding-harnesses-workspaces--agent-supervisions-aos-core)
2. [2. Multi-Agent Orchestration, Swarms & Protocols](#2-multi-agent-orchestration-swarms--protocols)
3. [3. Computer-Use, OS Sandboxing & Remote Desktops](#3-computer-use-os-sandboxing--remote-desktops)
4. [4. Context, Memory, AST Code-Graphs & Knowledge](#4-context-memory-ast-code-graphs--knowledge)
5. [5. Security, Pentesting, CI/CD & Verification Gates](#5-security-pentesting-cicd--verification-gates)
6. [6. Frontend, UI-Komponenten & Design Systems (Godmode UI/UX)](#6-frontend-ui-komponenten--design-systems-godmode-uiux)
7. [7. Video Generation, Creative Media Tech & Remotion (Godmode Media)](#7-video-generation-creative-media-tech--remotion-godmode-media)
8. [8. Hardware, Robotics & PCB Engineering](#8-hardware-robotics--pcb-engineering)
9. [9. Cloud Infrastructure, Flotten-Management & SaasEngine](#9-cloud-infrastructure-flotten-management--saasengine)
10. [10. Web Scraping, Lead Generation & Extraction Tools](#10-web-scraping-lead-generation--extraction-tools)
11. [11. Reverse Engineering & Binary Analysis](#11-reverse-engineering--binary-analysis)

---

## 1. AI Coding Harnesses, Workspaces & Agent Supervisions (AOS Core)

*Anzahl kuratierter Tools: 79*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**Agent HUD Open**](https://github.com/jazzenchen/agent-hud-open) | `🖥️ macOS App` | Swift macOS Notch-HUD für Coding-Agenten: Zeigt Token-Verbrauch, API-Kosten und Session-Status direkt in der MacBook-Notch an. |
| [**Agentic Inbox**](https://github.com/cloudflare/agentic-inbox) | `☁️ Cloud / SaaS` | Serverless AI Email Client auf Cloudflare: Vollständiger Mail-Client, der autonom E-Mails liest, kategorisiert und beantwortet. Läuft serverless auf Cloudflare Workers/Agents. |
| [**AGENTS.md Specification**](https://github.com/agentsmd/agents.md) | `📐 Pattern` | Offener Standard für Coding-Agent-Instruktionen: Standardisiertes Format für Copilot, Gemini CLI, Cursor, Claude Code. Dient als Referenz-Linter für `npm run validate` im AOS-Ökosystem. |
| **Alexaiupdates 9-Skill Suite** | `🧩 Skill` | @alexaiupdates &#124; Prompt- & Workflow-Skills für Claude: `/prompt-master` (Clean Spec), `/grill-me` (Fragen stellen bis Klarheit herrscht), `/how-to`, `/optimizer` (Opus-Polishing), `/fable`, `/personal-voice`, `/anti-ai` (KI-Phrasen entfernen), `/write-a-skill`, `/handoff`. &#124; `IMG_7162` |
| [**Anime.js (v4)**](https://github.com/juliangarnier/anime) | `🎨 Motion Lib` | Modernes Web-Animationsframework: Performante Keyframe-, SVG- und Morphing-Engine mit 73.4k Stars. |
| [**AnyPS5**](https://github.com/boykopovar/AnyPS5) | `🖥️ OSS App` | Automatisches Porting- und Relinking-Tool für Executables auf Linux und Windows. |
| [**AutoHarness**](https://github.com/tigerless-labs/autoharness) | `⚙️ Harness` | Self-Learning Skill Layer für Claude Code: Lernt automatisch neue Fähigkeiten direkt aus realen Arbeitssessions, führt Duplikate zusammen (`fold/reflector`) und bereinigt ungenutzte Skills selbstständig. |
| [**ax (Google)**](https://github.com/google/ax) | `⚙️ Framework` | Google's Open Agentic Orchestration Runtime: Offenes Framework von Google zur Multi-Agenten-Orchestrierung. |
| **BDB Agent OS (v4.19.0 Snapshot)** | `🏢 Intern` | 🏢 Interner Projekt-Snapshot: Tim's Agent OS Setup & Workspace-Struktur. |
| **BDB Wave (hybridlabor-api/bdb-wave)** | `🏢 Intern` | 🏢 Interner Pull Request: Audio-reaktive Waveform-Visualisierung für Creative Tech. |
| [**Blackbit.sh**](https://blackbit.sh) | `⚙️ Framework` | Multi-Model Orchestrierung: Optimiertes Setup, bei dem jedes Modell seine spezialisierte Rolle erhält (z.B. Opus plant jede Aufgabe und leitet an Ausführer weiter). |
| **Boris Cherny Workflow Heuristics** | `📐 Pattern` | Produktions-Leitplanken des Claude-Code-Schöpfers: Plan Mode Default (ab 3 Schritten Pflicht), Subagents Liberally (Hauptkontext sauber halten), Self-Improvement Loop (tasks/lessons.md nach User-Korrekturen), Verification Before Done, Demand Elegance, Autonomous Bug Fixing. |
| **Chitubox Pro** | `🖥️ 3D Software` | 🖨️ 3D-Druck Slicer & Vorbereitungs-Software für SLA/DLP-Harzdrucker. |
| **Claude Code Session History** | `🏢 Intern` | 🏢 Interne Session-Historie: Best-Practice Workflows für Coucou AOS, bdb wave und Multi-Agent Runs. |
| [**Claude Managed Agents**](https://x.com/ClaudeDevs) | `⚙️ Platform` | Dynamic Workflows Public Beta: Anthropics offizielle Ankündigung für dynamische Agenten-Workflows und verwaltete Multi-Agenten-Ausführung. |
| [**Claude-Code-Mods**](https://github.com/hamzafer/claude-code-mods) | `🧩 Plugin Hub` | Curated Plugins & Mods for Claude Code: Strukturierte Mod-Sammlung zur Erweiterung von Claude Code Fähigkeiten. |
| [**Composio**](https://github.com/ComposioHQ/composio) | `⚙️ Framework` | 100+ Enterprise Tool-Integrations für Agenten: Standardisierte Actions und MCP-Schnittstellen für Slack, Notion, GitHub, Salesforce, Gmail u.v.m. |
| [**Coucou (Mochi)**](https://github.com/Louis-CFM/coucou) | `🖥️ Mobile / iOS` | ⚠️ Doppelt — Repo steht bereits in Kategorie 1 (Coucou/Mochi). Neu: iPhone-App mit Face-ID-Approval, "Message your session" → VS Code, Widgets/Live Activity, private iCloud — Kurzbeschreibung in Kat. 1 ggf. erweitern. |
| [**Council of High Intelligence**](https://github.com/0xNyk/council-of-high-intelligence) | `🖥️ OSS App` | Multi-Perspektiven-Beratung für harte Entscheidungen: Lässt 18 historische und technische Denker (Socrates, Feynman, Munger, Lovelace, Rams, Musashi, Torvalds, Karpathy, Aurelius) gegeneinander debattieren, bevor Code geschrieben wird. Für Claude Code, Codex, Gemini CLI und OpenCode. |
| [**creative-director-skill**](https://github.com/smixs/creative-director-skill) | `🧩 Skill` | "World-class creative director in a skill": Ideation via SIT/TRIZ/Lateral Thinking + Cannes-Lions-Evaluations-Engine, kalibriert gegen 571 legendäre Kampagnen (Originalitäts-Cap gegen Pattern-Sättigung). ~235 Stars, CC-BY-4.0. |
| [**CTA Gallery**](https://cta.gallery) | `🎨 UI Gallery` | Kuratierte Calls-to-Action mit Fokus auf Conversion und Typografie. |
| [**dagu**](https://github.com/dagucloud/dagu) | `☁️ Cloud / SaaS` | Leichtgewichtiger Single-Binary Workflow Orchestrator: Führt deklarative YAML-Pipelines über bestehende Skripte, SSH-Befehle und Docker-Container aus. Keine Datenbank nötig, ideale Alternative zu Airflow und Cron für Saasengine-Flotten. |
| [**DBX**](https://github.com/t8y2/dbx) | `☁️ Cloud / SaaS` | Universeller 25-MB Datenbank-Client: Unterstützt 100+ Datenbanken (MySQL, Postgres, SQLite, Redis, Mongo, DuckDB) in einer übersichtlichen Oberfläche. Mit integriertem MCP-Server, CLI und AI-Assistent. |
| [**Decepticon**](https://github.com/BitterSecurity/Decepticon) | `🛡️ Security` | Autonomer Hacking-Agent für Red Teams: Vollautomatisierte Penetrationstests und Schwachstellensuche. |
| [**DeskcommCRM**](https://github.com/melgarafael/DeskcommCRM) | `☁️ Cloud / SaaS` | Open-Source AI Sales OS mit WhatsApp (WAHA): Self-hosted CRM mit nativen KI-Agenten für Conversational Sales. MCP-ready, Multi-Tenant. |
| [**Directus**](https://github.com/directus/directus) | `☁️ Cloud / SaaS` | Headless SQL-First Data Engine & CMS: Stülpt sofort REST- und GraphQL-APIs über bestehende SQL-Datenbanken (Postgres/MySQL) mit granularer Rechteverwaltung und Web-Studio. |
| [**everything-claude-marketing**](https://github.com/brainbytes-dev/everything-claude-marketing) | `🧩 Skill` | Komplettes Marketing-Intelligence-System für Claude Code: 18 Agents, 72 Skills, 22 Commands (Strategist, SEO, Paid Ads, Growth-Hacker, PR, CRO …). |
| [**Foreman (ThruWire)**](https://github.com/thruwire/foreman) | `⚙️ Framework` | Autonomer Supervisor für Coding-Agenten: Begleitet langsame Coding-Agenten (Claude, Cursor, Codex) mit schnellen, deterministischen System-1-Entscheidungen (via Jev-Modell). Erkennt Loops, Blockaden und prüft Arbeitsfortschritt. |
| [**Ghostty**](https://github.com/ghostty-org/ghostty) | `🖥️ OSS App` | Fast, native, feature-rich Terminal Emulator: GPU-beschleunigt mit modernem Tab/Window-Management und plattformübergreifender C/Zig-Bibliothek (`libghostty`) für native Coding- und Agent-Terminals. |
| [**GitBot**](https://github.com/gitbot-hq/GitBot) | `🖥️ OSS App` | "Give your coding agents a home": Lokaler Server (Port 3000), der Claude Code/Codex/OpenCode aus dem Browser fernsteuert — wiederverwendbare Bots, persistente Threads, per-Bot Permissions. npm `@gitbot-hq/gitbot`. Vergleichbar mit Coucou/GitHub-Remote-Steuerung. |
| [**GithubSignals**](https://github.com/giovancarl444/githubsignals) | `⚙️ Core Tool` | Modulares Release- und Aktivitäts-Monitoring für Open-Source-Repositories. |
| [**google-research/harness2**](https://github.com/google-research/harness2) | `⚙️ Harness` | Modulare 8-Komponenten Agent-Harness-Architektur von Google Research: Saubere Entkopplung von Modell-Inferenz, Tool-Execution, Memory und Verifikations-Loops. |
| [**Hairline**](https://github.com/lucasmarkes/hairline) | `🧩 Skill` | Feine isometrische Linien-Figuren: Reagiert interaktiv auf Mausbewegungen. Für React und reines DOM. Inklusive Claude-Skill `hairline-create`. |
| [**hark-pool**](https://github.com/0xgetz/hark-pool) | `☁️ Cloud / SaaS` | Headless Account Pooling & OpenAI Proxy: Erstellt Hark-Accounts automatisiert und bündelt den gesamten Pool als einzelnen OpenAI-kompatiblen Provider für 9Router. Zero Dependencies, Round-Robin Session-Adapter. |
| [**Herdr**](https://github.com/herdrdev/herdr) | `⚙️ Framework` | "The runtime your coding agents live on": Isolierte Ausführungsumgebung und lokales Sandboxing für Coding-Agenten. ~33k Stars, Apache-2.0. |
| [**Hermarchy (Omarchy-Theme)**](https://github.com/archer-clawbot/omarchy-hermarchy-theme) | `⚙️ Core Tool` | Research-Workstation-Theme für Omarchy mit optionalem Hermes-Agent-Status-Panel (Quickshell-Plugin). ~86 Stars. Interessant als Aesthetic-Referenz ("cyan is semantic, not decorative") für eigene Agent-UIs. |
| [**i-have-adhd**](https://github.com/ayghri/i-have-adhd) | `🧩 Skill` | ADHD-freundlicher Output-Skill für Claude Code & Codex: Zwingt den Agenten dazu, ausschweifende Erklärungen wegzulassen und sofort die prägnante, handlungsrelevante Antwort zu liefern. |
| [**image-blaster**](https://github.com/neilsonnn/image-blaster) | `🖥️ OSS App` | Single-Photo-to-3D Skill für Claude: Erzeugt aus einem 2D-Bild ein 3D-Asset/Mesh im Terminal. |
| [**Inertia (nettanvirdev)**](https://github.com/nettanvirdev/inertia) | `⚙️ Framework` | Modulares Inertia-Starter-Setup für moderne Fullstack-Architekturen. |
| [**inertia-ai 0.1.0**](https://github.com/nettanvirdev/inertia/releases/tag/v0.1.0) | `🖥️ Computer-Use` | Erstes Release von inertia-ai. README geprüft (MIT): Desktop-Workspace für lokale AI-Agenten (Tauri 2, React 19), nur Windows getestet; API-Keys liegen unverschlüsselt, die Shell läuft mit Nutzerrechten. |
| [**Jev Engineering Tree (@polydao)**](https://x.com/polydao) | `📐 Pattern` | Prompt-Methodik (kein Repo): Claude-Code-Agent-Tree mit Fable-Advisor (liest alles, schreibt nie), Jev-Fork-Layer (deterministische which-file/which-tool/retry-Entscheidungen < 0,5s statt Opus-Aufrufen), 3 Subagenten (medium effort), Review+Verify vor Ship. Passgenau zu unserer Harness-/Token-Einspar-Diskussion. |
| [**Kestra**](https://github.com/kestra-io/kestra) | `☁️ Cloud / SaaS` | Deklarative Event-Driven Orchestrierung: Alternative zu Airflow für daten- und codegetriebene Workflows via YAML. 26k Stars. |
| [**Khazix Skills**](https://github.com/KKKKhazix/khazix-skills) | `🧩 Skill` | Multi-Harness Skill Repository: 40+ Skills für Claude Code, Codex, Cursor & Co., inklusive `neat-freak` (`/neat` Codebase-Hygiene), `hy-analysis` (Architektur-Audit) und `storage-analyzer`. |
| [**Laminar (lmnr)**](https://github.com/lmnr-ai/lmnr) | `⚙️ Core Tool` | Open-Source LLM & Agent Observability: Tracing, Prompt-Evaluation und Dataset-Generierung (OpenTelemetry native, Rust/TypeScript). |
| [**LangChain**](https://github.com/langchain-ai/langchain) | `⚙️ Framework` | Connective Tissue Framework: Standardisierte Ketten, Tools, Retriever und Gedächtniskomponenten für LLM-Anwendungen. |
| [**Lawve · awesome-legal-skills**](https://github.com/lawve-ai/awesome-legal-skills) | `🧩 Skill` | 70+ kuratierte Agent-Skills für Legal-Work (NDA-Review, GDPR, Due-Diligence, Commercial Law), beigesteuert von Praktikern; portable Standards statt proprietärer Formate. ~700 Stars. |
| [**LazySkills**](https://github.com/alvinunreal/lazyskills) | `🧩 Skill` | Blazing-fast TUI für Agent-Skills: Prüft installierte Skills, Agenten-Sichtbarkeiten und Konfigurationsfehler in einer übersichtlichen Terminal-Oberfläche. |
| **Liquid Glass / Liquid Logo** | `🎨 Shader Demo` | Demo-Referenzen &#124; Shader-gestützte interaktive Flüssigglas- und Logo-Verzerrungseffekte für moderne Landing Pages. &#124; `IMG_7186`, `IMG_7187` |
| [**Listmonk**](https://github.com/knadh/listmonk) | `☁️ Cloud / SaaS` | Hochperformanter Self-Hosted Newsletter & Transaktions-Mailer: Schneller Go-basierter E-Mail-Dienst (Mailchimp-Alternative) für Massen-Mails und System-Nachrichten bei minimalem Ressourcenverbrauch. |
| [**Lucide Icons**](https://github.com/lucide-icons/lucide) | `⚙️ Framework` | Community-Standard Icon-Bibliothek: Über 1.000 konsistente Icons mit Figma-Plugin und nativer Integration für alle JS-Frameworks. |
| [**Magpie**](https://github.com/magpie-ai/magpie) | `🖥️ OSS App` | Multi-Model Quota Switcher & Local Gateway: Menüleisten-Gateway, das Coding-Agenten (Claude Code auf Kimi, Codex auf DeepSeek, Gemini CLI auf GLM, OpenCode auf ChatGPT) routet und bei Quota-Limits automatisch und lautlos auf den nächsten Account weiterschaltet. |
| [**mattpocock/skills v1.3.1**](https://github.com/mattpocock/skills/releases/tag/v1.3.1) | `🧩 Skill` | Changelog v1.3.1 geprüft: 1. `resolving-merge-conflicts` ersatzlos entfernt (Agenten lösen das nativ). 2. Konvention `CONTEXT.md` zu `GLOSSARY.md`/`GLOSSARY-MAP.md` umbenannt (für `domain-modeling`, `grill-with-docs`, etc.). 3. Cross-Skill-Aufrufe standardisiert auf expliziten Aufruf `Call the Skill tool with "<name>"` statt `/skill`-Syntax (harness-neutral). 4. `grilling`: Trennlinien (`---`) zwischen aufeinanderfolgenden Fragen ergänzt. |
| [**Maxun**](https://github.com/getmaxun/maxun) | `🕷️ Scraper / Data` | No-Code Web Scraping & Crawler Engine: Wandelt Webseiten automatisch in strukturierte REST-APIs um. Unterstützt visuelles Extrahieren, Pagination und AI-Parsing. |
| [**MiniCPM (OpenBMB)**](https://github.com/OpenBMB/MiniCPM) | `🧠 AI Model` | SOTA On-Device Multimodal LLMs: Extrem effiziente Bild- und Sprachverarbeitung direkt auf Endgeräten und Edge-Servern. 17.5k Stars. |
| [**Morphy**](https://get.appmorphy.com/) | `🖥️ Canvas App` | "Early access"-Seite, Funktion aus dem Titel nicht ersichtlich. |
| [**MuAPI**](https://muapi.ai) | `☁️ API Gateway` | All-in-One Model Gateway & API Proxy: Einheitlicher Zugang zu Multi-Model-APIs, Assistenten und Agenten-Workflows mit einheitlichem Abrechnungs- und Concurrency-Handling. |
| [**muapi-cli**](https://github.com/SamurAIGPT/muapi-cli) | `☁️ Cloud / SaaS` | Offizielles CLI & MCP Server für muapi.ai: Generiert Bilder, Videos und Audio direkt aus dem Terminal oder aus Coding-Agenten heraus (14 KI-Modelle). |
| [**Muro**](https://github.com/MrRockySL/Muro) | `🖥️ macOS App` | Schlanke, native Live-Wallpaper-Engine für macOS 14+ mit minimalem RAM- und CPU-Verbrauch. |
| [**Navbar Gallery**](https://navbar.gallery) | `🎨 UI Gallery` | Spezialisierte Referenzsammlung für moderne, interaktive Navigationsleisten. |
| [**Officeverse**](https://officeverse.id) | `⚙️ Framework` | Framework zur programmatischen Generierung von Office-Dokumenten (Word, PPT, Excel) für automatisierte Reportings und Präsentationen. |
| [**Opcode**](https://github.com/winfunc/opcode) | `🖥️ Computer-Use` | Desktop GUI for Claude Code (ehem. Claudia): Erlaubt das Verwalten von Sessions, Projekten, Token-Kosten und Custom Agents in einem einzigen Desktop-Fenster ohne Terminal-Jonglage. |
| [**open-agent-connector**](https://github.com/Anil-matcha/open-agent-connector) | `☁️ Cloud / SaaS` | Open-Source Alternative zu Composio & Nango: Self-hosted Integrationen für GitHub, Slack, Hacker News und HTTP-Actions via MCP oder REST. |
| [**OpenHarness**](https://github.com/autonomous-ai/openharness) | `⚙️ Harness` | The Ultimate Harness for Coding Agents: Universelles Open-Source Harness für autonome Coding-Agenten und Multi-Tool Workflows. |
| [**OpenSEO**](https://openseo.so) | `☁️ SEO Platform` | Open-Source SEO Alternative zu Semrush & Ahrefs: Keyword-Research, Backlink-Audits und offizieller Google Search Console (GSC) MCP Server. |
| [**Paperthin**](https://github.com/LilMGenius/paperthin) | `🧩 Skill` | Cross-Harness Skill-Verteilung (npx skills add LilMGenius/paperthin): Verankert Senior-Engineering-Reflexe und Heuristiken direkt in Claude, Codex, OpenCode und Antigravity. |
| [**playbooks**](https://github.com/playbooks-ai/playbooks) | `⚙️ Engine` | Semantisches Programmiersystem für KI-Agenten: Standardisierte, ausführbare Playbooks zur Steuerung komplexer Agenten-Zyklen. |
| [**Promix (X-Post)**](https://x.com/Promixyz/status/2102424036416348494) | `⚙️ Core Tool` | Post mit einem Kurzlink; Inhalt unklar, Repo nicht aufgelöst. |
| [**PRP-core (Wirasm)**](https://github.com/Wirasm/prp) | `🧩 Skill` | PRP-Methodik (Product Requirement Prompts = PRD + Codebase-Intelligence + Runbook): Plugin mit `/prp-core:prp-prd`, `/prp-core:prp-plan`, `/prp-core:prp-implement`, `/prp-loop` (headless plan→implement→PR→review Loop). 2.2k Stars. Direkt vergleichbar mit unserem Plan-Cycle. |
| [**Recordly**](https://github.com/webadderallorg/Recordly) | `🖥️ Computer-Use` | Open-Source Desktop Screen Recorder: Erstellt ohne Videoschnitt-Kenntnisse professionelle Produkt-Demos mit Cursor-Zoom, Auto-Framing und Studio-Export. 31.8k Stars. |
| [**Refine**](https://github.com/refinedev/refine) | `⚙️ Framework` | React-Framework für Enterprise CRUD & Dashboards: Die Brücke zwischen Low-Code und Custom Code für interne Tools und B2B-Apps mit dediziertem AI Agent. |
| [**Replicate API**](https://replicate.com) | `☁️ Cloud / SaaS` | Serverless GPU Model Execution: Ausführen tausender Open-Source-Modelle (Flux, SDXL, Whisper, LLMs) per API ohne eigene GPU-Cluster-Wartung. |
| [**Rust Skills**](https://github.com/actionbook/rust-skills) | `🧩 Skill` | AI-Powered Rust Development & Meta-Cognition Framework: Claude Code Plugin & Skill-Suite (Ownership, Borrowing, Lifetimes, Concurrency, Unsafe-Checker, Dynamic Skills aus `Cargo.toml`). Schließt die klaffende Rust-Lücke in AOS und ist das Fundament für den Tauri v2 Rust-Core in Orchestrator 2.0. |
| [**social-ai-team**](https://github.com/stevenflanagan1/social-ai-team) | `🧩 Skill` | Komplettes AI-Social-Team für SMBs als Claude-Code-Skills (10 Skills): Brand-Onboarding, Content-Calendar, Caption-Writer, Creative-Designer (Nano Banana), LinkedIn-Writer, Performance-Review. |
| [**TablePlus VMPal**](https://vmpal.app) | `🖥️ macOS App` | Leichtgewichtige VM-App für Apple Silicon & KI-Agenten: Sichere, isolierte Sandboxes für Coding-Agenten auf macOS. |
| [**Tavily API**](https://tavily.com) | `🕷️ Search API` | Real-Time AI Web Search API: Speziell für LLM-Agenten optimierte Websuche mit strukturierten Quellen und bereinigtem Markdown-Content. |
| [**TikTok 5.6B Dataset**](https://huggingface.co/datasets/datasocial/tiktok-5.6B-videos) | `📊 Dataset` | Riesiger Trainings- und Analyse-Datensatz für virale Videoformate, Hooks und Metadaten. |
| [**ToolJet**](https://github.com/ToolJet/ToolJet) | `☁️ Cloud / SaaS` | Low-Code Internal Tools Builder (Retool-Alternative): Schneller Bau von Admin-Dashboards, Datenbank-UIs und Kunden-Backends mit visuellen Komponenten und Anbindung an interne APIs. |
| [**Warren**](https://github.com/Dymyt-ry/warren) | `🖥️ Agent UI` | "Agents are teammates now. Give them a room.": Ein Baum aus Räumen für Menschen + Coding-Agenten; `@mention` landet direkt in der laufenden Session. Local-first (localhost:8790), MIT. |
| [**yanliudesign (Yan Liu)**](https://github.com/yanliudesign) | `⚙️ Core Tool` | GitHub-Profil eines Designers; relevante Repos noch nicht ermittelt. |

---

## 2. Multi-Agent Orchestration, Swarms & Protocols

*Anzahl kuratierter Tools: 13*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**A2A Protocol**](https://github.com/a2aproject/A2A) | `📐 Pattern` | Agent-to-Agent Interoperability Protocol: Offener Standard zur Kommunikation zwischen unterschiedlichen, isolierten Multi-Agenten-Systemen (Discovery, Modalitäten-Aushandlung, Task-Kollaboration). Ergänzt MCP auf Agent-Ebene. |
| [**Agno (AgentOS)**](https://github.com/agno-agi/agno) | `⚙️ Framework` | Multi-Modal Agent Platform & Runtime (ehem. Phidata): Eigenständiger Agenten-Stack mit Memory, Session-Store, RBAC und integriertem Web-Dashboard. |
| [**AI Employees**](https://github.com/markfulton/ai-employees) | `⚙️ Framework` | 8 Open Source AI Employees & 60 Scheduled Routines: Deckt die Domänen GTM, SEO, WebDev, Social, Ads, Sales, Support und Chief of Staff ab. Füllt die bisher schwächste Domäne in AOS (`saas-ops` / Business-Workflows) mit schlüsselfertigen Routinen, abgesichert über das AOS GO-Gate. |
| **Autonomous 4-Eyes Factory Pattern** | `📐 Pattern` | Deterministischer Build- & Review-Loop: Feature -> Spec-Writer (Opus) -> Builder (Opus) -> 4 parallele Reviews (Security [Opus], UX [Sonnet], UI-Design [Sonnet], Code [Sonnet]) -> max. 2 Runden -> All Pass -> Approve -> Merge to main. Bei Eskalation: Human-Approval. |
| [**ChatDev 2.0 (DevAll)**](https://github.com/OpenBMB/ChatDev) | `⚙️ Framework` | Zero-Code Multi-Agent Platform: Nachfolger des klassischen ChatDev für universelle Multi-Agenten-Orchestrierung. Erlaubt die visuelle und deklarative Definition kollaborierender Agenten-Teams ohne Code. |
| [**CrewAI**](https://github.com/crewAIInc/crewAI) | `⚙️ Framework` | Rollenbasiertes Multi-Agenten-Framework: Orchestrierung spezialisierter Agenten (Researcher, Writer, Reviewer) über strukturierte Konfigurationen. |
| [**DeerFlow 2.0 (ByteDance)**](https://github.com/bytedance/deer-flow) | `⚙️ Framework` | Open-Source Multi-Agent Workflow-Plattform von ByteDance: Deep Research, Reasoning, Web-Browsing und Sandbox-Code-Ausführung. |
| [**OmniRoute**](https://github.com/diegosouzapw/OmniRoute) | `⚙️ Framework` | Freies MIT-AI-Gateway: ein Endpoint, 359 Provider (150+ gratis), 1200+ Modelle; Quota-aware Auto-Fallback, RTK+Caveman-Kompression (15–95 % Token-Ersparnis), MCP/A2A. Läuft mit Claude Code, Codex, Cursor, OpenCode, Cline, Copilot. |
| [**OpenFlow**](https://github.com/patrikbergd/openflow) | `⚙️ Framework` | Visueller Canvas-Builder für Multi-Agenten-Pipelines: Drag-and-Drop Pipeline-Verschaltung (Planner → Architect → Coder), angetrieben von opencode serve. |
| [**OpenRig**](https://github.com/mvschwarz/openrig) | `⚙️ Framework` | Multi-Agent-Harness (Claude Code + Codex als ein System): Agent-Team in YAML (RigSpec) definiert, `rig up` bootet tmux-Sessions, Topologie-Graph-TUI, Sessions adoptieren, `rig send/broadcast/chatroom`, Snapshot/Restore. ~2k Stars, npm `@openrig/cli`. Konkurrenz/Synergie zu AO-Orchestrator. |
| [**Switch**](https://github.com/flintai/switch) | `⚙️ Framework` | Human-Agent Collaboration Framework: Bindet KI-Agenten nativ in bestehende Team-Kanäle (Slack, Discord, Linear) ein, inklusive Console und Playground. |
| [**Taskuary**](https://github.com/idbumble/taskuary) | `⚙️ Framework` | Personal AI Assistant for your Job: E-Mails, Chats und Tickets werden in Aufgaben verwandelt; bestehende Agenten (Claude Code, Codex, Gemini) arbeiten sie im Hintergrund ab. |
| [**Warp Agentic**](https://warp.dev) | `⚙️ Framework` | Warp Terminal built for coding with multiple AI agents: Multi-Agent Kollaboration im Terminal für macOS, Linux und Windows. |

---

## 3. Computer-Use, OS Sandboxing & Remote Desktops

*Anzahl kuratierter Tools: 15*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**AWS Strands-Box**](https://github.com/strands-agents/box) | `🖥️ Computer-Use` | OS-Level Sandboxing für autonome Agenten: Dogwood Policy Language (zeitliche & bedingte Regeln), External Secret Injection. Behebt das in AOS anerkannte Residual-Sicherheitsdefizit (H2: "Gate is not a sandbox") für ungetestete Agentenbefehle. |
| [**Bops**](https://github.com/OrgoAI/bops) | `🖥️ Computer-Use` | Autonome Business-Ops Bot-Flotte: Mac-App, bei der jeder Bot einen eigenen Orgo-Cloud-Computer mit 4 Bildschirmen hat. Zugriff auf 1000+ Tools via Composio, Langzeitgedächtnis via Honcho und Computer Use via Codex. FSL-1.1. |
| [**Celesto**](https://github.com/CelestoAI/celesto) | `🖥️ Computer-Use` | Secure & Persistent Computer for AI Agents: Bietet isolierte, persistente Cloud/Desktop-Umgebungen (inkl. Windows Guide) für Agenten-Execution. Essentiell für sichere Code-Ausführung außerhalb der Host-Maschine. |
| [**CUA (Trycua)**](https://github.com/trycua/cua) | `🖥️ Computer-Use` | Scale Computer-Use 2.0: Open-Source OS-Treiber, Cross-OS Flotten (Mac/Windows/Linux) und Evaluierungs-Benchmarks für Computer-Use Agenten. Direkte Synergie mit den AOS Computer-Use MCPs. |
| [**ESP32 iPhone Agent**](https://github.com/onehumanbeing/esp32-iphone-agent) | `🤖 Hardware` | $7 Hardware-Agent zur physischen iPhone-Steuerung: Agiert als Bluetooth-HID-Gerät für automatisierte Klicks und Tests ohne Jailbreak oder Dev-Account. |
| [**Google Artemis**](https://github.com/google/artemis) | `🖥️ Computer-Use` | Android & Mobile UI Automation mit nativem MCP Server: Ermöglicht Coding-Agenten das direkte Steuern und Testen von physischen/virtuellen Mobilgeräten via ADB & Computer-Use (Observe-and-Act Loop). |
| [**LCU**](https://github.com/AMONTLABS/LCU) | `🖥️ Computer-Use` | Decoupled Computer Use: Universelle Maus- und Tastatur-Steuerung für beliebige Coding-Agenten und Harnesses. |
| [**Microsoft Quicksand**](https://github.com/microsoft/quicksand) | `🖥️ Computer-Use` | Lightweight Agent Sandboxing: Extrem schnelles Sandboxing von AI Agenten zur Verhinderung destruktiver Host-Eingriffe. Erlaubt isolierte Dateisystem- und Netzwerk-Zyklen. |
| [**Open SaaS**](https://github.com/wasp-lang/open-saas) | `🖥️ Computer-Use` | Fullstack SaaS Starter Kit (Wasp / React / Node / Prisma): Bringt Stripe-Abrechnung, Rollen/Auth, Background Jobs und E-Mail-Templates out-of-the-box mit. Ausgezeichnete Vorlage für Saasengine-Endprodukte. |
| [**open-dots**](https://github.com/Anil-matcha/open-dots) | `☁️ Cloud / SaaS` | Self-Hosted AI Agent Workspace & Alternative zu OpenAI Operator / Claude Cowork: MIT-Lizenz, Chat-UI, Connectors, Human-in-the-Loop Freigaben und optionaler Computer-Use. |
| [**QuickDesk**](https://github.com/barry-ran/QuickDesk) | `🖥️ Computer-Use` | AI-Native Remote Desktop mit MCP Server: Open-Source Remote Desktop, der es beliebigen Agenten via standardisiertem MCP Server erlaubt, entfernte Rechner visuell wahrzunehmen und zu steuern (Maus, Tastatur, Screen). Direkte Brücke zu bdb-os-remote! |
| [**Sill**](https://github.com/Saffsanity/sill) | `🖥️ Computer-Use` | Low-Latency Mac-to-iOS Display Mirroring (getsill.app): Streamt beliebige macOS-Fenster mit HEVC auf iPad/iPhone mit Touch- und Apple-Pencil-Rückkanal (P2P/Tailscale). |
| [**Squid**](https://github.com/agent-squid/squid) | `🖥️ Computer-Use` | Your Local Coding Agents, Unified: Vereint lokale Coding-Agenten unter einer gemeinsamen Oberfläche. |
| [**Windows-MCP**](https://github.com/cursortouch/windows-mcp) | `🖥️ Computer-Use` | Native Windows Computer-Use MCP Server: Bringt Cursor, Claude Code und Antigravity direkte Desktop-Interaktion unter Windows. |
| [**Windows-Use**](https://github.com/sirendhead/Windows-Use) | `🖥️ Computer-Use` | Open-Source Computer-Use for Windows: Speziell auf Windows abgestimmte UI-Automatisierung für Coding-Agenten via Vision & OS Accessibility APIs. |

---

## 4. Context, Memory, AST Code-Graphs & Knowledge

*Anzahl kuratierter Tools: 16*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**book-to-skill**](https://github.com/epishkin/book-to-skill) | `🧩 Skill` | Dokumenten- und Buch-zu-Skill-Generator: Transformiert Fachbücher, PDFs und Source-Ordner in abrufbare Agent-Skills für Claude Code und Codex. |
| [**cao (Answer me with HTML)**](https://github.com/epishkin/cao) | `🧩 Skill` | Token-sparender Visual Explainer Skill: Erzeugt interaktive HTML-Erklärungsseiten nach ASD-STE100 bei 1/7 des typischen Token-Aufwands. |
| [**Codebase Memory MCP**](https://github.com/DeusData/codebase-memory-mcp) | `☁️ Cloud / SaaS` | AST Knowledge-Graph MCP Server: Parst Repositories via Tree-Sitter & LSP in eine lokale SQLite-Wissensdatenbank. Reduziert Kontext-Tokens bei Code-Recherche um bis zu 99% (z.B. von 412k auf 3.4k Tokens). Direkte Synergie mit Synapse & memB. |
| [**COG (Cognition + Obsidian + Git)**](https://github.com/SafeSynt/cog) | `⚙️ Core Tool` | Self-Evolving Second Brain (13k Stars): Agentengeführtes Wissenssystem rein auf Basis von Markdown-Dateien und Git-Versionierung. |
| [**context-mode**](https://github.com/mksglu/context-mode) | `🖥️ OSS App` | Context Window Optimization & Sandboxing: Reduziert Tool-Outputs in Coding-Agenten um bis zu 98% (z.B. 315 KB auf 5.4 KB in Claude Code), persistiert Session-Memory und routet Tools über 17 Plattformen via MCP und Hooks (26k Stars). |
| [**Headroom**](https://github.com/headroomlabs-ai/headroom) | `🖥️ Computer-Use` | Kontext-Kompressions-Layer für KI-Agenten: Reduziert Input-Tokens um bis zu 57% (bei JSON/RAG 60–95%) durch intelligentes Pruning, behält aber kritische Logs (z.B. FATAL-Zeilen) byte-genau bei. Desktop-App (`Glance Switch / AG`) läuft lokal auf macOS ohne Cloud-Uploads. |
| [**Karakeep (ehem. Hoarder)**](https://github.com/karakeep-app/karakeep) | `☁️ Cloud / SaaS` | Self-Hostable Bookmark-Everything App: Automatische KI-Verschlagwortung, Volltextsuche, lokale Bild-/Link-Archivierung (auch mit Ollama). Bildet die visuelle Brücke zwischen Web-Recherche (`bdbrainstorm`) und memB Vektor-Gedächtnis. |
| [**Knowledge Work Plugins**](https://github.com/anthropics/knowledge-work-plugins) | `🧩 Skill` | Offizielle Claude Plugins von Anthropic: Offizielles Plugin-Repository für Wissensarbeiter und Entwickler-Workflows. |
| [**llmtrim**](https://github.com/fkiene/llmtrim) | `🖥️ OSS App` | Lokaler LLM-Traffic-Kompressor: Reduziert API-Token (-31% In, -74% Out) bei nur ~5ms Latenz durch semantisch verlustfreie Kompression. |
| [**Mem0**](https://github.com/mem0ai/mem0) | `🖥️ OSS App` | Persistente Langzeit-Memory für Agenten: Speichert Konversationen, Entscheidungen und Fakten über Sessions hinweg; verhindert Gedächtnisverlust bei Agenten-Neustarts. |
| [**Outline**](https://github.com/outline/outline) | `☁️ Cloud / SaaS` | Team Knowledge Base & Wiki: Schnelles, schickes Dokumentations- und Wissenssystem (Notion/Confluence-Alternative) für interne Teams und Kundenhandbücher. |
| [**Raven (EverMind)**](https://github.com/EverMind-AI/Raven) | `⚙️ Framework` | "The Harness of Harnesses", gebaut für RSI (recursive self-improvement): Host-Agent, der eigene + Third-Party-Agenten (Claude Code, Codex, OpenCode, Hermes, OpenClaw…) orchestriert; EverOS-Memory (Markdown-native, local-first), Evolver bewertet Harness-Änderungen gegen Benchmarks. 4.4k Stars, Apache-2.0, pre-alpha. |
| [**Repowise**](https://github.com/repowise-dev/repowise) | `🖥️ OSS App` | AST Codebase Intelligence & Health MCP: Parst Dependency Graphs, Git-Historie, Tests und Architekturentscheidungen. Verhindert, dass Agenten bei jedem Prompt teuer die gesamte Codebase neu durchsuchen müssen. AGPL-3.0. |
| [**Syncthing**](https://github.com/syncthing/syncthing) | `🖥️ OSS App` | Dezentraler Cross-Device Datei-Sync: Peer-to-Peer, Ende-zu-Ende verschlüsselt ohne Cloud. Nützlich zur nahtlosen Replikation von `~/.aos/` Konfigurationen, Worktrees und memB Embeddings zwischen MacBook und stationärem GPU-Rig. |
| [**trim-1**](https://github.com/caveman-ai/trim-1) | `🖥️ OSS App` | Ultra-schneller Build-Log-Trimmer: Slicet gigabytelange Compiler- und CI/CD-Logs auf den exakten Fehlerkontext für LLM-Prompts herunter. |
| [**Understand Anything**](https://github.com/Egonex-AI/Understand-Anything) | `🖥️ OSS App` | Interaktive Codebase-Wissensgraphen: Generiert dynamische Architektur- und Abhängigkeitsgraphen aus Code und Dokumentation für Coding-Agenten. |

---

## 5. Security, Pentesting, CI/CD & Verification Gates

*Anzahl kuratierter Tools: 10*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**bug-bounty-hunting-prompts**](https://github.com/mdpsec/bug-bounty-hunting-prompts) | `🛡️ Security` | Strukturierte Bug-Bounty-Prompts: Verwandelt chaotisches Ausprobieren in einen evidenzbasierten Sicherheits-Workflow für LLMs und Security-Agenten. |
| [**Claude-BugHunter**](https://github.com/elementalsouls/Claude-BugHunter) | `🧩 Skill` | Multi-Harness Red-Team & Security Pipeline: Agent-Skill-Paket für Claude Code, OpenCode, Codex CLI und Antigravity mit Burp MCP Ports, 6-Phasen-Workflow und 7-Fragen-Validierungs-Gate gegen False Positives. |
| [**e2e (tester-army)**](https://github.com/tester-army/e2e) | `🛡️ Security` | Replay-fähiges Agent-Testing Framework: Kombiniert natürlichsprachliche Agenten-Schritte (`agent.act`) mit Playwright-Locators für Web, iOS und Android (Apache 2.0). Einmal erfolgreiche Schritte werden gecacht und bei Folge-Läufen ohne erneute Modell-Calls kostenlos wiederholt. |
| [**Headcount**](https://github.com/cbrock84/headcount) | `🛡️ Security` | Add a department, not a prompt: 16 Departments, 146 Skills speziell für Claude Code gebaut (Security, Legal, Product, Tech, Operations, Marketing, Finance). Ideale Ergänzung zu den AOS Playbooks. |
| [**Pullfrog**](https://github.com/pullfrog/pullfrog) | `🛡️ Security` | BYOK CodeRabbit in GitHub Actions: Autonome PR-Reviews, automatisches Beheben von CI-Fehlern, Merge-Konflikten und Issue-Triage direkt in CI/CD mit Claude, Codex, Grok oder OpenCode. |
| [**security-audit-skill (Cloudflare)**](https://github.com/cloudflare/security-audit-skill) | `🧩 Skill` | Coding-Agent-Skill für mehrphasige Security-Audits mit unabhängig verifizierten, maschinenlesbaren Findings. Vergleichbar mit Strix / Claude-BugHunter (Kat. 1). |
| [**Strix**](https://github.com/usestrix/strix) | `🛡️ Security` | Autonomer AI Penetration Testing Agent: Testet Web-Apps und APIs wie ein echter Hacker. Validiert Schwachstellen, generiert PoC-Exploits und liefert Fixes. Go / Bubble Tea TUI. Ideal als Gate-Check vor Releases. |
| [**Tracecat**](https://github.com/TracecatHQ/tracecat) | `🛡️ Security` | Open-Source AI-Native Security Automation (SOAR): Orchestriert Agenten, MCP-Tools und Incident-Playbooks auf Basis von Temporal. |
| [**Watermarks Remover**](https://github.com/guillaumemoyer/watermarks-remover) | `🛡️ Security` | AI-Provenance & Hygiene Service (23.4k Stars): Entfernt unsichtbare Unicode-Wasserzeichen, C2PA-Marker und KI-Fingerprints aus Texten und Code. |
| [**Zerra**](https://github.com/zerra-ai/zerra) | `🛡️ Security` | Local-First Blue-Team AppSec-Scanner: Findet Schwachstellen und Secrets in Repos, verifiziert Fixes in Sandboxes und generiert automatische Pull Requests ohne Telemetrie. |

---

## 6. Frontend, UI-Komponenten & Design Systems (Godmode UI/UX)

*Anzahl kuratierter Tools: 54*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**21st.dev**](https://21st.dev) | `🎨 Design Lib` | Großer Marktplatz für moderne React-Komponenten für individuelles Design abseits des Standard-KI-Looks. |
| [**AG-UI Protocol**](https://ag-ui.org) | `🎨 Design Lib` | Offener UI-Standard für Agent-Oberflächen: Einheitliche Protokoll-Events (`RUN_STARTED`, `TOOL_CALL_START`, `TEXT_MESSAGE_CONTENT`, `RUN_FINISHED`) für beliebige Agenten und Frontends. |
| [**Agents Observe**](https://github.com/simple10/agents-observe) | `🎨 Media Tech` | Echtzeit-Observability-Dashboard für Claude Code & Codex: Lokales Web-Dashboard (`localhost:5173`) mit Multi-Agenten-Filterung, Session-Replay, Suchfunktion und genauer Token-Kostenanalyse. |
| [**Anatomy**](https://github.com/wheresryan22/anatomy) | `🧩 Skill` | Interaktive 3D/SVG-Zerlegung als Agent-Skill: Erklärt Konzepte und Architekturen, indem es sie als funktionierendes, interaktives isometrisches 3D-Objekt aus präzisen Einzelteilen (SVG, WebGL, 3D) generiert (`npx skills add wheresryan22/anatomy`). |
| [**Animos**](https://animos.app) | `🎨 Design Lib` | Browserbasiertes Tool zur Erstellung und zum Export (MP4) von ansprechenden UI-Animationen und Produkt-Showcases. |
| [**ascii.rest**](https://ascii.rest/) | `🎨 Media Tech` | Animierte ASCII-Art für Webseiten (von @bas3line). Design-Inspiration. |
| [**Awwwards Skill (/awwwards)**](https://github.com/juliobsz/skills) | `🧩 Skill` | High-Agency Frontend-Designer Skill: Erstellt preisverdächtige Websites aus einem Einzeiler inklusive visueller Browser-Validierung. |
| [**Backgrounds Supply**](https://backgrounds.supply) | `🎨 Media Tech` | Hochwertige Texturen, Gradients und Mesh-Hintergründe für Hero-Sections und moderne Webseiten. |
| [**Chakra UI**](https://chakra-ui.com) | `🎨 Design Lib` | Einfaches Styling-System mit modularen, zugänglichen Komponenten für schnelles Prototyping. |
| [**Claude Code Mods**](https://github.com/nateherkai/claude-code-mods) | `🎨 Media Tech` | 4 unverzichtbare UI-Mods für Claude Code: 1. `CacheKeeper` (Echtzeit-Timer für 5-Min-Cache-Expiry, Token-Kosten-Warnung), 2. `Goal Tracker` (visueller Fortschrittsbalken & Subtask-Liste), 3. `Collision Guard` (erkennt Datei-Konflikte bei mehreren parallelen Sessions, Worktree-Prompt), 4. `Next Steps` (Aktionsvorschläge nach jedem Turn). |
| **Claude Code Mods (News)** | `🎨 Media Tech` | ClaudeDevs (X) &#124; News-Impuls: Claude Code ist jetzt moddable — Mods aus TypeScript in Plugins (`/plugin`), UI-Verhalten, Statuslines (z.B. "Token Weather") austauschbar. Relevant für AOS-Plugin-Strategie. &#124; `IMG_7033` |
| [**Claude Code Templates**](https://github.com/davila7/claude-code-templates) | `🎨 Media Tech` | Interactive Web Interface & 100+ Production-Ready Templates: Multi-Agent Collaboration, Live-Visualisierung des Reasonings. Dient als direkter Blueprint zur Modernisierung der `aos store ui` (Port 4322) und des Launchpads (Port 7900) mit One-Click-Testlauf. |
| [**Componentry**](https://github.com/harshjdhv/componentry) | `🎨 Media Tech` | Animierter React-Component-Library (Partikel-Typografie, Liquid-Glass, WebGL-Gradients, Kinetic Text); Install via `npx shadcn @latest add @componentry/...` + MCP. Vercel-OSS-backed. |
| [**Desigma**](https://github.com/deepfounder-ai/desigma) | `🖥️ Design App` | Local-First Open-Source UI-Design-Tool in Rust: Figma-Import, Vektorbearbeitung und Offline-Erstellung ohne Cloud-Zwang. |
| [**designlang**](https://github.com/Manavarya09/design-extract) | `🎨 Design Lib` | `npx designlang <url>` extrahiert komplette Design-Systeme von Live-Websites: W3C-DTCG-Tokens (primitive/semantic/composite), Tailwind-Config, Figma-Variablen, shadcn-Theme, Brand-Book-PDF, MCP-Server für Claude Code/Cursor, WCAG-Remediation. ~4k Stars, MIT. Passt exakt zu DTCG-/Token-Disziplin von Godmode UI/UX. |
| [**diagram-design**](https://github.com/cathrynlavery/diagram-design) | `🎨 Design Lib` | Redaktioneller Diagramm-Skill für Claude Code / Codex: Erzeugt 42 Diagramm-Typen als sauberes, schattenfreies HTML + SVG. Kein generisches Mermaid-Layout, hohe visuelle Eleganz. |
| [**Farm.js**](https://github.com/farming-labs/farm.js) | `🎨 Media Tech` | Fullstack Product Framework: Verbindet Vite's Entwicklungsgeschwindigkeit mit typisiertem App-Directory-Routing, Server Actions und Streaming SSR. Unterstützt React, Solid, Vue und Svelte. |
| [**Footer Design**](https://footer.design) | `🎨 Design Lib` | Inspirationsquelle für kreative und funktionale Footer-Layouts. |
| [**Gauge UI**](https://github.com/thordursk/gauge-ui) | `🎨 Design Lib` | Customizable UI Gauges & Meter Components: Umfangreiche Kollektion modularer Komponenten für Dashboards, Speedometer, Ladebalken und Timer. |
| [**Genjutsu Motion UI**](https://github.com/AThevon/genjutsu) | `🎨 Design Lib` | Motion Design System: Lottie- & SVG-basierte Animations-Workflows, interaktives State-Handling und Keyframe-Controls für High-End Interfaces. |
| **Glassy Dashboard Particles** | `🎨 WebGL Demo` | 🎨 UI Showcase (louis_rlee): 30k Partikel bei 60 fps ohne Lade-Spinner in React/WebGL. |
| **Glitch Orchestra** | `🎨 Media Tech` | @kemb_glitch (Instagram) — noch nicht released &#124; "A Claude Code Mod" vom Glitch Cat Club: Pixel-Arbeiter (conductor/frontend/copy/tests) orchestrieren Claude-Code-Sessions mit Live-Status. Experimental, "sharing soon" — Watchlist-Eintrag. &#124; `IMG_7029`, `IMG_7043`–`IMG_7047` |
| [**Grida (Replace.so)**](https://github.com/gridaco/grida) | `🎨 Media Tech` | Design-to-Code & Canvas Engine: Headless Design System und Canvas-Renderer für automatisierte Benutzeroberflächen. |
| [**hallmark**](https://github.com/Nutlope/hallmark) | `🎨 Design Lib` | Anti-AI-Slop Design Skill für Claude Code, Cursor & Codex: Von Hassan El Mghari. Schützt davor, dass Coding-Agenten generische, langweilige Standard-Komponenten generieren. |
| [**HeroUI (ex NextUI)**](https://heroui.com) | `🎨 Design Lib` | Moderne, polierte React-Komponenten mit nativer Barrierefreiheit für Dashboards und SaaS-Frontends. |
| [**Impeccable**](https://github.com/pbakaus/impeccable) | `🎨 Media Tech` | AI-Design-Skill für Claude / Agenten: Über 20 Befehle (`craft`, `critique`, `polish`, `audit`, `colorize`) zur Vermeidung von KI-Slop. Erstellt `PRODUCT.md` und `DESIGN.md`. |
| [**Jiro.build**](https://jiro.build) | `🎨 Design Lib` | 1.200+ kuratierte UI-Design-Prompts für Webseiten und Dashboards. |
| [**Kojima Generator**](https://kojima-san.vercel.app) | `🎨 Design Lib` | Retro-Futuristische UI- & Sci-Fi-HUD-Komponenten vom Macher von HeroKit. |
| [**Logo Design Skill**](https://github.com/kaankiziltug/logo-design-skill) | `🧩 Skill` | 1.400+ SVG-Referenzen mit automatischen CLI-Prüfskripten (16px-Test, Squint-Test, Mirror-Test) für Claude. |
| [**Magic UI**](https://magicui.design) | `🎨 Design Lib` | Spezialisiert auf Landing Pages: Animierte Texte, Marquees, Grids, Spotlight-Karten und Shader-Effekte. |
| [**Mantine**](https://mantine.dev) | `🎨 Design Lib` | 100+ React-Komponenten und Hooks für funktionale Web-Applikationen und komplexe Interfaces. |
| **Marketing Psychology Skill** | `🧩 Skill` | Gezielte Anwendung von 50+ kognitiven Heuristiken (Loss Aversion, Social Proof, Scarcity, Anchor Effect) auf UI-Copywriting und Funnel-Strukturierung. |
| [**Mobbin**](https://mobbin.com) | `🎨 Media Tech` | Echte UI/UX-Screenflows aus populären Mobile- und Web-Apps zur Analyse von Navigationsmustern. |
| [**MUI**](https://mui.com) | `🎨 Design Lib` | Etabliertes Ökosystem für komplexe Enterprise-Dashboards, Datentabellen und Formularlandschaften. |
| [**OpenBot**](https://github.com/CopilotKit/openbot) | `🎨 Media Tech` | Self-Hosted AI Coworker Stack: Open-Source-Plattform mit AG-UI, Browser- und Tool-Rechten auf eigener Infrastruktur für interne Mitarbeiter-Agenten. |
| [**OpenTakeoff**](https://github.com/Kentucky-ai/opentakeoff) | `🎨 Media Tech` | Building Plan Measurement Engine: Ermöglicht KI-Agenten das exakte Ausmessen von Bauplänen via 40 MCP Tools + Browser Canvas. Perfekter Anwendungsfall für `plan-canvas`. |
| [**Prompsy**](https://prompsy.com) | `🎨 Media Tech` | "The prompt operating system": Prompts speichern/organisieren/optimieren, Bakeoffs (gleicher Prompt × 6 Modelle + Auto-Judge), Snap-&-Mirror (Screenshot → Smart Prompt), Chrome-Extension `/prompsy` überall, Flows-Canvas. SaaS, kein OSS-Repo bekannt. |
| [**Quant-UX**](https://github.com/KlausSchaefers/quant-ux) | `🎨 Media Tech` | Visual Prototyping, Usability Testing & Analytics: Prototyping-Plattform zur automatisierten Auswertung von Nutzerinteraktionen. |
| [**React Aria**](https://react-spectrum.adobe.com/react-aria) | `🎨 Media Tech` | Headless UI-Primitives von Adobe mit vollständiger Barrierefreiheit und flexibler Styling-Hoheit. |
| [**Readme.so**](https://readme.so) | `🎨 Media Tech` | Interaktiver visueller Markdown-Editor zum schnellen Zusammenklicken professioneller README-Dateien. |
| [**Saaspo**](https://saaspo.com) | `🎨 Design Lib` | Kuratierte Sammlung bester SaaS-Landing-Pages, Pricing-Grids und Komponenten-Patterns. |
| [**Screenshot-to-Code**](https://github.com/abi/screenshot-to-code) | `🎨 Media Tech` | Wandelt Screenshots, Figma-Mockups und Screencasts direkt in sauberen Tailwind-, React- oder Vue-Code um. |
| [**second-brain-os**](https://github.com/undefined-ui/second-brain-os) | `🧩 Skill` | Selbstpflegende AI-Wissensdatenbank für Claude Code + Obsidian: Guide, Starter-Vault, Agent-Skills, Skripte. Vergleichbar mit memB / OpenWiki. |
| [**shadcn/ui**](https://ui.shadcn.com) | `🎨 Design Lib` | Der de-facto Standard: Saubere, zugängliche Primitives zum direkten Kopieren in die Codebase. |
| [**Skiper UI**](https://skiper-ui.com) | `🎨 Design Lib` | 106+ animierte React/shadcn-Komponenten im "Single-File"-Ansatz (Image-Reveal, Hover-Effekte, Dynamic Island). |
| [**Space UI**](https://www.spaceui.one) | `🎨 Design Lib` | 101+ interaktive Komponenten für Next.js/Base UI & Tailwind — Liquid-Switches, Morphing-Controls, Shaders, Tactile Microinteractions; MIT, shadcn-CLI-Install. |
| [**Spline 3D**](https://spline.design) | `🎨 Design Lib` | Web-basiertes 3D-Design-Tool mit interaktiven Physik- und Kamera-Events, exportierbar nach React / Three.js / R3F. |
| [**System Design Primer**](https://github.com/donnemartin/system-design-primer) | `📐 Pattern` | Der Standard-Leitfaden für skalierbare Systemarchitektur (DNS, Load Balancer, Caching, Sharding). |
| [**Transitions.dev**](https://github.com/Jakubantalik/transitions.dev) | `🧩 Skill` | UI Transitions Skill für Coding-Agenten: Kuratierte Sammlung eleganter UI-Transitions, die direkt per Agent-Skill (`npx transitions-dev add ...`) in Projekte eingebaut werden können. |
| [**Tremor**](https://tremor.so) | `🎨 Media Tech` | Maßgeschneidert für Analytics: Charts, KPI-Karten und Datenvisualisierungen für Dashboards. |
| [**Uiverse.io**](https://uiverse.io) | `🎨 Design Lib` | Größte Open-Source-Bibliothek für interaktive CSS- & Tailwind-Elemente (Buttons, Checkboxen, Loader, Karten). |
| [**VGPU (Vercel Labs)**](https://github.com/vercel-labs/vgpu) | `🎨 Media Tech` | Agent-Ready WebGPU Library: TypeScript-Framework für WebGPU, Shaders, 3D-Gaussian-Splatting und Raymarching. Speziell entwickelt für die einfache Steuerung durch KI-Coding-Agenten (CLI & MCP-Schnittstellen). |
| [**Watermelon UI**](https://github.com/WatermelonCorp/watermelon-platform) | `🎨 Design Lib` | 600+ freie Open-Source UI-Komponenten und Dashboards für Entwickler und Design-Teams. |
| [**Whiteboard**](https://github.com/devdotfast/whiteboard) | `🎨 Media Tech` | Open-Source Canvas für Mensch-Agent-Design: Desktop-App mit SDK für Claude Code und Codex, auf dem Agenten Systemarchitekturen, Flussdiagramme und UI-Konzepte visuell live aufzeichnen können. MIT. |

---

## 7. Video Generation, Creative Media Tech & Remotion (Godmode Media)

*Anzahl kuratierter Tools: 46*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| **250+ Agent Company Architecture** | `📐 Architecture` | 📐 Multi-Agenten Enterprise Architektur: Blaupause für autonome Abteilungen mit 250+ Agenten. |
| [**Aceternity UI**](https://ui.aceternity.com) | `🎨 Design Lib` | Hochwertige Micro-Interactions, 3D-Karten, animierte Hintergründe und Framer Motion Effekte (v2.0). |
| [**AGRec**](https://github.com/huipengli0708-dot/AGRec) | `🖥️ Screen Recorder` | Screen-Recording- und Walkthrough-Capture für macOS: Aufzeichnung von Agenten-Demos und visuellen Testabläufen. |
| [**ai-clipping-generator**](https://github.com/SamurAIGPT/ai-clipping-generator) | `🎨 Media Tech` | AI Video Clipping SaaS-Starter: Extrahiert virale Shorts, Reels und TikToks automatisch aus YouTube-Videos (Next.js, Stripe, Prisma). |
| [**ani-cli**](https://github.com/pystardust/ani-cli) | `🎨 Media Tech` | Leichtgewichtiges POSIX-Shell CLI-Tool zum schnellen Streamen und Scrapen von Anime im Terminal. |
| [**Animate (Claude Code)**](https://github.com/cth9191/animate) | `🎨 Design Lib` | Procedural Animation in any style for Claude Code: Erstellt animierte Videos vollständig im Code via `<canvas>`, deterministisches Frame-by-Frame Rendering nach MP4 via Headless Browser + ffmpeg. |
| [**Auto-Editor**](https://github.com/WyattBlue/auto-editor) | `🎨 Media Tech` | Automatischer Stille- & Pause-Schneider: CLI-Werkzeug, das Sprechpausen und stille Passagen aus Audio- und Videodateien automatisch herausschneidet. |
| [**autoshorts**](https://github.com/JayWebtech/autoshorts) | `🎨 Media Tech` | Local-First Desktop App für 9:16 Videoclips: Erkennt Highlights in Langformat-Videos per KI und schneidet vertikale Snippets mit viralem Ranking. |
| [**Awesome Seedance**](https://github.com/LearnPrompt/awesome-seedance) | `🎨 Media Tech` | Evidenzbasierte Prompt-Bibliothek für Seedance 2.5 / 2.0: 600+ überprüfte Prompts, 260+ Cross-Model-Runs, 25 Templates und 50 installierbare Video-Skills. |
| [**brag**](https://github.com/latent-spaces/brag) | `🎨 Media Tech` | "You built it. Now brag.": Verwandelt ein fertiges Softwareprojekt mit einem einzigen Terminalbefehl in ein knackiges Launch-Video. |
| [**claude-content-skills**](https://github.com/Ootto-AI/claude-content-skills) | `🧩 Skill` | Quelle der "Reel Automation Suite": 30+ Klartext-Skills; `reel-analyzer` (Frames+Transkript → Hook, Beats, Pacing), `reel-builder`, `content-factory`. 127 Sterne. Der Name "Reel Automation Suite" steht nicht im Repo. |
| [**claude-motion**](https://github.com/whaleyxbt/claude-motion) | `🎨 Motion Kit` | Motion-Design-Toolkit für Coding-Agenten: Remotion-Erweiterung mit visuellen Geschmacksregeln, automatischer Frame-Prüfung, Sound-Engine und Web-Sim-Rendering (60 fps). |
| [**claude-reels**](https://github.com/iamachilles/claude-reels) | `🎨 Media Tech` | Schnitt und Untertitel (ffmpeg, HyperFrames, mlx-whisper) |
| [**claude-video**](https://github.com/bradautomates/claude-video) | `🎨 Media Tech` | "Give Claude the ability to watch any video": `/watch` lädt das Video, extrahiert Frames, transkribiert und übergibt alles an Claude. Dritter Kandidat neben Claude-Watch und Watch Skill (Kat. 1 / 8.1). README geprüft (MIT): voll lokal mit `local`-Engine (Python 3.10+, ffmpeg, yt-dlp, WhisperX; ca. 3 GB Platz, 8 GB RAM); Gemini/Groq/OpenAI sind optionale Cloud-Wege (Gemini lädt Videos zu Google hoch). Instagram Reels sind in der README nicht erwähnt — yt-dlp kann sie evtl. laden, ungetestet. |
| **claude-video** | `🎨 Media Tech` | siehe Kat. 9.1 &#124; `/watch`: Download, Frames, WhisperX lokal &#124; MIT &#124; ja &#124; Analyse-Baustein |
| [**Claude-Watch**](https://github.com/taoufik123-collab/claude-watch) | `🎨 Media Tech` | Video-Analyse-Skill für Claude: Ermöglicht Agenten das Verarbeiten von Videos über FFmpeg-Schnittstellenerkennung (Scene-Change), Whisper-Transkripte, 2-fps-Hook-Analyse und Markdown-Reports. |
| [**CodeVideoModel**](https://github.com/code-video-model/CodeVideoModel) | `🎨 Design Lib` | Open-Source Code-to-Video Engine: MiniMax-H3 basiertes Modell zur code-gesteuerten Videoerzeugung und Szenerie-Animation. |
| [**Convkit (conv)**](https://github.com/shdwfruit/convkit) | `🎨 Media Tech` | Universal CLI Media & File Converter: Ein einheitlicher Befehl (`conv clip.mkv clip.gif`), der 115 Formate automatisch auf ffmpeg, ImageMagick, LibreOffice, pandoc oder Typst abbildet und lokal ausführt (`brew install shdwfruit/tap/convkit`). |
| [**Cult UI**](https://github.com/nolly-studio/cult-ui) | `🎨 Design Lib` | 78+ animierte Primitives & AI-Agent-Patterns: Erweiterung für shadcn/ui mit Framer Motion, AI-SDK-Mustern und vorgefertigten interaktiven Blöcken. |
| [**EffectCraft**](https://github.com/storytold/effectcraft) | `🎨 Media Tech` | Open-Source After Effects Reimplementation: Clean-Room Neubau von Adobe After Effects für Motion Graphics, Compositing und VFX. |
| [**Explainroo**](https://github.com/explainroo/explainroo) | `🎨 Media Tech` | Explainer Videos & Product Demos made by AI Agent: Open-Source: Lokale TTS Voice (Kokoro), Wort-Timing (Whisper) und Canvas-Renderer erzeugen fertige Erklärvideos per Agent. |
| [**fframes**](https://github.com/fframes-studio/fframes) | `🎨 Design Lib` | GPU-beschleunigtes Video-Coding-Framework: Rendert Videos programmatisch via Rust und SVG direkt auf der GPU, statt auf langsame Browser-Canvas-Renderer zu warten. Hohe Relevanz für Hyperframes/OpenMontage. |
| **fframes** | `🎨 Media Tech` | fframes-studio/fframes &#124; — &#124; — &#124; — &#124; — &#124; ❌ 404 — Repo nicht auffindbar, Eintrag in Kat. 3 prüfen |
| [**genart-skill**](https://github.com/camilleroux/genart-skill) | `🧩 Skill` | Deterministisches Rendering, Hash-Seeding; Canvas 2D, p5.js, three.js/WebGL, SVG; erzeugt PNG-Frames, Contact-Sheets, Batch-Export (`/plugin install genart@camilleroux-genart`) |
| [**Hyperframes (HeyGen)**](https://github.com/heygen-com/hyperframes) | `🎨 Media Tech` | "Write HTML. Render video. Built for agents.": Offizielles HeyGen-Framework zur programmatischen Generierung von Videos via TypeScript & WebGL. Keine Cloud-Farmen nötig; perfekte Basis für Video-Agenten. 55k Stars. |
| [**Luma-Dream-Machine-Pro-Premium-Edition**](https://github.com/Dragonkrebaza) | `🎨 Media Tech` | Prompt-/Presets-Sammlung für Luma Dream Machine (Video-Generierung). Qualität unklar — tief priorisiert. |
| [**ManimGx**](https://github.com/academa-labs/manimgx) | `⚙️ 3D Engine` | GPU-beschleunigte 3D-Animationsengine: Rust- und wgpu-basierter Drop-in-Ersatz für Manim CE. Rendert Animationen bis zu 90x schneller als ManimCE (36s 1080p60 Video in 3s auf M4 Pro). |
| [**Mortiflix**](https://github.com/gtkottman/mortiflix-oss) | `🎨 Media Tech` | A Motion Design Studio on your machine: Open-Source Motion Design Engine für programmgesteuertes Rendern. Direkte Bereicherung für den `video-motion-assistant`. |
| [**Motionmaxxing (FinalMotion)**](https://github.com/Tejashmakwana/motionmaxxing) | `🎨 Design Lib` | Looksmaxxing for Motion Graphics: Verwandelt AI-Video-Slop in professionelles Motion-Design. 53 vermessene Momente, 12 Easing-Kurven, 150 Regeln, G0–G5 Mog-Checks via ffmpeg. Perfekter Qualitäts-Linter für den `video-motion-assistant` und die Creator Extension. |
| [**muapi-comfyui**](https://github.com/SamurAIGPT/muapi-comfyui) | `🎨 Design Lib` | ComfyUI Custom Nodes für 600+ Modelle: Zugriff auf Seedance, Kling, Veo3, Flux, HiDream und Imagen4 über muapi.ai. |
| [**onetake**](https://github.com/feitangyuan/onetake) | `🎨 Media Tech` | Claude Agent Skill für "One-Continuous-Take"-Motion-Films: Launch-Films/Teaser, wo jeder Beat aus dem vorherigen wächst statt PPT-artiger Szenen-Stack; Continuity-Oracle misst Carry-Score; klingt wie eine direkte Konkurrenz/Inspiration zu Hyperframes/OpenMontage. PolyForm-Noncommercial, ~1.3k Stars. Install: `git clone ... ~/.claude/skills/onetake`. |
| [**Open-Generative-AI**](https://github.com/Anil-matcha/Open-Generative-AI) | `🎨 Media Tech` | Self-Hosted AI Studio mit 400+ Modellen: Bündelt Bild- und Videomodelle (Flux, Kling, Sora, Wan) in einer filterfreien, selbst gehosteten Oberfläche. |
| [**Open-Higgsfield-AI**](https://github.com/Autom8AI/Open-Higgsfield-AI) | `🎨 Media Tech` | Open-Source Alternative zu Higgsfield AI: Kostenloses Bild- und Video-Generierungsstudio mit 20+ Modellen (Flux, SDXL, Midjourney, Ideogram). Self-hosted & anpassbar. |
| [**OpenChatCut**](https://github.com/0xsl1ne/OpenChatCut) | `🎨 Media Tech` | Lokaler Konversations-Videoeditor: Steuerung der Multitrack-Timeline durch natürliche Sprache; fügt automatisch Untertitel, Übergänge und Musik hinzu. |
| [**OpenCut**](https://github.com/OpenCut-app/OpenCut) | `🎨 Media Tech` | Open-Source CapCut Alternative: Datenschutzfreundlicher, plattformübergreifender Videoeditor gebaut mit Rust, GPUI und React. Multi-Track-Timeline, Ripple-Edits und Keyframes ohne Cloud-Zwang. |
| [**openvid**](https://github.com/CristianOlivera1/openvid) | `🎨 Media Tech` | Browserbasierter Video- & 3D-Mockup-Creator: Erstellt professionelle Produkt-Demos und interaktive 3D-Showcases in Sekunden direkt im Web. |
| [**Pageflows**](https://pageflows.com) | `🎨 Media Tech` | Vollständige Video-Aufzeichnungen von User Flows (Onboarding, Checkout, Upgrades) aus realen Produkten. |
| [**Pixelle-Video**](https://github.com/AIDC-AI/Pixelle-Video) | `🎨 Media Tech` | End-to-End KI-Videoengine via ComfyUI: Erzeugt aus einem simplen Text-Prompt ein komplettes Kurzvideo inkl. Drehbuch, Bildgenerierung, Voiceover und Schnitt lokal auf der eigenen GPU. |
| [**programmatic-reel**](https://github.com/gurungabit/programmatic-reel) | `🎨 Media Tech` | Skript, Voiceover (Kokoro TTS), Musik, Rendering über Remotion |
| **Reel Automation Suite** | `🧩 Skill` | Multi-Skill Setup &#124; Trio aus `/reel-analyzer` (Hook-, Struktur- und Pacing-Analyse), `/reel-builder` (Skript, Voiceover, Untertitel & Musik) und `/content-factory` (End-to-End Automatisierung). &#124; `IMG_7169`, `IMG_7196` |
| [**Swishy**](https://swishy.ai) | `🎨 Design Lib` | AI-gestützter Motion Designer zur schnellen Erstellung von Web- und Social-Media-Animationen. |
| [**twozero (TouchDesigner MCP)**](https://github.com/404dotzero/twozero-td-mcp) | `🎨 Design Lib` | "Vibe noding for TouchDesigner": Von @404.zero × @setupdesigns. Generiert TouchDesigner-Netzwerke via Claude Code & MCP direkt per Chat. Native Echtzeit-Visuals und Lichtshow-Steuerung. |
| **Video Arena Elo Ranking** | `🎨 Media Tech` | Artificial Analysis &#124; Rangliste führender Video-Generierungsmodelle (Sep 2026: Wan 3.0, Utopai X, Seedance 2.5, MiniMax H3, Gemini Omni Flash 1.1). &#124; `IMG_6942.PNG` |
| [**video-to-markdown**](https://github.com/marcomontalbano/video-to-markdown/tree/main) | `🎨 Media Tech` | Videos in Markdown-Dateien einbetten (Vorschaubild + Link). Nützlich für Reports mit Video-Referenzen. README geprüft: braucht einen Cloudinary-Account und pnpm, anonyme Analytics (Simple Analytics) — für lokalen Einsatz ungeeignet. |
| [**Watch Skill · DeepWatch**](https://github.com/oxbshw/watch-skill) | `🧩 Skill` | "Give AI agents eyes, ears, and verifiable results": Video/Audio/Screenshots → persistenter, timestamped Evidence-Index (OCR, Whisper, 1800+ Quellen); 39 MCP-Tools + CLI + REST; THE LOOP (capture→critique→fix→verify) prüft Agentenarbeit deterministisch. Functional twin von Claude-Watch (s. Kat. 1) — andere Codebasis. |
| **Watch-Skill vs Claude-Watch** | `📐 Comparison` | 🧩 Skill-Vergleich: Gegenüberstellung von watch-skill und Claude-Watch für Session-Monitoring. |

---

## 8. Hardware, Robotics & PCB Engineering

*Anzahl kuratierter Tools: 3*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| **Auto-aiming Trash Can (htx_studio)** | `🤖 Hardware` | 🤖 Hardware & Robotics Experiment: Autonom ausgerichteter Papierkorb mit Computer Vision. |
| **Manti Robotics PCB** | `🔌 Hardware` | `MANTI Engineering Workbench` &#124; Hardware & Robotics Engineering Workbench: KI-gesteuertes PCB-Design (ESP32-P4/C6, JLC Fertigung, Routing). Perfekte Ergänzung für den `pcb-design-assistant`. &#124; `IMG_7254.PNG`, `IMG_7255.PNG` |
| [**Text-to-CAD**](https://github.com/earthtojake/text-to-cad) | `🔌 Hardware` | 3D-CAD Superpowers für Coding-Agenten: Generiert lokale STEP-, GLB-, STL- und 3MF-Modelle via Build123d und OpenCASCADE, führt DFM-Prüfungen durch und erstellt technische Zeichnungen für Fertigungsdienstleister (17k Stars). |

---

## 9. Cloud Infrastructure, Flotten-Management & SaasEngine

*Anzahl kuratierter Tools: 16*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**Bento**](https://github.com/nyblnet/bento) | `☁️ Cloud / SaaS` | Single-File Local-First Office Suite: Das gesamte Dokumenten- und Präsentations-Tool passt in eine einzige HTML-Datei. Keine Cloud-Abhängigkeiten, KI-lesbares JSON-Format, Claude-Plugin. |
| [**Breakscale**](https://github.com/xevrion/breakscale) | `☁️ Cloud / SaaS` | Diskreter System-Design Simulator: Interaktiver Canvas zur Simulation von verteilten Systemen unter Last – visualisiert Queueing-Verhalten, Latenz-Percentile, Circuit-Breaker und Retry-Storms mit echten diskreten Ereignissen. |
| [**Claude Skills Founder (Pricing Strategy)**](https://github.com/emotixco/claude-skills-founder) | `🧩 Skill` | SaaS-Pricing & Founder Toolkit für Claude Code: Befehle wie `/founder:pricing-strategy` zur systematischen Evaluierung von Preismodellen, Tier-Strukturen und Unit Economics direkt im Terminal. |
| [**Coolify**](https://github.com/coollabsio/coolify) | `☁️ Cloud / SaaS` | Open-Source PaaS (Heroku / Vercel Alternative): Zentrale Orchestrierung für Bare-Metal- und Cloud-Server via SSH. Ideal für die BDB-Flotten-Bereitstellung von Apps, Datenbanken und Services ohne Vendor Lock-in. |
| [**golive-skill**](https://github.com/mikehasa/golive-skill) | `🧩 Skill` | Agent-Skill + Node-CLI (ohne Abhängigkeiten): bringt ein Agent-Produkt live (Hosting, DB, Domain, E-Mail, Payments) auf eigenen Accounts; Ablauf detect → plan → approve → apply → verify. Kein Backend, keine Telemetrie. README geprüft (MIT): Zugangsdaten liegen im Klartext in `~/.config/golive/credentials` (Modus 0600); braucht Accounts bei Vercel/Netlify, Supabase/Neon, Registrar, Resend, Stripe. |
| [**gstack**](https://github.com/garrytan/gstack) | `☁️ Cloud / SaaS` | Production-Ready Fullstack-Templates von Garry Tan für schnelles Software-Scaffolding und Deployments. |
| [**InsForge**](https://github.com/insforge/insforge) | `☁️ Cloud / SaaS` | All-in-one Backend Platform for Agentic Coding: Schnelles, agenten-optimiertes Backend-System mit Datenbank, Auth und APIs (191k Downloads). |
| [**Mixpost**](https://github.com/inovector/mixpost) | `☁️ Cloud / SaaS` | Self-Hosted Social Media Management: Open-Source-Alternative zu Buffer und Hootsuite. Multi-Account-Planung, Analytics und Medien-Verwaltung auf eigener Infrastruktur. |
| **Offizielle Cloud MCP Server** | `☁️ Cloud / SaaS` | Provider-Verzeichnis &#124; Vercel (`vercel/next-devtools-mcp`), Cloudflare (`cloudflare/mcp-server-cloudflare`), GCP (`GoogleCloudPlatform/cloud-run-mcp`), Tencent Cloud & Hostinger. &#124; `IMG_7147` |
| [**Paperless-ngx**](https://github.com/paperless-ngx/paperless-ngx) | `☁️ Cloud / SaaS` | Supercharged Document Management System: Scannt, archiviert, taggt und durchsucht Rechnungen, Verträge und Belege automatisch per OCR. Relevante Backend-Infrastruktur für Agentur-Playbooks (`pb-invoice-check`). |
| [**Plexo**](https://github.com/anmolkapil/plexo) | `☁️ Cloud / SaaS` | Multi-Network Bonding Download Manager: Bündelt parallele Internetverbindungen (WLAN, Ethernet, USB-Tethering) in parallele Streams für maximale Download-Geschwindigkeiten. |
| [**Postiz**](https://github.com/gitroomhq/postiz-app) | `☁️ Cloud / SaaS` | Open-Source AI Social Media Scheduler (35k Stars): Multi-Platform-Scheduling, Content-Planung und Analytics (Next.js, Prisma, BullMQ). |
| [**Send**](https://github.com/timvisee/send) | `☁️ Cloud / SaaS` | Verschlüsselter Dateiversand mit automatischer Löschung: Sicheres, flüchtiges Bereitstellen von Produktionsartefakten aus `production_artifacts/` an externe Partner mit Ablauf-Timer. |
| [**Shipyard**](https://github.com/cosscom/shipyard) | `☁️ Cloud / SaaS` | Run Coding Agents on Remote Dev Machines: Verlagert Coding-Agenten vom Laptop auf VPS, Cloud-VMs oder Heimserver. Jeder Agent läuft in eigenem Git-Worktree mit Dev-Server. Mac-App mit Kanban-Status. |
| [**Shoutrrr / Shouter**](https://github.com/coollabsio/shoutrrr) | `☁️ Cloud / SaaS` | Social Media Scheduler (Buffer / Typefully Alternative): Zentrales Verfassen und zeitgesteuertes Ausspielen von Beiträgen auf X, LinkedIn, Instagram und Bluesky. Self-hosted über Docker/Coolify. |
| **Twelve Dollar Server Challenge** | `📐 Pattern` | Rust/epoll-basierte Hochleistungs-Serverarchitektur (rust-epoll-scooter): Benchmark für extreme Concurrency-Lasten auf Minimal-Hardware ($12/Monat). |

---

## 10. Web Scraping, Lead Generation & Extraction Tools

*Anzahl kuratierter Tools: 1*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**Google Maps Scraper Kit**](https://github.com/Mahanaicoach/google-maps-scraper-kit) | `🕷️ Scraper / Data` | Lokaler Google Maps Scraper mit Docker & Claude Skill: Kostenloser lokaler Lead-Scraper ohne externe API-Kosten. |

---

## 11. Reverse Engineering & Binary Analysis

*Anzahl kuratierter Tools: 3*

| Tool / Projekt | Typ | Beschreibung & Relevanz für BDB |
| :--- | :--- | :--- |
| [**Cutter**](https://github.com/rizinorg/cutter) | `🔍 Reverse Eng.` | Free & Open-Source Reverse Engineering Platform: Powered by Rizin / Radare2 mit Ghidra Decompiler. Erweitert das Security-Review-Portfolio (`security-reviewer`) um tiefe Binäranalyse und Disassembly. |
| [**Ghidra (NSA)**](https://github.com/NationalSecurityAgency/ghidra) | `🔍 Reverse Eng.` | Premier Software Reverse Engineering Suite (55k+ Stars): Disassembler, Decompiler und interaktiver Code-Graph für Windows, macOS und Linux. |
| [**REA (Reverse Engineer Anything)**](https://github.com/morluto/rea) | `🔍 Reverse Eng.` | Reverse Engineering MCP für Agenten: Ermöglicht Coding-Agenten das automatisierte Analysieren und Decompilieren von Binärdateien, Web-APIs und App-Interna. #3 Trending Repo of the Day. |

---
