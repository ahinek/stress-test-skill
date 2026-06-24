---

name: stress-test
description: Structured failure-first review for plans, launches, strategies, delivery commitments, and organizational decisions.
---------------------------------------------------------------------------------------------------------------------------------

# Stress Test Skill

## Purpose

Use this skill to test a meaningful plan before commitment.

A Stress Test assumes the plan has failed and works backward to explain why. This framing surfaces risks, hidden assumptions, weak signals, organizational friction, and uncomfortable truths that ordinary reviews often miss.

The goal is not to criticize the plan.

The goal is to make the plan harder to break.

## Cassandra Assessment

The primary output of the Stress Test Skill is a Cassandra Assessment.

A Cassandra Assessment identifies the most credible failure modes, hidden assumptions, and preventable risks associated with a proposed plan. The goal is not to predict the future with certainty, but to surface warnings early enough that they can still be acted upon.

The name comes from Cassandra of Greek mythology, who was granted the ability to foresee disasters but cursed to have her warnings ignored.

A Cassandra Assessment is designed to surface credible warnings before resources are committed and while corrective action remains possible.

The Stress Test Skill is the process.

The Cassandra Assessment is the artifact it produces.

---

# Relationship to Risk Reduction

Stress Test is the first step in this workflow:

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

---

# Operating Modes

This skill has two modes:

1. Default Mode
2. Deep Dive Mode

Use Default Mode unless the user explicitly asks for Deep Dive Mode.

---

## Default Mode

Default Mode is the standard behavior.

Default Mode produces a concise decision-support artifact.

Use Default Mode for:

* release reviews
* strategy reviews
* operational changes
* organizational initiatives
* leadership preparation
* first-pass risk analysis

Default Mode prioritizes:

* signal over completeness
* prioritization over documentation
* actionability over explanation
* decision support over exhaustive analysis

---

## Deep Dive Mode

Deep Dive Mode is used only when the user explicitly requests detailed analysis.

Use Deep Dive Mode for:

* workshops
* executive planning sessions
* major strategic initiatives
* high-cost commitments
* detailed investigation of a specific failure mode

Deep Dive Mode may include:

* failure narratives
* expanded assumptions
* detailed warning signs
* prevention strategies
* workshop-level analysis

---

# Invocation Rules

Use Default Mode for requests such as:

```text
Stress test this.
Stress test this plan.
Find the blind spots.
What could kill this?
Poke holes in this.
What am I missing?
```

Use Deep Dive Mode for requests such as:

```text
Stress test this in deep-dive mode.
Run a full stress test.
Give me the detailed version.
Deep dive this plan.
Expand failure mode #3.
```

If the user does not specify a mode, use Default Mode.

---

# When To Use This Skill

Use this skill when:

* the user has a concrete plan
* the cost of being wrong is meaningful
* the plan can still be changed
* there is a decision, commitment, launch, strategy, or organizational change being considered

Good candidates include:

* product launches
* feature launches
* AI adoption efforts
* organizational changes
* Jira migrations
* process changes
* executive proposals
* delivery commitments
* strategic initiatives
* platform migrations

Do not use this skill for:

* factual questions
* vague brainstorming with no concrete plan
* editing requests
* purely creative work
* decisions that are already irreversible

---

# Minimum Context

Before running a Stress Test, understand:

1. What is being stress-tested?
2. Who is affected?
3. What does success look like?

If this information is already available from the conversation or supporting documents, proceed.

If not, ask the smallest useful question necessary.

Ask one question at a time.

Infer reasonable context whenever possible rather than turning the interaction into an intake form.

---

# Commitment Requirement

Do not present all risks as equally important.

Force prioritization.

If evidence is incomplete:

* make the best grounded judgment possible
* state uncertainty clearly
* avoid hiding behind "it depends"

The skill should produce conclusions, not merely observations.

---

# Organizational Failure Modes

Always evaluate whether failure could emerge from:

* unclear ownership
* cross-functional dependency friction
* overloaded teams
* conflicting executive incentives
* metrics distortion
* timeline pressure overwhelming quality controls
* AI accelerating unstable processes
* communication gaps between leadership and delivery teams
* hidden operational work not represented in plans
* governance structures that slow local decision-making
* reporting needs overwhelming delivery needs

---

# Default Mode Output Budget

Default Mode must operate within a constrained output budget.

Maximum output:

* 5 failure modes
* 3 organizational failure patterns
* 5 recommendations
* 5 checklist items
* 5 early warning indicators

These are maximums, not targets.

Use fewer items when fewer items adequately explain the risk landscape.

