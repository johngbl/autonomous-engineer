# Changelog

All notable changes to the Autonomous Engineer Meta-Skill are documented here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-08-13

### First Public Release

The complete Agentic Loop & Graph Engineering framework as a **single self-contained SKILL.md**.

**Motor (SKILL.md) — 9 Sections + 3 Appendices, fully self-contained:**
- Section I: Rigid Boundaries & Anti-Pattern Ban List (13 guardrails)
- Section II: Phase 0 — Discovery, Context Engineering & Zero-Prompt Auto-Provisioning
- Section III: Phase 1 — Specification, Layer Boundaries & Memory State
- Section IV: Phase 1.5 — Multi-Agent Persona Orchestration & Graph Engineering (G=V,E)
- Section V: Phase 2 — Repro-First TDD, Art Direction, Open Loop Floor & Gauntlet Protocol
- Section VI: Phase 3 — 3-Layer Evaluator, TextGrad 3-Block, Circuit Breaker
- Section VII: Phase 4 — Adversarial Audit, EDD, Procedural Memory, Graph Degradation
- Section VIII: Phase 5 — Definition of Done & Git Safety Lock
- Section IX: Factory Mode & Human Oversight Protocol
- Appendix A: Design Research Directives (agent actively searches current sources)
- Appendix B: Inline Templates (AGENTS.md, SPEC.md formats)
- Appendix C: Procedural Memory Format

**Key Capabilities:**
- Context Engineering with symbol-graph navigation and Context7/MCP anchoring
- Spec-Driven Development with full lifecycle (draft → approved → in_progress → verified → archived)
- 3-Layer Evaluator Pipeline (Linter → Types/Security → Tests/UI)
- TextGrad Failure Gradient Protocol (3-block structured capture + classification + recalibration)
- Strict TDD with Enforced Deletion Rule
- Graph Engineering Topology G=(V,E) with fan-out/fan-in and escalation threshold
- Gauntlet Protocol: Blind Visual Critic loop for high-fidelity UI tasks (max 8 iterations)
- Speculative Model Routing + Secondary Turn Ceiling
- Git Worktrees parallel orchestration + A2A Delta-Only protocol
- Ephemeral Micro-VM tiering (E2B/Daytona/Modal)
- Evals-Driven Development with golden dataset
- Inter-project Procedural Memory (~/.agents/procedural-memory.md)
- Human Comprehension Guardrail + Minimal Tool Surface
- Pre-Flight Checklist + Token Budget Ceiling
- Light/Dark Factory modes with Code Sampling Rule
- Open Loop Floor (anti-slop for subjective tasks)
- Cyclomatic Complexity Gate
- Verifier Primacy Principle
- Compound Error Mathematics anchor
- Graph Node Graceful Degradation
- Trigger Taxonomy (Event, Cron, Manual, Proactive)
- Untrusted Content Boundary + Guardrail Precedence (anti indirect prompt injection)
- Provisioning Trust Chain (verified sources only + transparency log)
- Proactive Registry Consultation Protocol (agent auto-researches by task type)
- Design Research Directives (no fixed URLs, agent searches current sources at runtime)

**Repository Structure:**
- `evals/` — Golden dataset (9 behavioral cases)
- `.github/workflows/evals.yml` — EDD CI Gate

**Installation:**
```bash
npx skills add johngbl/autonomous-engineer --yes --global
```

---

## Development History (Pre-Release)

<details>
<summary>Internal iterations leading to v1.0.0</summary>

### Iteration 4 (Graph Engineering)
- Added Graph Engineering Topology G=(V,E), escalation threshold, dynamic rubric generation
- Added delta-only A2A, trigger taxonomy, secondary turn ceiling
- Added graph node graceful degradation
- Expanded spec lifecycle with in_progress/verified states and auto-archiving

### Iteration 3 (Harness Hardening)
- Added Compound Error Mathematics, Human Comprehension Guardrail, Minimal Tool Surface
- Added MCP Resilience, Pre-Flight Checklist, Feedback Sensor Priority
- Added TextGrad 3-Block Structured Capture, Fixed vs Creator Loops, Token Budget Ceiling
- Added Gauntlet Protocol (Blind Visual Critic)

### Iteration 2 (Motor + Factory Architecture)
- Restructured into immutable motor + living registry + scaffolds + evals
- Added TextGrad, EDD lifecycle, Micro-VM tiering, inter-project memory
- Added Git Worktrees + A2A, Speculative Model Routing, MCP auto-provisioning
- Added Clarification Gate, Spec lifecycle states, Registry update protocol

### Iteration 1 (Original Manifesto)
- 8-section Senior Autonomous Engineering Manifesto
- Context Engineering, Spec-Driven Development, 3-Layer Evaluator Loop
- Strict TDD with Enforced Deletion Rule
- Anti-Slop Art Direction & Headless UI Verification
- Rigid Workspace Sandboxing & Git Safety Lock
- Multi-Agent Persona Orchestration
- Procedural Memory Distillation

</details>
