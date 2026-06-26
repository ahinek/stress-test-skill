---
name: stress-test
description: Structured failure-first review for plans, launches, strategies, delivery commitments, and organizational decisions.
---

# Stress Test Skill

## Purpose

Use this skill to evaluate meaningful plans before commitment by assuming the plan has already failed and working backward to determine why.

Failure-first analysis surfaces hidden assumptions, organizational friction, weak signals, and preventable risks that conventional reviews often overlook.

The objective is not to criticize the plan.

The objective is to improve the plan before reality does.

---

# Cassandra Assessment

The primary output of the Stress Test Skill is a **Cassandra Assessment**.

A Cassandra Assessment identifies the most credible failure modes, hidden assumptions, and preventable risks associated with a proposed plan. Its purpose is not to predict the future with certainty, but to expose the most likely ways a plan could fail while there is still time to improve it.

The name comes from Cassandra of Greek mythology, who was granted the ability to foresee disasters but cursed to have her warnings ignored.

A Cassandra Assessment is designed to surface credible warnings before resources are committed and while corrective action remains possible.

The **Stress Test Skill** is the process.

The **Cassandra Assessment** is the artifact it produces.

---

# Core Principles

Every Stress Test should follow these principles.

## 1. Assume Failure

Begin with the assumption that the plan has already failed.

Work backward to determine the most credible explanations.

Do not evaluate whether the plan is "good." Explain why it failed.

---

## 2. Commit to Conclusions

Do not present every risk as equally important.

Rank findings by:

- Likelihood
- Impact
- Preventability
- Decision value

When evidence is incomplete:

- Make the best grounded judgment possible.
- Clearly distinguish evidence from uncertainty.
- Avoid hiding behind "it depends."

Produce conclusions, not merely observations.

---

## 3. Be Specific

Avoid generic risks that could apply to almost any initiative.

Every finding should be grounded in:

- the plan
- the organization
- the stakeholders
- the delivery context

If a finding could be copied unchanged into another assessment, it probably is not specific enough.

---

## 4. Be Actionable

Every recommendation should improve the plan.

Prefer recommendations that:

- reduce risk
- expose assumptions
- simplify execution
- clarify ownership
- improve decision quality

Avoid recommendations that merely restate the problem.

---

## 5. Be Concise

Prefer fewer, stronger findings over exhaustive analysis.

Every item included in the assessment should earn its place by being:

- likely
- impactful
- preventable
- decision-relevant

Do not add findings simply because additional risks exist.

---

# Relationship to Risk Reduction

Stress Test is the first step in a two-skill workflow.

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

The Stress Test Skill identifies the most credible ways a plan could fail.

The Risk Reduction Skill converts those findings into a prioritized mitigation backlog.

---

# Operating Modes

## Default Mode

Default Mode is the standard operating mode.

Use it for:

- release reviews
- strategy reviews
- organizational initiatives
- operational improvements
- executive proposals
- delivery commitments
- first-pass risk analysis

Default Mode emphasizes:

- decision support over exhaustive analysis
- prioritization over completeness
- actionability over explanation
- concise, high-value findings

Unless explicitly requested otherwise, always use Default Mode.

### Output Limits

Maximum:

- 5 failure modes
- 3 organizational failure patterns
- 5 recommendations
- 5 checklist items
- 5 early warning indicators

These are maximums—not targets.

Use fewer items whenever they adequately explain the risk landscape.

---

## Deep Dive Mode

Deep Dive Mode is used only when explicitly requested.

Use it for:

- executive planning workshops
- major strategic initiatives
- high-cost commitments
- detailed investigation of specific failure modes

Deep Dive Mode may include:

- failure narratives
- expanded assumptions
- detailed warning signs
- prevention strategies
- workshop-level analysis

The same Core Principles still apply.

---

# When to Use This Skill

Use this skill when:

- a concrete plan exists
- meaningful decisions have not yet been finalized
- the cost of failure is significant
- meaningful changes are still possible

Typical applications include:

- product launches
- feature launches
- AI adoption initiatives
- organizational changes
- Jira or platform migrations
- process improvements
- delivery commitments
- executive proposals
- strategic initiatives

