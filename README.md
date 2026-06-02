# Stress Test Skill

A structured failure-first review skill that helps teams identify likely breakdowns, hidden assumptions, organizational risks, and prevention opportunities before major commitments.

The skill is inspired by Dr. Gary Klein's Premortem technique but extends it by forcing prioritization, ranking likely outcomes, identifying hidden assumptions, and grounding recommendations in historical patterns and organizational realities.

The goal is not to criticize a plan.

The goal is to make the plan harder to break.

---

# Relationship to Risk Reduction

Stress Test is intended to be the first step in a two-skill workflow.

```text
Stress Test
    ↓
Potential Failures
    ↓
Risk Reduction
    ↓
Mitigation Backlog
    ↓
Project Execution
```

Stress Test answers:

> How does this fail?

Risk Reduction answers:

> Which failures should we spend effort preventing right now?

Stress Test identifies potential failure modes.

Risk Reduction converts those failure modes into prioritized mitigation work.

---

# Operating Modes

The skill supports two modes.

## Default Mode

Default Mode is the standard behavior.

Use it for:

* release reviews
* roadmap reviews
* AI adoption efforts
* organizational changes
* operational improvements
* strategic initiatives
* executive proposals

Default Mode:

* focuses on the 5-8 strongest failure modes
* prioritizes signal over completeness
* produces a concise decision-making artifact
* targets approximately 3-5 pages of output

This is the recommended mode for most situations.

---

## Deep Dive Mode

Deep Dive Mode is intended for:

* workshops
* executive planning sessions
* major strategic initiatives
* detailed investigation of a specific failure mode

Deep Dive Mode expands selected failure modes into fuller narratives, assumptions, warning signs, and prevention strategies.

Use this mode when detailed exploration is more important than brevity.

---

# When to Use This Skill

Use this skill when:

* the cost of being wrong is meaningful
* timelines are tight
* multiple teams are involved
* dependencies are unclear
* organizational coordination matters
* leadership visibility is high
* quality and delivery pressure are increasing
* AI acceleration may amplify existing process weaknesses

This skill works especially well when teams feel:

* something about this feels risky
* we may be missing something
* this looks good on paper, but...
* poke holes in this before we commit

---

# Quick Start

Ask Claude or another compatible assistant:

```text
Stress test this:

Plan:
[What are we doing?]

Audience / stakeholders:
[Who is affected?]

Success criteria:
[What would make this successful?]

Constraints:
[Deadlines, staffing, dependencies, technical limits, political realities, quality expectations.]

Known concerns:
[What already feels risky, unclear, controversial, or assumed?]
```

Users do not need perfect formatting.

The skill should infer what it can and ask only for the most important missing information.

---

# Rendered Examples

View the formatted HTML examples here:

- [Jira Consolidation Stress Test](https://ahinek.github.io/stress-test-skill/examples/jira-consolidation-stress-test.html)
- [Jira Consolidation Risk Reduction](https://ahinek.github.io/stress-test-skill/examples/jira-consolidation-risk-reduction.html)

# Invocation Examples

## Default Mode

```text
Stress test this release plan before we commit to the date.
```

```text
Stress test this AI rollout for engineering teams.
```

```text
Find the blind spots in this organizational change proposal.
```

```text
What could kill this launch plan?
```

---

## Deep Dive Mode

```text
Stress test this in deep-dive mode.
```

```text
Run a full stress test on this strategic initiative.
```

```text
Expand failure mode #3.
```

```text
Give me the detailed version.
```

---

# What the Skill Produces

The skill produces:

* Most Likely Failure
* Most Dangerous Failure
* Cheapest Failure to Prevent
* Hidden Assumption
* Base Rate Analysis
* Organizational Failure Analysis
* Revised Plan Recommendations
* Pre-Launch Checklist
* Early Warning Indicators

The skill forces prioritization rather than treating all risks as equally important.

---

# Organizational Risks It Evaluates

In addition to technical and delivery risks, the skill evaluates:

* unclear ownership
* dependency friction
* overloaded teams
* conflicting incentives
* metrics distortion
* communication breakdowns
* hidden operational work
* unrealistic coordination assumptions
* AI amplifying unstable processes
* timeline pressure overwhelming quality controls

---

# Templates

Quick-start templates are available in:

```text
templates/
```

Start with:

```text
templates/quick-start-template.md
```

Additional templates may be added over time for:

* release planning
* organizational change
* strategic initiatives
* AI rollouts
* operational migrations

---

# Skill Location

```text
skills/stress-test/SKILL.md
```

---

# Intended Usage

This skill is designed for internal organizational use with Claude and compatible AI assistants.

It is intended to support:

* engineering leadership
* product leadership
* program management
* release planning
* Agile coaching
* organizational change planning
* cross-functional delivery reviews

---

# Philosophy

A review asks:

> Is this a good plan?

A council asks:

> What would different perspectives say?

A Stress Test asks:

> This failed. Why?

That framing changes the quality of the analysis dramatically.

