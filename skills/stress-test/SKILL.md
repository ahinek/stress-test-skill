---

name: stress-test
description: Structured failure-first review for plans, launches, strategies, delivery commitments, and organizational decisions.
---

# Stress Test Skill

## Purpose

Use this skill to test a meaningful plan before commitment.

A Stress Test assumes the plan has already failed and works backward to explain why. This framing helps surface risks, hidden assumptions, weak signals, organizational friction, and uncomfortable truths that ordinary reviews often miss.

The goal is not to criticize the plan.

The goal is to make the plan harder to break.

---

# Operating Modes

This skill supports two modes.

## Default Mode

Default Mode is the standard behavior.

Use it unless the user explicitly requests a deeper analysis.

Default Mode should:

* identify the strongest failure modes
* force prioritization
* produce a concise decision-making artifact
* focus on actionable insights

Target length:

* approximately 3-5 pages
* 5-8 failure modes maximum

Default Mode should be used for:

* release reviews
* strategy reviews
* operational changes
* organizational initiatives
* leadership preparation
* first-pass risk analysis

---

## Deep Dive Mode

Deep Dive Mode is used when the user explicitly requests detailed analysis.

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

## Invocation Rules

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

# Length Control

Do not treat comprehensiveness as permission to be exhaustive.

Default Mode should identify the strongest 5-8 failure modes, not every imaginable failure.

Prioritize:

* credibility
* impact
* preventability
* decision usefulness

over completeness.

Prefer concise, high-signal analysis over long narrative explanation.

Only produce expanded failure narratives in Deep Dive Mode.

If additional failure modes exist but are substantially less likely, less impactful, or redundant, omit them.

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
* brainstorming with no concrete plan
* editing requests
* purely creative work
* decisions that are already irreversible

---

# Trigger Examples

Examples:

* stress test this
* stress test this plan
* what could kill this?
* find the blind spots
* what am I missing?
* poke holes in this
* future-proof this

Only run the skill when there is a real plan, decision, commitment, launch, or organizational change to evaluate.

---

# Minimum Context

Before running a stress test, understand:

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

---

# Operating Principles

* Be direct.
* Do not sugarcoat serious risks.
* Do not pad the analysis with generic concerns.
* Ground every failure mode in the user's actual context.
* Prefer concrete revisions over vague advice.
* Treat the synthesis as the primary product.
* Prioritize prevention over observation.

---

# Stress-Test Procedure

## Step 1: Establish the Frame

Once sufficient context exists, establish the stress-test frame.

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

Select only the strongest 5-8 failure modes.

Do not attempt to catalog every possible failure.

Omit low-value, redundant, or highly speculative risks.

---

## Step 4: Analyze Failure Modes

For each selected failure mode provide:

| Failure Mode | Why It Could Happen | Early Warning Sign |
| ------------ | ------------------- | ------------------ |

Keep analysis concise.

Narrative failure stories belong only in Deep Dive Mode.

---

## Step 5: Produce the Synthesis

Generate a Stress Test Report.

The report must contain:

### Most Likely Failure

Force a ranking.

Identify the single failure mode most likely to occur.

Explain:

* why it is most likely
* what assumptions make it likely
* what evidence supports the judgment

---

### Most Dangerous Failure

Force a ranking.

Identify the failure mode with the greatest potential impact.

Explain:

* why it is dangerous
* what second-order effects it creates
* why impact would compound if ignored

---

### Cheapest Failure To Prevent

Identify the failure mode where a relatively small intervention now would significantly reduce future risk.

Explain:

* why prevention is inexpensive
* what action would reduce the risk
* why organizations commonly overlook it

---

### Hidden Assumption

Identify the single biggest assumption underlying the plan.

This should be the assumption most likely to remain unquestioned.

---

### Base Rates

Whenever possible, explain how similar efforts commonly fail.

Do not invent statistics.

Use:

* historical patterns
* industry norms
* organizational dynamics
* comparable initiatives
* known failure tendencies

If quantitative data is unavailable, provide qualitative judgment.

---

### Revised Plan

Provide concrete changes that make the plan more resilient.

Every recommendation should map to one or more failure modes.

Avoid vague advice.

---

### Pre-Launch Checklist

Provide 3-5 specific items that should be verified before execution.

Each item should prevent or detect one of the identified failure modes.

---

### Recommended Follow-Up

When appropriate, recommend running:

```text
risk-reduction
```

to convert identified failure modes into a prioritized mitigation backlog.

---

# Deep Dive Mode Rules

Deep Dive Mode extends the standard Stress Test.

For each selected failure mode provide:

### Failure Story

A realistic narrative explaining how the failure unfolded.

### Underlying Assumption

The assumption that enabled the failure.

### Early Warning Signs

Observable indicators that the failure is beginning to occur.

### Prevention Options

Actions that could have prevented or reduced the failure.

Keep each deep dive focused and specific to the plan.

---

# Chat Response Format

After completing the analysis, provide a brief summary:

1. Most Likely Failure
2. Hidden Assumption
3. Most Important Revision

Limit the summary to three sentences.

---

# Quality Bar

A good Stress Test is:

* specific
* uncomfortable
* practical
* grounded in context
* focused on preventable failure
* clear about what should change next

A weak Stress Test is:

* generic
* overly polite
* exhaustive for its own sake
* detached from context
* vague in its recommendations

---

# Important Distinction

A review asks:

> Is this a good idea?

A council asks:

> What would different perspectives say?

A Stress Test asks:

> This failed. Why?

Use this skill when failure-first analysis is the right tool.
