# Stress Test Skill

A structured failure-first review skill that helps teams identify likely breakdowns, hidden assumptions, organizational risks, and prevention opportunities before major commitments. This skill is inspired by Dr. Gary Klein's "Premortem" concept, but takes it much further into a forced ranking/commitment behavior. It also asks questions like “How do projects like these usually fail?.” Ultimately, this skill will feed a "Risk Burndown" skill.

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

The goal is to make plans harder to break before teams commit to them publicly, or at the very least identify the greatest potantials for failure in order to tackle them early before they cause delay to the project.

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

## Templates

Quick-start templates are available in:

```text
templates/
```

Start with:

```text
templates/quick-start-template.md
```

Additional templates may be added over time for:
- release planning
- organizational change
- strategic initiatives
- AI rollouts
- operational migrations

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