Do not use this skill for:

- factual questions
- open-ended brainstorming
- editing or writing assistance
- purely creative work
- decisions that have already become irreversible

---

# Minimum Context

Before beginning the assessment, understand:

1. What is being evaluated?
2. Who is affected?
3. What does success look like?

If sufficient context already exists in the conversation or supporting documents, begin immediately.

Otherwise, ask only the smallest number of questions necessary to complete the assessment.

Prefer inference over interrogation.

Avoid turning the assessment into an intake form.

---

# Operating Rules

The quality of a Cassandra Assessment depends more on disciplined reasoning than exhaustive analysis.

### Prefer Expected Failures

Begin with failure modes that commonly occur in similar initiatives before exploring unusual possibilities.

Use historical patterns, organizational experience, and known delivery risks whenever possible.

Rare events deserve attention only when their consequences or likelihood justify it.

---

### Challenge Assumptions

Look for assumptions that the plan depends upon but never explicitly states.

Examples include:

- ownership
- staffing
- organizational alignment
- stakeholder behavior
- technical readiness
- external dependencies
- schedule realism
- governance
- customer adoption

Treat hidden assumptions as first-class risks.

---

### Look Beyond Technical Risk

Evaluate both execution risks and organizational risks.

Many plans fail because of coordination, communication, incentives, governance, or competing priorities rather than technical implementation.

Do not allow technical discussion to crowd out organizational analysis.

---

### Distinguish Evidence from Judgment

Separate:

- observable facts
- reasonable inference
- informed judgment
- uncertainty

Do not invent evidence.

Do not overstate confidence.

When uncertainty exists, acknowledge it while still making a recommendation.

---

### Prefer Actionable Findings

Every significant finding should lead naturally to one or more actions.

Avoid observations that cannot influence a decision.

If a finding would not change the plan, consider omitting it.

---

### Maintain Appropriate Skepticism

Do not assume the proposal is flawed.

Do not assume it is sound.

Approach every plan as something capable of succeeding or failing depending on the validity of its assumptions and execution.

---

# Organizational Failure Patterns

Always consider whether failure could emerge from one or more of these areas:

- unclear ownership
- cross-functional dependency friction
- overloaded teams
- conflicting incentives
- metrics distortion
- governance bottlenecks
- communication gaps
- hidden operational work
- unrealistic coordination assumptions
- timeline pressure overwhelming quality controls
- AI accelerating unstable processes
- reporting requirements overwhelming delivery

Only include patterns that materially contribute to the assessment.

---

# Output Requirements

The primary deliverable is a **Cassandra Assessment**.

When file creation is supported:

- Generate a single self-contained HTML document.
- Use the default filename:

```text
examples/[descriptive-name]-stress-test.html
```

Unless the user specifies another path.

The HTML should:

- use inline CSS
- use semantic HTML headings
- use bordered HTML tables
- be readable in a browser
- copy cleanly into Google Docs
- require no external assets or JavaScript
- include a generated timestamp when practical

If HTML generation is unavailable, produce clean GitHub-flavored Markdown.

Never use:

- ASCII tables
- Unicode box-drawing tables
- terminal-rendered tables

---

# Stress-Test Procedure

## Step 1 — Establish the Frame

Begin with failure-first framing.

Use wording similar to:

> It is six months from now. This plan has failed. It did not merely underperform—it failed clearly enough that people are looking back to understand what happened. We are now working backward to determine why.

This framing is required.

Without it, the assessment often becomes a conventional risk review.

---

## Step 2 — Identify Failure Modes

Generate plausible failure modes.

Each should be:

- specific
- realistic
- meaningful
- grounded in context

Avoid generic risks that could apply to almost any initiative.

---

## Step 3 — Prioritize

Rank findings according to:

- likelihood
- impact
- preventability
- decision value

Default Mode should identify only the highest-value findings.

Deep Dive Mode may explore additional failure modes when explicitly requested.

Remember:

A shorter assessment with stronger conclusions is preferable to a longer assessment filled with weaker observations.

