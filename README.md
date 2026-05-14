# Stress Test Skill

A structured failure-first review skill that helps teams identify likely breakdowns, hidden assumptions, organizational risks, and prevention opportunities before major commitments.

This skill is intended for planning reviews involving:
- releases
- roadmap shifts
- AI rollouts
- organizational changes
- delivery commitments
- migrations
- strategic initiatives
- operational changes
- executive proposals

The goal is not to criticize plans for sport. The goal is to make plans harder to break before teams commit to them publicly.

---

# When to Use This Skill

Use this skill when:
- the cost of being wrong is meaningful
- timelines are tight
- multiple teams are involved
- dependencies are unclear
- organizational coordination matters
- leadership visibility is high
- quality and delivery pressure are both increasing
- AI acceleration may amplify existing process weaknesses

This skill works especially well when teams feel:
- “something about this feels risky”
- “we may be missing something”
- “this looks good on paper, but…”
- “poke holes in this before we commit”

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

Users do not need perfect formatting. The skill should infer what it can and ask only for the most important missing information.

---

# Lightweight Invocation Examples

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
Poke holes in this roadmap shift before I share it with leadership.
```

```text
What could kill this launch plan?
```

---

# Output Includes

The skill produces:

- Most likely failure
- Most dangerous failure
- Cheapest failure to prevent
- Hidden assumption
- Base-rate reasoning
- Organizational failure mode analysis
- Revised plan recommendations
- Pre-launch checklist
- Early warning indicators

The skill forces prioritization rather than treating all risks as equally important.

---

# Organizational Risks It Looks For

In addition to technical and delivery risks, the skill evaluates for:

- unclear ownership
- dependency friction
- overloaded teams
- conflicting incentives
- metrics distortion
- communication breakdowns
- hidden operational work
- unrealistic coordination assumptions
- AI amplifying unstable processes
- timeline pressure overwhelming quality controls

---

# Skill Location

```text
skills/stress-test/SKILL.md
```

---

# Intended Usage

This skill is designed for internal organizational use with Claude and compatible AI assistants.

It is intended to support:
- engineering leadership
- product leadership
- program management
- release planning
- Agile coaching
- organizational change planning
- cross-functional delivery reviews

---

# Philosophy

A normal review asks:
> “Is this a good plan?”

A stress test asks:
> “This failed six months from now. Why?”

That framing changes the quality of the analysis dramatically.
