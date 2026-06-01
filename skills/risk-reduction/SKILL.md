---

name: risk-reduction
description: Convert stress-test failure modes into a prioritized mitigation backlog by estimating likelihood, schedule impact, mitigation effort, and overall risk reduction potential.
---

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

Expected Conditions are not risks.

Expected Conditions should not appear in the Prioritized Risk Table.

Expected Conditions should still influence mitigation planning and backlog prioritization.

---

### Risks

Items with likelihood less than or equal to 50% remain risks.

Only risks are scored and prioritized.

---

## Likelihood Estimation

For every risk:

1. Estimate a likelihood percentage.
2. Provide a concise rationale.
3. Challenge the estimate internally.
4. Adjust the estimate if warranted.

Base estimates on:

* Historical patterns
* Organizational dynamics
* Technical complexity
* Stakeholder behavior
* Comparable initiatives
* Known failure modes

Do not generate arbitrary percentages.

Do not display self-challenge reasoning unless it materially changes the estimate.

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

Use decimal values for Risk Score.

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

Good examples:

* Conduct migration pilot
* Assign dependency owner
* Establish rollback rehearsal

Bad examples:

* Improve communication
* Increase visibility
* Align stakeholders

---

## Output Formatting

Use standard GitHub-flavored markdown.

Do not use:

* ASCII tables
* Unicode box-drawing tables
* Terminal-rendered tables

Output should render cleanly in:

* GitHub
* GitLab
* Google Docs
* Markdown editors

Responses containing box-drawing characters are incorrect.

---

# Risk Reduction Analysis

## Expected Conditions

Use this exact markdown table format:

| Condition | Likelihood | Why This Is Expected |
| --------- | ---------- | -------------------- |

Rules:

* Use markdown table syntax exactly.
* Do not substitute another table format.
* Limit "Why This Is Expected" to one sentence.
* Include only items with likelihood greater than 50%.

After the table, provide a short section:

### Implication

Briefly describe what the project should proactively plan for based on these Expected Conditions.

---

## Prioritized Risk Table

Use this exact markdown table format:

| Failure | Likelihood | Delay (Weeks) | Score | Effort | Rationale |
| ------- | ---------- | ------------- | ----- | ------ | --------- |

Rules:

* Use markdown table syntax exactly.
* Do not substitute another table format.
* Include only risks with likelihood less than or equal to 50%.
* Rationale must be one sentence maximum.
* Delay must represent expected schedule impact if the failure occurs.
* Score = Likelihood × Delay.
* Effort must be Low, Medium, or High.
* Sort highest score to lowest score.

---

## Mitigation Recommendations

Use this exact markdown table format:

| Failure | Mitigations |
| ------- | ----------- |

Rules:

* Use markdown table syntax exactly.
* Do not substitute another table format.
* Provide exactly three mitigation bullets per risk.
* Each mitigation should be concise.
* Each mitigation should be actionable.
* Prefer prevention over detection.

---

## Mitigation Backlog

Use this exact markdown table format:

| Priority | Mitigation Activity | Related Risk | Effort |
| -------- | ------------------- | ------------ | ------ |

Rules:

* Use markdown table syntax exactly.
* Do not substitute another table format.
* Sort by:

  1. Highest Risk Score
  2. Lowest Mitigation Effort
  3. Greatest Risk Reduction Potential

The backlog may contain more items than the number of risks.

The purpose of this section is to create actionable work.

---

## Risk Reduction Summary

Calculate:

* Total Risk Score Before Mitigation
* Estimated Risk Score After Mitigation
* Estimated Risk Reduction Percentage

Also identify:

* Highest Leverage Mitigation
* Cheapest Mitigation
* Hardest Remaining Risk

Keep this section concise.

Use bullets rather than long narrative explanations.

---

## Execution Recommendation

Provide:

### Immediate Actions

The first actions that should be taken before execution begins.

### Block Execution Until

Conditions that should be satisfied before broad rollout or commitment.

### Key Insight

The single most important insight produced by the analysis.

Limit this section to concise bullets and short paragraphs.

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