Do not add content merely because it exists.

Every included item should earn its place by being:

* likely
* impactful
* preventable
* decision-relevant

---

# Output Requirements

When the environment supports file creation, create an HTML artifact as the primary output.

Default file name pattern:

```text
examples/[descriptive-name]-stress-test.html
```

If the user provides a file name or path, use the user's requested path.

Do not rely on terminal-rendered tables as the final artifact.

Do not use:

* ASCII tables
* Unicode box-drawing tables
* terminal-rendered tables

Do not use these characters in tables:

```text
┌ ┬ ┐ ├ ┼ ┤ └ ┴ ┘ │
```

The HTML artifact must:

* use real HTML tables
* include clean section headings
* use simple inline CSS
* be readable in a browser
* be suitable for copying into Google Docs
* include the full Stress Test report
* include timestamp or generated date when possible

If file creation is not available, output clean markdown using standard GitHub-flavored markdown tables.

Responses containing box-drawing characters are incorrect.

---

# HTML Artifact Requirements

Generate a single self-contained HTML file.

Use:

* inline CSS
* readable typography
* clear section headers
* bordered HTML tables
* simple spacing
* no external dependencies
* no JavaScript required

The HTML should include these sections:

1. Executive Summary
2. Failure Modes
3. Base-Rate Analysis
4. Organizational Failure Patterns
5. Revised Plan Recommendations
6. Pre-Launch Checklist
7. Early Warning Indicators
8. Recommended Follow-Up

The HTML file should be the durable artifact.

The chat response should be brief and should point to the generated file path.

---

# Stress-Test Procedure

## Step 1: Establish the Frame

Once sufficient context exists, establish the Stress Test frame.

Use wording similar to:

> It is six months from now. This plan has failed. It did not merely underperform; it failed clearly enough that people are looking back to understand what went wrong. We are now working backward to explain why.

Failure-first framing is required.

Without it, the analysis often becomes a generic risk review.

---

## Step 2: Generate Failure Modes

Generate plausible failure modes.

Failure modes must be:

* specific to the plan
* realistic
* meaningful
* grounded in context

Avoid generic risks that could apply to any initiative.

---

## Step 3: Prioritize Failure Modes

Rank failure modes based on:

* likelihood
* impact
* preventability
* decision usefulness

Default Mode:

* Select only the 5 highest-value failure modes.
* Do not attempt to catalog every possible failure.
* Omit low-value, redundant, or highly speculative risks.

Deep Dive Mode:

* May include up to 8 failure modes.
* May expand on each failure mode with additional narrative analysis.

---

# Default Mode Report Format

Default Mode must use this structure.

# Cassandra Assessment

Generated by the Stress Test Skill

This assessment identifies the most credible failure modes, hidden assumptions, and preventable risks associated with the proposed plan. The goal is not to predict the future with certainty, but to surface warnings early enough that they can still be acted upon.

The name comes from Cassandra of Greek mythology, who was granted the ability to foresee disasters but cursed to have her warnings ignored.

A Cassandra Assessment is designed to surface credible warnings before resources are committed and while corrective action remains possible.

## Executive Summary

### Most Likely Failure

* Failure:
* Why:
* Assumption:

### Most Dangerous Failure

* Failure:
* Why:

### Cheapest Failure to Prevent

* Failure:
* Action:

### Hidden Assumption

* Assumption:

### Readiness Recommendation

Choose one:

* Ready for Risk Reduction
* Conditionally Ready for Risk Reduction
* Not Ready for Risk Reduction

Provide no more than 5 supporting bullets.

---

## Failure Modes

Use an HTML table in the generated artifact.

Columns:

* Failure Mode
* Likelihood
* Impact
* Warning Sign

Rules:

* Limit to the 5 highest-value failure modes.
* Keep warning signs brief.
* Use short phrases rather than paragraphs.
* Do not provide narrative explanations inside the table.

---

## Base-Rate Analysis

Use an HTML table in the generated artifact.

Columns:

* Failure Mode
* Probability
* Base-Rate Rationale

Rules:

* Limit rationale to one sentence per row.
* Do not invent statistics.
* Use qualitative judgment when precise data is unavailable.

---

## Organizational Failure Patterns

Use an HTML table in the generated artifact.

Columns:

* Pattern
* Why It Matters

Rules:

* Include no more than 3 patterns.
* Keep each explanation to one sentence.

---

## Revised Plan Recommendations

Use an HTML table in the generated artifact.

Columns:

* Priority
* Recommendation
* Failure Modes Addressed

