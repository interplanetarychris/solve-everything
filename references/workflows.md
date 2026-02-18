# Solve Everything — Workflow Guides

Detailed instructions for each workflow. The SKILL.md routes you here based on user intent.

## Table of Contents

1. [Strategic Assessment](#strategic-assessment)
2. [Maturation Audit](#maturation-audit)
3. [Moonshot Alignment](#moonshot-alignment)
4. [Institutional Design](#institutional-design)
5. [Stakeholder Action Plan](#stakeholder-action-plan)

---

## Strategic Assessment

**When to use:** The user has a project, company, product, or initiative and wants to
understand how it fits within the Solve Everything framework. This is the most common
and most comprehensive workflow.

**Example prompts:**
- "Analyze my startup through the Solve Everything lens"
- "How does QuoteWise fit into the abundance framework?"
- "What's my strategic position in the intelligence economy?"

### Procedure

**Phase 1 — Discovery (ask the user)**

Gather enough context to do a meaningful analysis. You need to understand:

1. What the project/company does (core value proposition)
2. Who it serves (customers, beneficiaries, stakeholders)
3. What stage it's at (idea, prototype, growth, mature)
4. What the user's role is (founder, advisor, employee, investor)
5. What specific strategic questions they have

Don't require all of this upfront — start with what they give you and ask follow-ups
as needed. Many users will drop you into the middle ("here's my company, analyze it")
and that's fine.

**Phase 2 — Framework Mapping**

Work through each framework dimension systematically:

1. **Moonshot Adjacency** — scan all 15 moonshots in `moonshots`. For each one, ask:
   does this project contribute to, depend on, or benefit from this moonshot? Rate
   adjacency as primary (directly advancing), secondary (enabling or benefiting), or
   none. Most projects will be primary on 1-2 and secondary on 2-4.

2. **Stack Position** — map the project onto the 9-layer `industrial_intelligence_stack`.
   Which layers does it operate in? Which does it depend on but not control? Where are
   the gaps between layers it controls and layers it needs?

3. **Maturation Level** — assess the domain's current L0-L5 level using
   `maturation_curve.levels`. Look at the transition criteria between the current level
   and the next. What would need to be true for the domain to advance?

4. **Flywheel Engagement** — where does the project enter the `abundance_flywheel`?
   Which of the 5 steps does it directly power? Is the flywheel spinning or stalled?

5. **Wavefront Position** — which phase of the `solution_wavefront` is the project in?
   Emerging, scaling, or normalized?

**Phase 3 — Gap and Risk Analysis**

1. **Relationship Tracing** — use `relationships.requires` to check prerequisites.
   Is the project assuming something is in place that isn't? Use `relationships.unlocks`
   to identify downstream impact the user might not be seeing.

2. **Failure Mode Scan** — walk through each entry in `failure_modes`. For each one,
   assess: is this project exposed to this risk? If yes, check the `countered_by` field
   and assess whether the counter-design is present in the user's approach.

3. **Anti-Pattern Check** — review `companion.patterns_and_antipatterns`. Flag any
   anti-patterns the project's current approach might be falling into.

**Phase 4 — Synthesis and Recommendations**

Bring everything together into a clear strategic picture:

1. **Position Summary** — where the project sits across all framework dimensions
2. **Strengths** — framework-aligned elements that create leverage
3. **Gaps** — missing prerequisites, unaddressed failure modes, anti-patterns
4. **Opportunities** — unlocks the project enables, adjacent moonshots to lean into
5. **Action Items** — concrete next steps, ideally mapped to stakeholder playbook timeframes

If the user wants a formatted deliverable, use the Strategic Assessment Report template
from `references/output-templates.md`.

---

## Maturation Audit

**When to use:** The user wants to understand where a domain, industry, or capability
sits on the L0-L5 Maturation Curve and what it takes to advance.

**Example prompts:**
- "Where is construction on the maturation curve?"
- "How mature is AI in healthcare right now?"
- "What would it take to get education from L2 to L3?"

### Procedure

1. **Identify the domain** — clarify what's being assessed. It might be an industry
   (construction), a capability (autonomous vehicles), or a specific application
   (AI-assisted drug discovery).

2. **Score current level** — for each maturation level in `maturation_curve.levels`,
   assess whether the domain has reached it. Use real-world evidence where possible.
   The levels are cumulative — you can't be L3 without having passed through L1 and L2.

3. **Identify the transition edge** — the boundary between current level and next level
   is where the interesting analysis lives. What specific criteria from the next level
   are unmet? What would need to change?

4. **Map blockers to framework** — use `relationships.requires` to identify what the
   next maturation level depends on. Check `failure_modes` for systemic risks that could
   prevent advancement. Look at `institutional_primitives` for structural changes needed.

5. **Benchmark against moonshots** — which moonshots would accelerate this domain's
   maturation? Check `moonshots` for relevant missions and their benchmarks/milestones.

6. **Produce scorecard** — use the Maturation Scorecard template if the user wants
   a formatted output.

---

## Moonshot Alignment

**When to use:** The user wants to understand which of the 15 Moonshots their work
connects to, and how to strengthen that alignment.

**Example prompts:**
- "Which moonshots does my renewable energy startup align with?"
- "How can I position my work closer to a specific moonshot?"
- "What's the spillover from Moonshot 7 into my domain?"

### Procedure

1. **Scan all 15 moonshots** — for each moonshot in `moonshots`, evaluate:
   - Direct contribution (the project advances this moonshot's mission)
   - Enabling contribution (the project builds infrastructure this moonshot needs)
   - Spillover benefit (achieving this moonshot would benefit the project)

2. **Deep-dive primary alignments** — for the 1-3 moonshots with strongest alignment:
   - Compare the project against the moonshot's `benchmarks` and `milestones`
   - Check `how_ai_solves` — is the project using these approaches?
   - Review `guardrails` — is the project respecting these constraints?
   - Map `spillover` effects — what else does this moonshot unlock?

3. **Trace the graph** — use `relationships.unlocks` to find indirect connections.
   A project might not directly align with a moonshot but could unlock something
   that does.

4. **Identify gaps** — where is the project falling short of moonshot benchmarks?
   What capabilities or partnerships would close the gap?

5. **Produce brief** — use the Moonshot Alignment Brief template if requested.

---

## Institutional Design

**When to use:** The user is designing a prize, program, policy, organization, or
institutional mechanism and wants to ground it in abundance principles.

**Example prompts:**
- "Help me design an XPRIZE for ocean health"
- "How should I structure this government AI program?"
- "Design a prize that incentivizes the right behavior"
- "What institutional primitives should this foundation adopt?"

### Procedure

1. **Clarify the design challenge** — what institution is being designed? What outcome
   should it produce? Who are the stakeholders?

2. **Map to Institutional Primitives** — review all 5 entries in `institutional_primitives`.
   Which primitives should this institution embody? Most well-designed institutions
   engage at least 3 of the 5.

3. **Apply the Abundance Flywheel** — how does this institution fit into the
   `abundance_flywheel`? Does it accelerate the cycle or just sit within one step?
   The best institutional designs create self-reinforcing loops.

4. **Check the Seven Great Conversions** — review `seven_great_conversions`. Which
   conversions does this institution advance? Design choices should actively push
   toward the "to" side of each relevant conversion.

5. **Failure-proof the design** — for each `failure_modes` entry, ask: could this
   institution accidentally trigger or amplify this failure mode? If yes, incorporate
   the `countered_by` design into the institutional structure.

6. **Define success metrics** — use `economic_dashboard` to select appropriate
   measurement frameworks. New institutions should measure what matters, not just
   what's easy to count.

7. **Assign stakeholder roles** — use `stakeholder_playbooks` to identify which
   roles need to be engaged and what each should contribute.

8. **Produce canvas** — use the Institutional Design Canvas template if the user
   wants a structured output.

---

## Stakeholder Action Plan

**When to use:** The user has a specific role and wants to know what concrete actions
the framework recommends for that role.

**Example prompts:**
- "I'm a city mayor — what should I do about AI?"
- "What's the 90-day plan for a healthcare CEO?"
- "I'm a researcher — how do I contribute to abundance?"

### Procedure

1. **Identify the role** — match to one of the 15 roles in `stakeholder_playbooks`.
   If the user's role doesn't match exactly, find the closest fit and note the adaptation.

2. **Pull the playbook** — extract all actions for that role, organized by timeframe
   (90-day, 6-month, 1-year).

3. **Contextualize** — adapt the generic playbook to the user's specific situation.
   A mayor of a 50,000-person city has different resources than a mayor of 5 million.
   A startup CEO has different leverage than a Fortune 500 CEO.

4. **Add dependencies** — use `relationships.requires` to flag prerequisites for the
   recommended actions. If an action requires something the user doesn't have, note it
   and suggest how to get it.

5. **Connect to moonshots** — which moonshots does this role most directly contribute to?
   Help the user see their work as part of the larger picture.

6. **Produce action plan** — use the Stakeholder Action Plan template if the user
   wants a formatted deliverable.
