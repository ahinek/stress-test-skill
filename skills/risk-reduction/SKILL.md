---

name: risk-reduction
description: Convert stress-test failure modes into a prioritized mitigation backlog by estimating likelihood, schedule impact, mitigation effort, and overall risk reduction potential.
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Risk Reduction

## Purpose

This skill transforms Stress Test findings into a practical mitigation plan.

Stress Test identifies potential failures.

Risk Reduction determines:

* Which failures deserve action first
* Which issues are expected conditions rather than risks
* Which mitigation activities provide the greatest reduction in project risk
* How much overall project risk can be reduced before execution begins

The goal is not to create a risk register.

The goal is to reduce project risk before those failures occur.

---

## Relationship to Stress Test

This skill is intended to be used after a Stress Test.

Expected workflow:

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

Stress Test identifies possible future failures.

Risk Reduction converts those failures into actionable mitigation work.

---

## Expected Inputs

Preferred input:

* Output from the Stress Test skill

Acceptable inputs:

* Identified failure modes
* Project risks
* Project concerns
* Project plans with known issues

If Stress Test output is available, use it.

---

## Classification Rules

### Expected Conditions

Any item with likelihood greater than 50% should be classified as an Expected Condition.

Expected Conditions:

* Should be planned for
* Should be staffed for
* Should be scheduled for
* Should be budgeted for

Expected Conditions should not appear in the risk ranking table.

---

### Risks

Items with likelihood less than or equal to 50% remain risks.

Only risks are scored and prioritized.

---

## Likelihood Estimation

For every risk:

1. Estimate a likelihood percentage.
2. Explain the rationale.
3. Challenge the estimate.

### Likelihood Rationale

Base estimates on:

* Historical patterns
* Organizational dynamics
* Technical complexity
* Stakeholder behavior
* Comparable initiatives
* Known failure modes

Do not generate arbitrary percentages.

Every estimate must include reasoning.

### Self-Challenge

For each estimate answer:

> Why might this estimate be wrong?

The purpose is to avoid false precision and overconfidence.

The challenge should be concise and specific.

---

## Risk Scoring

For each risk estimate:

* Likelihood (%)
* Delay impact in weeks

Calculate:

```text
Risk Score = Likelihood × Delay Weeks
```

Example:

```text
40% × 6 weeks = 2.4
```

Use decimal values.

---

## Mitigation Effort

Estimate mitigation effort as:

* Low
* Medium
* High

Favor practical interventions.

Favor low-effort / high-impact mitigations when possible.

---

## Mitigation Recommendations

Provide exactly three mitigation recommendations per risk.

Recommendations must be:

* Concise
* Actionable
* Specific
* Realistic

Avoid generic advice.

Examples:

Good:

* Conduct migration pilot
* Assign dependency owner
* Establish rollback rehearsal

Bad:

* Improve communication
* Increase visibility
* Align stakeholders

---

## Output Format

Use standard GitHub-flavored markdown.

Do not use:

- ASCII tables
- Unicode box-drawing tables
- Terminal-rendered tables

Output should render cleanly in:

- GitHub
- GitLab
- Google Docs
- Markdown editors

---

# Risk Reduction Analysis

## Expected Conditions

Use a GitHub-flavored markdown table.

Do not use ASCII tables.

Do not use Unicode box-drawing tables.

Required format:

| Condition | Likelihood | Why This Is Expected |
|-----------|------------|----------------------|

Limit "Why This Is Expected" to a single sentence.

---

## Prioritized Risk Table

Use a GitHub-flavored markdown table.

Do not use ASCII tables.

Do not use Unicode box-drawing tables.

Required format:

| Failure | Likelihood | Delay (Weeks) | Score | Effort | Rationale |
|----------|------------|---------------|--------|--------|-----------|

Rules:

- Rationale must be one sentence maximum.
- Delay must represent expected schedule impact if the failure occurs.
- Score = Likelihood × Delay.
- Effort must be Low, Medium, or High.

Do not provide narrative explanations within the table.

---

## Mitigation Recommendations

Use a GitHub-flavored markdown table.

Do not use ASCII tables.

Do not use Unicode box-drawing tables.

Required format:

| Failure | Mitigations |
|----------|-------------|

Rules:

- Provide exactly three mitigation bullets.
- Each mitigation should be concise.
- Mitigations should be actionable.
- Prefer preventative actions over detection activities.

---

## Mitigation Backlog

Sort by:

1. Highest Risk Score
2. Lowest Mitigation Effort
3. Greatest Risk Reduction Potential

Format:

| Priority | Mitigation Activity | Related Risk | Effort |
| -------- | ------------------- | ------------ | ------ |

---

## Risk Reduction Summary

Calculate:

* Total Risk Score Before Mitigation
* Estimated Risk Score After Mitigation
* Estimated Risk Reduction Percentage

Also identify:

* Highest leverage mitigation
* Cheapest mitigation
* Most expensive mitigation
* Hardest remaining risk to reduce

---

## Decision Rules

Always prioritize:

* Risk reduction over risk documentation
* Prevention over monitoring
* Mitigation over observation
* Low-effort / high-impact actions
* Organizational risks alongside technical risks

Never produce a passive risk register.

Always produce actionable mitigation work.

The final output should help the team answer:

> What should we do next to reduce the probability of delay or failure?