```markdown
---

# Cassandra Assessment Specification

Every assessment should communicate a clear point of view while remaining grounded in evidence.

The assessment should be concise, prioritized, and immediately useful to decision-makers.

Use the following structure.

# Cassandra Assessment

*Generated by the Stress Test Skill*

A Cassandra Assessment identifies the most credible failure modes, hidden assumptions, and preventable risks associated with the proposed plan. Its purpose is not to predict the future with certainty, but to expose the most likely ways a plan could fail while there is still time to improve it.

---

## Overall Assessment

Choose one:

- Ready for Risk Reduction
- Conditionally Ready for Risk Reduction
- Not Ready for Risk Reduction

Briefly explain the reasoning behind the assessment.

---

## Executive Summary

Include:

- Most Likely Failure
- Most Dangerous Failure
- Cheapest Failure to Prevent
- Hidden Assumption

Keep each finding concise and decision-oriented.

---

## Failure Modes

Present as an HTML table containing:

| Failure Mode | Likelihood | Impact | Early Warning Sign |

Include only the highest-value failure modes.

Maximum: 5

---

## Base-Rate Analysis

Present as an HTML table.

| Failure Mode | Probability | Base-Rate Rationale |

Do not invent statistics.

Use qualitative probability whenever precise historical data is unavailable.

---

## Organizational Failure Patterns

Present as an HTML table.

| Pattern | Why It Matters |

Maximum: 3

Only include patterns that materially contribute to failure.

---

## Revised Plan

Present as an HTML table.

| Priority | Recommendation | Failure Modes Addressed |

Recommendations should be:

- concrete
- actionable
- proportional to the identified risks

Maximum: 5

---

## Pre-Launch Checklist

Provide no more than five items.

Every checklist item should validate a critical assumption or prevent a high-impact failure.

---

## Early Warning Indicators

Present as an HTML table.

| Indicator | Why It Matters |

Maximum: 5

Indicators should be observable signals that suggest a failure mode is beginning to emerge.

---

## Recommended Follow-Up

If the assessment is **Ready** or **Conditionally Ready**, recommend running the Risk Reduction Skill.

If **Not Ready**, explain the minimum clarification, validation, or planning required before meaningful risk reduction can begin.

---

# HTML Guidance

When HTML generation is available:

- Generate one self-contained HTML document.
- Use semantic HTML headings.
- Use bordered HTML tables.
- Use simple inline CSS.
- Keep typography clean and readable.
- Require no JavaScript or external assets.
- Include a generated timestamp when practical.

The HTML document is the durable artifact.

The chat response is only a summary.

---

# Deep Dive Mode

Deep Dive Mode extends—not replaces—the standard Cassandra Assessment.

After producing the standard assessment, expand selected failure modes as appropriate.

Each expanded failure mode may include:

- Failure Story
- Underlying Assumption
- Escalation Path
- Early Warning Signs
- Prevention Options

Deep Dive should provide additional insight rather than additional volume.

Do not expand every failure mode simply because Deep Dive Mode was requested.

---

# Chat Response

When an HTML artifact is generated, do not reproduce the assessment in chat.

Instead provide:

1. Generated file path.
2. Overall Assessment.
3. Most Likely Failure.
4. Highest-priority recommendation.

Limit the chat response to three or four concise sentences.

---

# Quality Bar

A strong Cassandra Assessment is:

- specific
- evidence-based
- willing to reach conclusions
- appropriately skeptical
- actionable
- concise
- grounded in organizational reality

A weak Cassandra Assessment is:

- generic
- exhaustive for its own sake
- reluctant to prioritize
- dominated by speculation
- detached from the actual plan
- filled with recommendations that would not change a decision

When deciding between completeness and usefulness, choose usefulness.

---

# Philosophy

A review asks:

> Is this a good plan?

A council asks:

> What would different perspectives say?

A Stress Test asks:

> This failed. Why?

A Cassandra Assessment answers:

> Given what we know today, what are the most credible reasons this plan could fail, and what should we change before reality teaches us the same lesson?

The purpose of this skill is not to predict the future.

Its purpose is to improve decisions before commitments become expensive to reverse.
```

