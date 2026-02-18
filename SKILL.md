---
name: solve-everything
description: >
  Strategic analysis framework based on "Solve Everything" by Dr. Alexander D. Wissner-Gross
  and Dr. Peter H. Diamandis — a blueprint for achieving abundance by 2035 through AI-driven
  Moonshots. Use this skill whenever the user wants to: analyze a project, company, or
  initiative through an abundance lens; generate a strategic assessment, maturation audit,
  or moonshot alignment report; map work to the Industrial Intelligence Stack or L0-L5
  Maturation Curve; design institutions, prizes, policies, or challenges using abundance
  primitives; get role-specific action items from the Stakeholder Playbooks; identify
  failure modes and counter-designs; or apply structured strategic thinking rooted in the
  idea that intelligence can solve scarcity. Also trigger when the user mentions "abundance
  framework", "moonshots", "industrial intelligence", "maturation curve", "solve everything",
  "Diamandis", "Wissner-Gross", or asks for strategic analysis involving AI-driven
  transformation of any domain.
---

# Solve Everything — Strategic Thinking Framework

You are applying the Solve Everything framework: a structured model for how intelligence
(human + AI) can systematically solve humanity's greatest challenges and produce abundance
by 2035. Authored by Dr. Alexander D. Wissner-Gross and Dr. Peter H. Diamandis.
Published at solveeverything.org.

## Load the Framework Data

Before doing anything else, read the structured framework:

```
Read references/framework.json
```

This JSON is the framework's core knowledge base: 9 Industrial Intelligence Stack layers,
6 maturation levels (L0-L5), 15 Moonshots with benchmarks and guardrails, 5 Institutional
Primitives, the Abundance Flywheel, Solution Wavefront, Seven Great Conversions, failure
modes with counter-designs, a typed relationship graph (unlocks/requires), stakeholder
playbooks for 15 roles, and an economic dashboard.

Internalize the structure before responding. The `relationships` section is critical —
it contains the edges that let you trace how framework concepts connect to each other.

### On-Demand Files

Two supplementary files are loaded only when needed:

- **`references/glossary.json`** — 100+ term definitions. Load when you need precise
  definitions of framework vocabulary (e.g., a user asks "what is a Targeting Authority?").
- **`references/companion.json`** — Chapter summaries, 16 pattern/antipattern pairs,
  and a usage guide. Load when you need narrative context, the "why" behind the structures,
  or the pattern checklist for diagnostics.

## Core Thesis

Intelligence is becoming the universal solvent for scarcity. Every major human problem
— energy, health, food, education, housing, security — can be reframed as an intelligence
problem. AI is making intelligence abundant. This framework provides the vocabulary,
structures, and playbooks for navigating the transition from scarcity to abundance.

The framework is ambitious and optimistic by design. Abundance is achievable, not
inevitable — it requires deliberate institutional redesign, new metrics, safety
frameworks, and coordinated action. Maintain a constructive-but-rigorous tone: find
genuine pathways without hand-waving away real obstacles.

## The Analysis Method

When a user brings you anything — a project, company, initiative, policy, prize, or
question — help them see it through the Solve Everything lens using these steps:

### 1. Listen and Locate

Understand the user's context. Then place it in the framework:

- **Moonshot adjacency** — which of the 15 Moonshots does this touch? Most projects
  are primary on 1-2 and secondary on 2-4.
- **Maturation level** — where is the relevant domain on the L0-L5 curve? What would
  need to be true to advance to the next level?
- **Stack position** — which of the 9 Industrial Intelligence Stack layers are in play?
  Where are the gaps?

### 2. Trace Relationships

The `relationships` graph has typed edges. Use them:

- **unlocks** (11 edges) — what does this work enable downstream?
- **requires** (8 edges) — what prerequisites might be missing?
- **counters** (6 edges) — which failure modes does this address?
- **measured_by** (17 edges) — what metrics track success?

This graph traversal is what transforms a surface-level analysis into a structural one.

### 3. Check Patterns and Anti-Patterns

`companion.patterns_and_antipatterns` contains 16 paired patterns. Use them as a
diagnostic checklist. Common ones to watch for:

- Open infrastructure vs. proprietary lock-in
- Measure what matters vs. GDP-only thinking
- Institutional redesign vs. bolting AI onto legacy processes
- Safety by design vs. safety as afterthought

### 4. Scan Failure Modes

Walk through `failure_modes`. For any initiative, ask: which of these could derail it?
Each failure mode has a `countered_by` field pointing to the specific design that
neutralizes it. If the counter-design isn't present in the user's approach, flag it.

### 5. Find the Playbook

If the user has a specific role, look up `stakeholder_playbooks`. There are 15 roles
with concrete actions at three timeframes: 90-day, 6-month, and 1-year. Adapt the
generic playbook to the user's specific scale and context.

### 6. Synthesize

Help the user see the full picture:

1. **Where they are** — maturation level, stack position, flywheel engagement
2. **Where they're going** — which moonshot(s), wavefront phase
3. **What's in the way** — failure modes, missing prerequisites, anti-patterns
4. **What to do next** — playbook actions, pattern alignment, institutional primitives
5. **How to measure** — economic dashboard metrics, framework-specific KPIs

## Guided Workflows and Output Templates

For users who want a structured deliverable (not just a conversation), this skill
includes detailed workflow guides and output templates:

```
Read references/workflows.md
```

This file contains step-by-step procedures for five named workflows:

| Workflow | When to Use |
|---|---|
| **Strategic Assessment** | Comprehensive analysis of a project/company/initiative |
| **Maturation Audit** | Where a domain sits on L0-L5 and what advances it |
| **Moonshot Alignment** | Which moonshots connect to the user's work and how |
| **Institutional Design** | Designing prizes, programs, policies, or organizations |
| **Stakeholder Action Plan** | Role-specific actions at 90-day, 6-month, 1-year horizons |

Each workflow includes discovery questions to ask, analysis phases to follow, and
synthesis guidance. When using a workflow, also load the output templates:

```
Read references/output-templates.md
```

This provides structured report formats (markdown with tables) for each workflow.
Use these when the user wants a deliverable they can share, present, or iterate on.

Not every interaction needs a formal workflow — often the 6-step analysis method above
is exactly right for exploratory conversation. Use the workflows and templates when
the user's intent calls for something structured.

## Framework Vocabulary

Use the framework's 100+ term glossary precisely. Terms like "Industrial Intelligence
Stack," "Solution Wavefront," "Abundance Flywheel," and "Institutional Primitives"
have specific definitions — load `references/glossary.json` when you need them. This
shared vocabulary is one of the framework's most valuable features — it gives diverse
stakeholders a common language for talking about the intelligence-to-abundance transition.

## Sources

- Framework: https://www.solveeverything.org
- Structured JSON: https://www.solveeverything.org/solve_everything_agent.json
- Agent Skills standard: https://agentskills.io

## Cross-Platform Compatibility

This skill follows the Agent Skills open standard. It works with Claude Code, OpenAI
Codex CLI, Google Gemini CLI, and any agent platform that supports the standard. The
core framework JSON (~20K tokens) loads in a single read; glossary and companion
narrative are in separate files (~5K and ~6K tokens) loaded on demand.
