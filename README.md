# Stress Test Skill

The **Stress Test Skill** is a structured failure-first reasoning framework for evaluating plans before major commitments are made.

Rather than asking whether a plan is good, the Stress Test assumes the plan has already failed and works backward to determine the most credible reasons why. This approach exposes hidden assumptions, organizational friction, weak signals, and preventable risks that conventional reviews often overlook.

The objective is not to criticize a plan.

The objective is to improve the plan before reality does.

---

# Cassandra Assessments

The primary output of the Stress Test Skill is a **Cassandra Assessment**.

A Cassandra Assessment identifies the most credible failure modes, hidden assumptions, and preventable risks associated with a proposed plan. Its purpose is not to predict the future with certainty, but to expose the most likely ways a plan could fail while there is still time to improve it.

The name comes from Cassandra of Greek mythology, who was granted the ability to foresee disasters but cursed to have her warnings ignored. A Cassandra Assessment is intended to surface credible warnings before resources are committed and while corrective action remains possible.

The **Stress Test Skill** is the reasoning process.

The **Cassandra Assessment** is the artifact it produces.

---

# Core Principles

Every Stress Test follows five principles.

## Assume Failure

Begin with the assumption that the plan has already failed and work backward to explain why.

## Commit to Conclusions

Prioritize findings by likelihood, impact, preventability, and decision value. Distinguish evidence from uncertainty, but avoid hiding behind "it depends."

## Be Specific

Focus on risks that are grounded in the actual plan, organization, stakeholders, and delivery context rather than generic observations.

## Be Actionable

Every significant finding should lead naturally to one or more changes that improve the plan.

## Be Concise

Prefer fewer, stronger findings over exhaustive analysis. Every item should earn its place by being likely, impactful, preventable, and decision-relevant.

---

# Relationship to Risk Reduction

The Stress Test Skill is intended to be the first step in a two-skill workflow.

```text
Stress Test
      ↓
Potential Failures
      ↓
Risk Reduction
      ↓
Mitigation Backlog
      ↓
Execution
```

The Stress Test identifies the most credible ways a plan could fail.

The Risk Reduction Skill converts those findings into a prioritized mitigation backlog.

---

# Operating Modes

## Default Mode

Default Mode is recommended for most situations.

Use it for:

* release reviews
* organizational initiatives
* operational improvements
* executive proposals
* delivery commitments
* first-pass risk analysis

Default Mode emphasizes:

* decision support over exhaustive analysis
* prioritization over completeness
* actionability over explanation
* concise, high-value findings

## Deep Dive Mode

Deep Dive Mode is intended for workshops, executive planning sessions, and detailed investigations of selected failure modes.

It extends the standard Cassandra Assessment with expanded failure narratives, assumptions, warning signs, and prevention strategies while preserving the same reasoning principles.

---

# When to Use This Skill

Use this skill when:

* meaningful decisions have not yet been finalized
* the cost of failure is significant
* the plan can still be changed
* multiple teams, organizations, or dependencies are involved

Typical applications include:

* product launches
* feature launches
* AI adoption initiatives
* organizational change
* platform or Jira migrations
* delivery commitments
* executive proposals
* strategic initiatives

Avoid using this skill for factual questions, editing requests, open-ended brainstorming, purely creative work, or decisions that are already irreversible.


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
# Invocation Examples
## Recommended Invocation
### Default Mode

```text
Stress test this plan.

## Plan

Consolidate multiple Jira workspaces into a single shared workspace.

## Stakeholders

Engineering
Product Management
QE
Release Management
Customer Support

## Success Criteria

- Minimal disruption
- Standardized workflows
- Improved reporting
- Shared governance

## Constraints

Migration must occur during active development.
No interruption to release planning.
Limited administrative resources.

## Known Concerns

Teams have customized workflows.
Some automation depends on existing project structures.

### Deep Dive Invocation

```text
Run a Deep Dive Stress Test.

Focus especially on:

- organizational resistance
- governance
- migration sequencing
- dependency management
- communication risks

Challenge every major assumption.
Identify the most likely organizational failure patterns.
```
The skill adapts to the amount of context provided. A single paragraph is often enough to begin. Additional detail improves the quality of the assessment but is not required.



---

# What a Cassandra Assessment Contains

A Cassandra Assessment contains:

* Most Likely Failure
* Most Dangerous Failure
* Cheapest Failure to Prevent
* Hidden Assumption
* Base Rate Analysis
* Organizational Failure Analysis
* Overall Assessment
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

# Rendered Examples

View the formatted HTML examples here (V2 examples coming soon):

- [Jira Consolidation Stress Test](https://ahinek.github.io/stress-test-skill/examples/jira-consolidation-stress-test.html)
- [Jira Consolidation Risk Reduction](https://ahinek.github.io/stress-test-skill/examples/jira-consolidation-risk-reduction.html)

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

Instead of asking:

> Is this a good plan?

Ask:

> If this plan failed six months from now, what would we wish we had seen today?

That question is the heart of the Stress Test Skill. It shifts the conversation away from defending the current plan and toward discovering the assumptions, risks, and decisions that are still within our power to change.

The purpose of a Cassandra Assessment is not to predict the future.

Its purpose is to improve decisions before commitments become expensive to reverse.


