# Risk Reduction Skill

A structured risk-reduction skill that transforms Stress Test findings into a prioritized mitigation backlog.

Most organizations are reasonably good at identifying risks.

Many are less effective at deciding:

* Which risks deserve action first
* Which risks are simply expected conditions
* Which mitigation activities provide the greatest reduction in project risk
* How much risk can be removed before execution begins

This skill focuses on reducing risk rather than documenting it.

---

# Relationship to Stress Test

This skill is designed to be used immediately after a Stress Test.

Workflow:

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

> Which failures are worth spending effort to prevent right now?

---

# When to Use This Skill

Use this skill when:

* A Stress Test has already been completed
* Project risks have already been identified
* Leadership needs prioritization rather than additional analysis
* Teams need mitigation activities
* Execution is approaching
* Delivery confidence needs improvement

Good candidates include:

* Release planning
* AI adoption initiatives
* Jira migrations
* Organizational changes
* Platform migrations
* Strategic initiatives
* Portfolio transformations
* Operational improvements

---

# Quick Start

Run a Stress Test first.

Then paste the resulting failure modes and ask:

```text
Run Risk Reduction on these Stress Test findings.
```

or

```text
Create a mitigation backlog from these failure modes.
```

or

```text
Which of these risks should we reduce first?
```

---

# What This Skill Produces

## Expected Conditions

Items with likelihood greater than 50%.

These are not treated as risks.

They should be:

* Planned for
* Staffed for
* Scheduled for
* Budgeted for

---

## Prioritized Risk Table

| Failure | Likelihood | Delay (Weeks) | Score | Likelihood Rationale | Self-Challenge | Mitigation Effort | Mitigations |
| ------- | ---------- | ------------- | ----- | -------------------- | -------------- | ----------------- | ----------- |

Sorted from highest score to lowest score.

---

## Mitigation Backlog

A prioritized list of mitigation work.

This is the primary output of the skill.

---

## Risk Reduction Summary

Provides:

* Total Risk Score Before Mitigation
* Estimated Risk Score After Mitigation
* Estimated Risk Reduction Percentage

---

# Scoring Method

Risk Score is calculated as:

```text
Likelihood × Delay Weeks
```

Example:

```text
40% × 6 weeks = 2.4
```

Higher scores indicate risks that deserve attention first.

---

# Expected Conditions vs Risks

A key distinction:

### Expected Conditions

Likelihood > 50%

Example:

```text
Users will require training on the new workflow.
Likelihood: 80%
```

This is not a risk.

It is part of the implementation plan.

### Risks

Likelihood ≤ 50%

Example:

```text
Migration automation may fail.
Likelihood: 35%
```

This remains a risk and should be evaluated.

---

# Templates

Quick-start templates should be placed in:

```text
templates/
```

Suggested first template:

```text
templates/risk-reduction-followup.md
```

---

# Skill Location

```text
skills/risk-reduction/SKILL.md
```

---

# Intended Usage

This skill is designed for:

* Engineering leadership
* Product leadership
* Program management
* Release planning
* Agile coaching
* Portfolio planning
* Organizational change initiatives

The objective is not to maintain a risk register.

The objective is to reduce the probability and impact of project failure before execution begins.
