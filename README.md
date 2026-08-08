# 🚀 Autonomous Engineer — Agentic Loop & Graph Engineering Meta-Skill

![Version](https://img.shields.io/badge/version-1.0.0-blue) ![License](https://img.shields.io/badge/license-MIT-green) [![skills.sh](https://img.shields.io/badge/skills.sh-johngbl%2Fautonomous--engineer-black)](https://skills.sh/johngbl/autonomous-engineer)

> **The definitive transition from "Vibe Coding" & Prompt Engineering to Agentic Loop & Context Engineering.**
> A single, self-contained Meta-Skill that transforms coding agents into Staff/Principal-level autonomous software engineers. Works with Claude Code, Cursor, Zed, Codex, Cline, and 76+ more via [skills.sh](https://skills.sh).

---

## 💡 Why Does This Repository Exist?

Sending manual prompts turn-by-turn in chat UIs is an obsolete bottleneck. Modern AI-assisted software development requires **Context Engineering**, **Spec-Driven Development (SDD)**, and **Evaluator-Optimizer Loops**.

The **Autonomous Engineer** is a single self-contained SKILL.md that equips coding agents to:

1. **Execute Intelligent Ecosystem Provisioning:** Detect what is strictly necessary to execute and validate the task, and provision only that — using the project's own mechanisms and preferring existing resources over introducing anything new.
2. **Practice Minimalist Engineering:** Write minimal, performant, and clean production code by reusing existing codebase abstractions and native language/browser APIs.
3. **Enforce Spec-Driven Development (SDD):** Formulate structured `/specs/` with lifecycle states (`draft → approved → in_progress → verified → archived`) before modifying production code.
4. **Prevent API & Package Hallucinations:** Validate packages, schemas, and framework APIs against official documentation indices (Context7 / MCP / web search) before importing.
5. **Enforce Strict TDD with the Deletion Rule:** Require a failing test *prior* to writing production code. If production code is written first, the agent is forced to delete it and restart with the test.
6. **Eliminate AI Visual Slop:** Require intentional art direction via active research, and verify visual UI via headless browser screenshots rendered to disk.
7. **Run 3-Layer Evaluator-Optimizer Loops with TextGrad:** Execute automated validation pipelines (Linter → Types/Security → Tests/UI) with failure-gradient classification and plan recalibration, plus a 5-iteration Circuit Breaker.
8. **Execute the Gauntlet Protocol (Blind Visual Critic):** For high-fidelity UI tasks, decompose into micro-components and validate each with a blind critic that only sees rendered screenshots vs. a visual benchmark.
9. **Learn Across Projects via Procedural Memory:** Distill debugging lessons into `~/.agents/procedural-memory.md` (persistent, survives reinstalls), consulted before every non-trivial task.
10. **Guard Against Comprehension Debt:** Enforce the Human Comprehension Guardrail — code must remain reviewable by the team, not just pass CI.
11. **Minimize Tool Surface:** Inject only the tools strictly necessary per sub-task, reducing the error surface for wrong tool selection.
12. **Pre-Flight Viability Checks:** Answer 4 gate questions (harness strength, feedback speed, stop condition, workload) before entering any long autonomous loop.
13. **Orchestrate Graph Engineering Topologies:** Escalate from single loops to directed acyclic graphs of specialized agents (G = V, E) with fan-out/fan-in, delta-only communication, and graceful node degradation.
14. **Preserve Human Comprehension (Light/Dark Factory):** Default to Light Factory with natural-language summaries; Dark Factory requires explicit opt-in + mandatory Code Sampling (1 in 5 PRs human-reviewed).
15. **Treat External Content as Untrusted Data:** Enforce an Untrusted Content Boundary against indirect prompt injection, a Provisioning Trust Chain, and Guardrail Precedence.
16. **Deliver Invisible Agent Artifacts:** All agent state files (`AGENTS.md`, `.tmp/`, `specs/archive/`) are gitignored. The delivered project appears 100% human-authored.

---

## 🏗️ Repository Architecture

```
autonomous-engineer/
├── SKILL.md                  <- THE COMPLETE SKILL: fully self-contained
├── README.md
├── LICENSE                   <- MIT
├── CHANGELOG.md              <- Version traceability
├── .gitignore
└── .github/
    └── workflows/
        └── evals.yml         <- CI Gate: structural integrity checks
```

**Design Principle:** `SKILL.md` is a **single, self-contained file** (~430 lines) that includes everything the agent needs: the full protocol (9 sections), design research directives, inline templates (AGENTS.md, SPEC.md formats), and procedural memory format (3 appendices). No external files, no registry, no templates directory. The agent generates all artifacts at runtime from embedded specifications. Installation is trivial (1 file) and the skill works identically across all supported agents.

---

## 🔥 Core Pillars

| # | Pillar | Description |
|---|--------|-------------|
| 1 | **Context Engineering** | Targeted symbol-graph navigation, Context7/MCP/web-search doc anchoring, zero context rot |
| 2 | **Spec-Driven Development** | Lifecycle-managed specs with acceptance criteria before code |
| 3 | **3-Layer Evaluator + TextGrad** | Linter → Types/Security → Tests/UI, with 3-block failure-gradient capture and plan recalibration |
| 4 | **Strict TDD + Deletion Rule** | Failing test first or production code gets deleted |
| 5 | **Intelligent Provisioning** | Minimum Necessary Principle + Context-Aware Provisioning + Trust Chain logging |
| 6 | **Multi-Agent Orchestration** | 4 personas with speculative model routing + Git Worktrees + A2A delta-only protocol |
| 7 | **Gauntlet Protocol** | Blind Visual Critic loop for high-fidelity UI (max 8 iterations, WOWED/GAP verdicts) |
| 8 | **Procedural Memory** | Autonomous recognition + distillation to `~/.agents/procedural-memory.md`; consulted before debugging |
| 9 | **Ephemeral Environment Tiering** | Local sandbox default; micro-VM escalation for high-risk operations |
| 10 | **Rigid Workspace Sandboxing** | Ban on destructive git, unvetted scripts, secrets exposure |
| 11 | **Human Comprehension Guardrail** | Code must remain reviewable; green CI + black-box code = defect |
| 12 | **Minimal Tool Surface** | Only necessary tools per sub-task; persona toolsets scoped |
| 13 | **Pre-Flight + Token Budget** | 4 viability questions before loops; 3x token ceiling with escalation |
| 14 | **Graph Engineering (G=V,E)** | Multi-agent DAG topology with fan-out/fan-in, delta-only A2A, node isolation |
| 15 | **Escalation Threshold** | Explicit rules for when to go from single loop to graph (>300k tokens, parallel need) |
| 16 | **Light/Dark Factory + Code Sampling** | Human oversight by default; Dark Factory opt-in with 1-in-5 PR review mandate |
| 17 | **Open Loop Floor + Anti-Slop** | Mechanical validation floor for subjective tasks; max 3 iterations; prohibited generic patterns |
| 18 | **Agent Invisibility** | All agent artifacts gitignored; delivered project appears 100% human-authored |

---

## ⚙️ Execution Flow

```
                    [ User Requirement / Prompt ]
                                 │
                                 ▼
    ┌──────────────────────────────────────────────────────────┐
    │ PHASE 0: Context Engineering & Auto-Provisioning         │
    │ • Essential Tooling Setup + Git Bootstrap                 │
    │ • Proactive Research & Memory Consultation               │
    │ • Clarification Gate (max 3 questions if ambiguous)      │
    │ • Pre-Flight Checklist (4 viability questions)           │
    │ • Mode Routing + Factory Mode Determination              │
    └────────────────────────────┬─────────────────────────────┘
                                 │
     ┌───────────────────────────┼───────────────────────────┐
     ▼                           ▼                           ▼
[ Analysis Mode ]        [ Micro-Task Mode ]       [ Spec-Driven Mode ]
• Read-Only              • Point Edits < 5 min     • /specs/ + AGENTS.md
• Planning/Discussion    • Direct Solo Loop        • Multi-Agent Personas
• Zero Code Changes      • Local Verification      • Worktrees + A2A
                                                             │
                                                             ▼
                                                   ┌───────────────────┐
                                                   │ PHASE 2: TDD +    │
                                                   │ Art Direction +   │
                                                   │ Gauntlet Protocol │
                                                   └─────────┬─────────┘
                                                             │
                                                             ▼
                                                   ┌───────────────────┐
                                                   │ PHASE 3: 3-Layer  │
                                                   │ Evaluator +       │
                                                   │ TextGrad + CB     │
                                                   └─────────┬─────────┘
                                                             │
                                                             ▼
                                                   ┌───────────────────┐
                                                   │ PHASE 4-5: Audit, │
                                                   │ Memory, DoD &     │
                                                   │ LOCAL Commit Only │
                                                   └───────────────────┘
```

---

## 🛠️ Installation

```bash
npx skills add https://github.com/johngbl/autonomous-engineer --skill autonomous-engineer --yes --global
```

Requires only Node.js/npx (Windows, macOS, Linux). The [skills.sh](https://skills.sh) CLI detects your installed agents and installs the skill into each agent's global skills directory. Use `--copy` if symlinks are unsupported, or drop `--global` for a project-scoped install.

> Browse at [skills.sh/johngbl/autonomous-engineer](https://skills.sh/johngbl/autonomous-engineer/autonomous-engineer)

---

## 💻 Daily Usage Workflows

Trigger your agent using standard natural language requests. The protocol automatically routes the task to the appropriate architecture mode.

### Example 1: Complex Spec-Driven Feature (Orchestration Mode)
> **Prompt:** `create the feature: Multi-tenant authentication module with Role-Based Access Control (RBAC) and Stripe billing integration.`

The agent provisions essential tooling, generates `/specs/001-rbac-billing.md`, initializes state tracking in `./AGENTS.md`, executes strict TDD across domain boundaries, and validates through all 3 evaluation layers.

### Example 2: Repro-First Bug Fix (Maker-Checker Mode)
> **Prompt:** `fix the bug: Coupon discounts are applying twice when checking out with multi-item carts.`

The agent writes a unit test that reproduces the duplicate discount bug and confirms it **fails**. It then modifies the domain logic until the test passes without altering the test assertion.

### Example 3: Quick Point Edit (Micro-Task Mode)
> **Prompt:** `quick fix: Fix the padding-top alignment on the user table header.`

The agent identifies a low-scope edit, updates the targeted file, runs the local linter/type-checker, and completes the task in seconds without creating state tracking files.

### Example 4: Architecture Review (Analysis Mode)
> **Prompt:** `analyze the code: Audit the /packages/core module for potential N+1 database queries and type safety risks.`

The agent operates in read-only mode, inspects the symbol graph, and delivers a detailed diagnostic report in chat without making file mutations.

### Example 5: Planning From Scratch (Analysis Mode → Clarification Gate)
> **Prompt:** `I want to build a SaaS platform for freelance invoicing.`

The agent asks at most 3 targeted questions (stack, auth, deployment), waits for answers, then produces a spec for approval before writing any code.

### Example 6: High-Fidelity UI (Gauntlet Protocol)
> **Prompt:** `create the feature: Build the landing page to match this design. [screenshot attached]`

The agent decomposes the page into micro-components, assigns each to a developer sub-agent, and validates with blind critics that compare rendered screenshots against the benchmark until `WOWED`.

---

## 📊 Comparison: Vibe Coding vs. Loop Engineering

| Dimension | "Vibe Coding" / Chat Prompts | Autonomous Engineer |
| :--- | :--- | :--- |
| **Workflow Philosophy** | Prompt → Code → Hope | **Context → Reasoning → Validation → Code** |
| **Tool Provisioning** | Manual human installation | **Intelligent Provisioning** (minimum necessary, context-aware) |
| **Specification** | Vague chat prompts | **Spec-Driven Development** with lifecycle states |
| **TDD Enforcement** | Optional / Ignored by AI | **Strict TDD + Enforced Deletion Rule** |
| **Package Validation** | Prone to API hallucinations | **Context7 / MCP / Web Search Real-Time Validation** |
| **UI Verification** | "Trust me, it looks good" | **Headless Screenshots + Gauntlet Protocol (Blind Critics)** |
| **Validation Pipeline** | Single test check or manual | **3-Layer Evaluator + TextGrad Failure Gradients** |
| **Failure Handling** | Retry blindly or give up | **Gradient classification + plan recalibration + Circuit Breaker** |
| **Context Hygiene** | Dumps full files (Context Rot) | Symbol Graph & Bounded Line Range Inspections |
| **Safety & Git Rules** | Risk of destructive overwrites | **Workspace Sandboxing** (ban on `git push`, `reset --hard`) |
| **Cross-Project Learning** | None | **Procedural Memory** (`~/.agents/procedural-memory.md`) |
| **Execution Isolation** | Local terminal only | **Ephemeral Micro-VM Tiering** (E2B/Daytona/Modal) |
| **Parallel Execution** | Sequential only | **Git Worktrees + A2A Protocol + Graph G=(V,E)** |
| **Token Efficiency** | Full model for everything | **Speculative Model Routing + Turn Ceilings** |
| **Cognitive Safety** | Code becomes black-box over time | **Comprehension Guardrail + Minimal Tool Surface + Pre-Flight** |
| **Human Oversight** | Full manual review or none | **Light/Dark Factory** with Code Sampling Rule |
| **Project Invisibility** | Agent artifacts visible in git | **All agent files gitignored; appears 100% human-authored** |

---

## 📄 License

Distributed under the **MIT License**. Free to use, modify, and distribute for commercial and non-commercial projects.

---

<p align="center">
  <b>Developed for and by the Loop Engineering community.</b><br>
  <i>"Build the loop. Remain the engineer."</i>
</p>