Rules:

* Include no more than 5 recommendations.
* Recommendations should be concrete and actionable.
* Each recommendation should map to one or more failure modes.

---

## Pre-Launch Checklist

Provide no more than 5 checklist items.

Each item should:

* validate a critical assumption

or

* prevent a high-impact failure

---

## Early Warning Indicators

Use an HTML table in the generated artifact.

Columns:

* Indicator
* Why It Matters

Rules:

* Include no more than 5 indicators.
* Avoid timelines, phases, and extended commentary.

---

## Recommended Follow-Up

If the plan is Ready or Conditionally Ready for Risk Reduction, recommend running the risk-reduction skill to convert the failure modes into a prioritized mitigation backlog.

If the plan is Not Ready for Risk Reduction, state what minimum clarification or validation is needed first.


---

## Failure Modes

Use an HTML table in the generated artifact.

Columns:

* Failure Mode
* Likelihood
* Impact
* Warning Sign

Rules:

* Limit to the 5 highest-value failure modes.
* Keep warning signs brief.
* Use short phrases rather than paragraphs.
* Do not provide narrative explanations inside the table.

---

## Base-Rate Analysis

Use an HTML table in the generated artifact.

Columns:

* Failure Mode
* Probability
* Base-Rate Rationale

Rules:

* Limit rationale to one sentence per row.
* Do not invent statistics.
* Use qualitative judgment when precise data is unavailable.

---

## Organizational Failure Patterns

Use an HTML table in the generated artifact.

Columns:

* Pattern
* Why It Matters

Rules:

* Include no more than 3 patterns.
* Keep each explanation to one sentence.

---

## Revised Plan Recommendations

Use an HTML table in the generated artifact.

Columns:

* Priority
* Recommendation
* Failure Modes Addressed

Rules:

* Include no more than 5 recommendations.
* Recommendations should be concrete and actionable.
* Each recommendation should map to one or more failure modes.

---

## Pre-Launch Checklist

Provide no more than 5 checklist items.

Each item should:

* validate a critical assumption

or

* prevent a high-impact failure

---

## Early Warning Indicators

Use an HTML table in the generated artifact.

Columns:

* Indicator
* Why It Matters

Rules:

* Include no more than 5 indicators.
* Avoid timelines, phases, and extended commentary.

---

## Recommended Follow-Up

If the plan is Ready or Conditionally Ready for Risk Reduction, recommend running the risk-reduction skill to convert the failure modes into a prioritized mitigation backlog.

If the plan is Not Ready for Risk Reduction, state what minimum clarification or validation is needed first.

---

# Default Mode Prohibitions

Default Mode must not:

* generate failure stories
* generate workshop narratives
* generate investigator reports
* deep-dive every failure mode
* provide exhaustive analysis
* explain every risk in detail
* produce more than 5 failure modes
* produce more than 5 recommendations
* produce more than 5 checklist items
* produce more than 5 early warning indicators

Narrative exploration belongs exclusively in Deep Dive Mode.

---

# Deep Dive Mode Rules

Deep Dive Mode extends the standard Stress Test.

For each selected failure mode, Deep Dive Mode may include:

### Failure Story

A realistic narrative explaining how the failure unfolded.

### Underlying Assumption

The assumption that enabled the failure.

### Early Warning Signs

Observable indicators that the failure is beginning to occur.

### Prevention Options

Actions that could have prevented or reduced the failure.

Deep Dive Mode may produce longer, workshop-level analysis.

Deep Dive Mode should still avoid generic risks and vague advice.

When the environment supports file creation, Deep Dive Mode should also generate an HTML artifact.

Default file name pattern:

```text
examples/[descriptive-name]-stress-test-deep-dive.html
```

---

# Chat Response Format

After completing the analysis, provide a brief chat summary.

Do not paste the full report into chat if an HTML artifact was generated.

The chat summary should include:

1. Generated file path
2. Most Likely Failure
3. Most Important Revision

Limit the chat summary to three sentences.

---

# Quality Bar

A good Stress Test is:

* specific
* uncomfortable
* practical
* grounded in context
* focused on preventable failure
* clear about what should change next
* delivered in a format that is easy to read, share, and reuse

A weak Stress Test is:

* generic
* overly polite
* exhaustive for its own sake
* detached from context
* vague in its recommendations
* formatted in a way that does not render cleanly

---

# Important Distinction

A review asks:

> Is this a good idea?

A council asks:

> What would different perspectives say?

A Stress Test asks:

> This failed. Why?

Use this skill when failure-first analysis is the right tool.

