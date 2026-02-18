# Solve Everything — Agent Skill

A cross-platform AI agent skill for the [Solve Everything](https://www.solveeverything.org) framework by Dr. Alexander D. Wissner-Gross and Dr. Peter H. Diamandis.

**Solve Everything** is a comprehensive blueprint for achieving abundance by 2035 through AI-driven Moonshots. This skill gives any AI agent structured access to the full framework — 140 glossary terms, 9 Industrial Intelligence Stack layers, the L0-L5 Maturation Curve, 15 Moonshots, 5 Institutional Primitives, the Abundance Flywheel, typed relationship graphs, stakeholder playbooks for 15 roles, and more.

This skill follows the [Agent Skills](https://agentskills.io) open standard and works across multiple platforms.

## What's Inside

```
solve-everything/
├── SKILL.md                        # Skill definition (165 lines)
├── references/
│   ├── framework.json              # Complete structured framework (98 KB)
│   ├── workflows.md                # 5 guided workflow procedures
│   └── output-templates.md         # Formatted report templates
├── README.md
└── LICENSE
```

**Context budget:** ~33K tokens for conversational use, ~38K for full workflow with templates. Leaves 80%+ of a 200K context window free for reasoning.

## Install

### Claude Code

```bash
# Personal (available in all your projects)
git clone https://github.com/interplanetarychris/solve-everything.git ~/.claude/skills/solve-everything

# Project-level (shared via version control)
git clone https://github.com/interplanetarychris/solve-everything.git .claude/skills/solve-everything
```

### OpenAI Codex CLI

```bash
git clone https://github.com/interplanetarychris/solve-everything.git .agents/skills/solve-everything
```

### Google Gemini CLI

```bash
# Workspace-level
git clone https://github.com/interplanetarychris/solve-everything.git .gemini/skills/solve-everything

# Or using the cross-platform path
git clone https://github.com/interplanetarychris/solve-everything.git .agents/skills/solve-everything
```

### Any Agent (Manual)

Download the [latest release](https://github.com/interplanetarychris/solve-everything/releases) and place the `solve-everything/` directory in your agent's skill discovery path.

### Direct JSON Access

If your agent doesn't support skills but can load context, the structured framework JSON is available directly:

```
https://www.solveeverything.org/solve_everything_agent.json
```

This single file (~31K tokens) contains the complete framework and can be loaded into any LLM context window.

## Usage

Once installed, the skill activates when you ask your agent about:

- Strategic analysis through an abundance lens
- Mapping projects to the Industrial Intelligence Stack or Maturation Curve
- Moonshot alignment for your work
- Designing institutions, prizes, or policies
- Role-specific action plans (CEO, mayor, researcher, investor, etc.)
- Any topic involving "solve everything," "abundance framework," or "moonshots"

### Example Prompts

**Strategic Assessment:**
> "Analyze my renewable energy startup through the Solve Everything framework. Where are we on the maturation curve and which moonshots are we adjacent to?"

**Institutional Design:**
> "I'm designing an XPRIZE for ocean health. Help me structure it using the institutional primitives and abundance flywheel."

**Stakeholder Playbook:**
> "I'm a city mayor. What should I be doing about AI in the next 90 days according to this framework?"

**Maturation Audit:**
> "Where is construction on the L0-L5 maturation curve? What would it take to advance to the next level?"

## Guided Workflows

The skill includes five structured workflows that produce formatted deliverables:

| Workflow | Output |
|---|---|
| **Strategic Assessment** | Full analysis with framework mapping, gap analysis, and action plan |
| **Maturation Audit** | Domain-by-domain L0-L5 scoring with evidence and advancement criteria |
| **Moonshot Alignment** | Which moonshots connect to your work, benchmark gaps, spillover effects |
| **Institutional Design** | Canvas for prizes, programs, or policies using the 5 primitives |
| **Stakeholder Action Plan** | Role-specific 90-day / 6-month / 1-year plan with dependencies |

## About the Framework

Solve Everything argues that intelligence is becoming the universal solvent for scarcity. Every major human problem — energy, health, food, education, housing, security — can be reframed as an intelligence problem, and AI is making intelligence abundant.

The framework provides:

- **Industrial Intelligence Stack** — 9 layers from raw intelligence to realized abundance
- **Maturation Curve** — L0 through L5 progression for any domain
- **15 Moonshots** — specific missions with benchmarks, milestones, and guardrails
- **Abundance Flywheel** — the self-reinforcing cycle that converts intelligence to abundance
- **Solution Wavefront** — how solutions emerge, scale, and normalize
- **Institutional Primitives** — 5 building blocks for abundance-oriented institutions
- **Failure Modes** — systemic risks with specific counter-designs
- **Stakeholder Playbooks** — concrete actions for 15 roles at three time horizons
- **Relationship Graph** — 42 typed edges (unlocks, requires, counters, measured_by) connecting concepts

Read the full framework at [solveeverything.org](https://www.solveeverything.org).

## Contributing

This skill is a community companion to the Solve Everything framework. Contributions are welcome — whether that's improving workflow guides, adding new output templates, refining the framework JSON as the source material evolves, or sharing how you've applied the framework in your own domain.

## License

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (Creative Commons Attribution 4.0 International).

You are free to share, adapt, and build upon this material for any purpose, including commercial use, as long as you give appropriate credit.

**Attribution:** The Solve Everything framework is by [Dr. Alexander D. Wissner-Gross](https://www.alexwg.org/) and [Dr. Peter H. Diamandis](https://grokipedia.com/page/Peter_Diamandis). This agent skill was created as a community companion to make the framework accessible to AI agents.

## Acknowledgments

- **Dr. Alexander D. Wissner-Gross** and **Dr. Peter H. Diamandis** for creating the Solve Everything framework
- Built using the [Agent Skills](https://agentskills.io) open standard
