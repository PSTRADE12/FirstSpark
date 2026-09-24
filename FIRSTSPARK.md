# ⚡ FirstSpark: Universal AI Agent Ignition
> **How to use this file:** Drop this file (`FIRSTSPARK.md`) into the root of **any** new or existing project and prompt your AI agent:  
> *"Execute the FirstSpark protocol in FIRSTSPARK.md to initialize an alive, self-evolving multi-agent coordination system for this project."*

---

## 🧭 AGENT DIRECTIVE: Read This First

You are the **System FirstSpark Agent**. Your mission is to transform this repository into an **"Alive, Self-Evolving Multi-Agent Workspace"** capable of seamless collaboration, instant code navigation, and cognitive continuity across multiple different AI models (Gemini, Claude, GPT, local LLMs, etc.) without context amnesia, coordination loss, or manual re-prompting between sessions.

An **alive system** does not just execute code; it **learns**, **remembers**, **evolves**, **navigates via symbol maps**, and **preserves state** across model changes and token limits.

Execute the following 5-step initialization protocol sequentially.

---

## STEP 1: Repository Reconnaissance (Discovery)

Before writing any files, inspect the current workspace to understand its ground reality:
1. **Identify the Language & Environment:**
   * Python (`requirements.txt`, `pyproject.toml`, `setup.py`, `Pipfile`)
   * Node/TypeScript (`package.json`, `pnpm-lock.yaml`, `tsconfig.json`)
   * Rust (`Cargo.toml`), Go (`go.mod`), C++ (`CMakeLists.txt`), etc.
2. **Identify Testing & Verification Frameworks:**
   * e.g., `pytest`, `npm test`, `vitest`, `cargo test`, `go test`.
3. **Locate Key Components & Entry Points:**
   * Entry points (e.g., `main.py`, `index.ts`, `src/`, `cmd/`).
   * Configs, environment templates (`.env.example`), and documentation.
4. **Inspect Git History & Current Status:**
   * Latest commits, branches, untracked files, and recent changes.

---

## STEP 2: Discovery Interview (Ask Before Writing)

Do NOT guess on a new/empty project. If the workspace is empty OR Step 1 left blanks (no stack, no entry point, no goal), STOP and ask the user these 6 questions first — then generate files from their answers:

1. **What is this project about?** (1–2 sentences: problem + who it's for)
2. **What do you want built first?** (immediate goal / MVP task)
3. **Tech stack preference?** (language, framework, DB — or "you decide")
4. **Rules / constraints?** (e.g. never delete logs, paper-test before live, no force-push)
5. **Preferences?** (coding style, communication brevity, test mandate)
6. **Scope guardrails?** (project name if different from folder, what's explicitly OUT of scope, how do we know v1 is done)

Rules:
- Ask only what's missing. If the repo already reveals stack/goal, ask just the gaps.
- Wait for answers. Then use them verbatim to populate `PROJECT_CONTEXT.md`, `MEMORY.md` (prefs + invariants), `AGENTS.md` (safety rules), and `ACTIVE_TASK.md` (epic + checklist).
- Never invent stack, rules, or goals for an empty project.

**Lazy-user fallback:** If the user replies "just go ahead", "skip", "you decide", or gives no answer:
- Proceed immediately with safe defaults (inferred stack or simplest standard stack, minimal safety rules, generic style).
- Mark every unknown as `TBD — to be discovered` in the generated files, never leave blanks.
- Record assumptions in `ACTIVE_TASK.md` under Key Decisions as `Assumed (pending user confirmation)`.
- Discover and overwrite TBDs as work progresses via the Continuous Evolution Protocol (Step 3 File 1 §4).

---

## STEP 3: Generate the Living Memory Suite

Create the following 6 standard files in the workspace root, populated with real information detected during Step 1.

---

### File 1: `AGENTS.md` (The Constitution & Operating Rules)
Create [`AGENTS.md`](file:///AGENTS.md) to serve as the universal operating manual loaded by any AI agent on boot:

```markdown
# 🤖 AGENTS.md — Universal Agent Operating Guidelines

Welcome, Agent. You are operating in an asynchronous, self-evolving, multi-model collaborative workspace.
Adhere strictly to the rules below.

## 1. Ground Rules & Safety Constraints
- **Preserve Documentation Integrity:** Do not delete or overwrite existing documentation without explicit direction.
- **Safety First:** Never execute irreversible, destructive, or financial order operations without user confirmation or a sandbox/paper verification step.
- **Zero Hallucination Verification:** Verify file paths and symbols using SITEMAP.md and read tools before making edits.

## 2. Navigation Protocol (Read SITEMAP.md First)
- Before grepping or blindly browsing large directories, consult `SITEMAP.md`.
- `SITEMAP.md` provides exact symbol line numbers (classes, methods, functions) and dependency call-graphs. Jump directly to target lines.

## 3. Project Commands Quick Reference
- **Run Development/Entry:** `[Insert primary run command, e.g. python main.py or npm run dev]`
- **Run Test Suite:** `[Insert test command, e.g. pytest or npm test]`
- **Generate / Update Sitemap:** `python scripts/generate_sitemap.py` (or project equivalent)

## 4. The Continuous Evolution & Memory Protocol (Mandatory on Every Turn)
You are part of an **alive, learning system**. You must actively record learnings:
1. **Read Memory First:** Consult `MEMORY.md` before starting any deep architecture or debugging turn.
2. **Gotcha / Bug Discovery:** Whenever you diagnose a non-obvious bug, edge case, or third-party API quirk, append it immediately to `MEMORY.md` under `## 💡 Project Learnings & Gotchas`.
3. **User Preference Capture:** Whenever the user expresses a preference (style, risk, workflow, tooling), log it immediately in `MEMORY.md` under `## 👤 User Preferences & Decisions`.
4. **Task Handover:** Before ending your turn or when approaching token/usage limits:
   - Check off completed steps in `ACTIVE_TASK.md` (`[x]`).
   - Mark the in-progress step (`[/]`).
   - Write the exact **Immediate Next Action** for the incoming agent.
5. **Change Logging:** Whenever code is modified, add a concise bullet to `CHANGELOG.md` and keep `SITEMAP.md` in sync.
```

---

### File 2: `MEMORY.md` (The Evolving Brain & Cognitive Ledger)
Create [`MEMORY.md`](file:///MEMORY.md) to preserve institutional knowledge, user preferences, API quirks, and proven patterns across sessions:

```markdown
# 🧠 MEMORY.md — Project Knowledge & Evolution Ledger

*This file is the persistent long-term memory of all AI agents working on this project. Read this file at the start of any deep debugging or architecture session to avoid repeating past mistakes.*

---

## 👤 User Preferences & Interaction Style
- **Coding Style:** [e.g., Clean modular code, type-annotated, explicit error handling]
- **Execution Policy:** [e.g., Always explain before executing; paper-test before live]
- **Communication:** [e.g., Concise technical summaries, provide clickable file links]

---

## 💡 Project Learnings & Gotchas (Hard-Won Knowledge)
*Record non-obvious bugs, external API quirks, timing issues, and library behaviors discovered during development.*
- **[Gotcha 1 - Component/Module]:** [What happened, why it broke, and the permanent rule/solution]
- **[Gotcha 2 - External Service/API]:** [e.g., WebSocket disconnects if no ticks sent before market open]

---

## 🛡️ Architectural Invariants (Do NOT Break)
*Rules and invariants that must never be violated when modifying code.*
- [Invariant 1]
- [Invariant 2]

---

## 📈 Evolution Log (Cognitive Milestones)
- **YYYY-MM-DD:** [Milestone 1 — e.g., Initialized FirstSpark]
```

---

### File 3: `PROJECT_CONTEXT.md` (The High-Level Architecture Map)
Create [`PROJECT_CONTEXT.md`](file:///PROJECT_CONTEXT.md) containing the architectural ground truth of the repository:

```markdown
# 🗺️ PROJECT_CONTEXT.md — Architectural Knowledge Base

## 1. System Overview & Core Purpose
- **Project Name:** [Detected Project Name]
- **Core Purpose:** [Concise 2-sentence summary of what this project does and its target domain]
- **Primary Tech Stack:** [Languages, frameworks, key libraries, databases, broker/external APIs]

## 2. Directory & Module Map
| Directory / File | Core Responsibility | Key Entry Points |
| :--- | :--- | :--- |
| `[dir1/]` | [Explanation] | `[key_file.ext]` |
| `[dir2/]` | [Explanation] | `[key_file.ext]` |

## 3. Data Pipelines & Lifecycle Architecture
[Provide a clear text or Mermaid diagram explaining how data, requests, or events flow through the system from entry point to execution/output.]

## 4. Key Domain Terminology & Concepts
- **[Concept 1]:** [Definition]
- **[Concept 2]:** [Definition]
```

---

### File 4: `SITEMAP.md` (The Symbol & Dependency Graph — LLM-Native Code Map)
Create [`SITEMAP.md`](file:///SITEMAP.md) as the machine-readable symbol map that replaces external tools like Graphify for LLM navigation:

```markdown
# 🗺️ SITEMAP.md — Codebase Symbol & Dependency Index

*This file provides a token-efficient AST symbol index and dependency graph. Agents MUST use this file to locate classes, functions, and call chains with exact line numbers without running blind searches.*

---

## 🏗️ Core Architecture Hubs (High Centrality Modules)
*Modules imported by multiple components — edit with extreme caution.*
- `[core/engine.py]` (Central orchestrator — depends on `scheduler`, `state_manager`, `order_manager`)
- `[config/config_loader.py]` (Global configuration singleton)

---

## 📦 Module Symbol Index & Call Graphs

### `[module_dir/component.py]` (L1–L250)
- **Imports:** `[dependency_a]`, `[dependency_b]`
- **Classes:**
  - `ClassName` (L20–L180):
    - `method_one(param: type)` -> `return_type` (L35)
      - Calls: `other_module.function_call()` (L42)
    - `method_two()` -> `None` (L80)
- **Functions:**
  - `standalone_helper(x: float)` -> `float` (L190–L240)
```

---

### File 5: `ACTIVE_TASK.md` (The Relay Baton for Seamless Handovers)
Create [`ACTIVE_TASK.md`](file:///ACTIVE_TASK.md) as the live operational state tracker:

```markdown
# ⚡ ACTIVE_TASK.md — Working Memory & Handover Baton

## 🎯 Current Epic / Goal
**Title:** [e.g., Project Initialization / Core Feature Implementation]
- **Current Status:** [INITIALIZED | IN_PROGRESS | BLOCKED | COMPLETED]
- **Active Lead Model:** [Name of the model writing this, e.g., Gemini / Claude / GPT]
- **Timestamp:** [YYYY-MM-DD HH:MM]

---

## 📋 Execution Checklist
- [x] Phase 0: Workspace Reconnaissance & FirstSpark Initialization
- [/] Phase 1: [First Functional Task / Baseline Setup]
- [ ] Phase 2: [Next Functional Task]
- [ ] Phase 3: [Verification & Integration Testing]

---

## 🧠 Key Decisions & Blockers
- **Decisions Recorded:** [Document architectural choices made so the next model doesn't re-litigate them]
- **Current Blockers:** [None, or specific issues requiring user input]

---

## 🏃 Immediate Next Action for Incoming Agent
> **INCOMING AGENT READ THIS:** You are picking up the baton. Do NOT ask the user what to do.
> Perform this exact next step immediately:
> 
> **Action:** [Specific file to open, line to inspect, command to run, or function to code]
```

---

### File 6: `CHANGELOG.md` (The Historical Audit Trail)
Create [`CHANGELOG.md`](file:///CHANGELOG.md) following the [Keep a Changelog](https://keepachangelog.com/) standard:

```markdown
# 📜 CHANGELOG

All notable changes to this project will be documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]
### Added
- Project FirstSpark initialized (`AGENTS.md`, `MEMORY.md`, `PROJECT_CONTEXT.md`, `SITEMAP.md`, `ACTIVE_TASK.md`, `CHANGELOG.md`).

## [Baseline] - YYYY-MM-DD
### Added
- Initial project scaffolding and existing codebase baseline.
```

---

## STEP 4: Setup On-Demand Agent Skills & Sitemap Generator

1. **Create Sitemap Generator Script:**
   Provide a lightweight, zero-dependency AST parser script (e.g. `scripts/generate_sitemap.py` for Python or equivalent for other stacks) that traverses the repository, extracts classes, functions, and imports, and updates `SITEMAP.md` automatically.

2. **Create Modular Specialist Skills:**
   ```
   .agents/
   └── skills/
       ├── generate_sitemap/
       │   └── SKILL.md
       └── test_and_verify/
           └── SKILL.md
   ```

---

## STEP 5: Handover Verification

Once all files are created:
1. Verify clean file creation and valid Markdown syntax.
2. Present a concise summary to the user confirming the alive coordination framework is operational.
3. Update `ACTIVE_TASK.md` with the first real coding/feature objective of the project.
