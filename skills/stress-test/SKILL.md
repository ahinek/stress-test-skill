---
name: stress-test
description: Structured failure-first review for plans, launches, strategies, delivery commitments, and organizational decisions.
---
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Stress Test Skill

## Purpose

Use this skill to help a user test a meaningful plan before they commit to it.

A stress test assumes the plan has already failed and works backward to explain why. This framing helps surface risks, false assumptions, weak signals, and uncomfortable truths that ordinary feedback often misses.

The goal is not to criticize the user’s plan for sport. The goal is to make the plan harder to break.

## When to Use This Skill

Use this skill when the user has a concrete plan, decision, strategy, launch, or commitment where the cost of being wrong is meaningful.

Good targets include:

* Product or feature launches
* Go-to-market plans
* Pricing or packaging changes
* Hiring decisions
* Strategy or positioning shifts
* Partnerships or vendor decisions
* Executive proposals
* Major process changes
* High-cost or high-visibility commitments

Do not use this skill for:

* Vague early ideas with no concrete plan yet
* Questions with a factual answer
* General editing or creative feedback
* Decisions that are already made and cannot be changed
* Requests that are better handled as multi-perspective review rather than failure analysis

## Trigger Guidance

### Mandatory Triggers

Run this skill when the user says something like:

* “premortem this”
* “premortem my…”
* “run a premortem”
* “what could kill this?”
* “future-proof this”
* “stress test this plan”
* “what am I missing here?”
* “find the blind spots”

### Strong Triggers

Usually run this skill when the user says something like:

* “what could go wrong?”
* “am I missing anything?”
* “poke holes in this”
* “where will this break?”
* “devil’s advocate this”

Only run the skill if there is an actual plan, decision, or commitment to analyze.

## Commitment Requirement

* Do not present all risks as equally important.
* Force prioritization.
* If evidence is incomplete, make the best grounded judgment anyway.
* Clearly state uncertainty rather than avoiding commitment.
* Avoid collapsing into “it depends” unless the situation genuinely requires it.

## Organizational Failure Modes

Always evaluate whether failure is likely to emerge from:

* unclear ownership
* cross-functional dependency friction
* overloaded teams
* conflicting executive incentives
* metrics distortion
* timeline pressure overwhelming quality controls
* AI accelerating unstable processes
* communication gaps between leadership and delivery teams
* hidden operational work not represented in plans

## Operating Principles

* Be direct.
* Do not sugarcoat serious risks.
* Do not pad the analysis with generic concerns.
* Ground every failure mode in the user’s actual context.
* Ask for missing context only when needed.
* Prefer concrete revisions over vague advice.
* Treat the synthesis as the main product.

## Minimum Context Required

Before running the stress test, make sure you understand three things:

1. **What is being premortemed?**
   The plan, product, launch, hire, strategy, or decision should be describable in one sentence.

2. **Who is affected?**
   Identify the audience, customers, users, team, stakeholders, buyers, or decision-makers involved.

3. **What does success look like?**
   Understand the outcome the user is hoping for. Failure is defined by inverting success.

## Context Gathering Process

### Step 1: Scan Existing Context

Before asking the user for more information, use any context already available:

* The current conversation
* Files or documents the user attached
* Project notes, briefs, plans, README files, or other relevant workspace content
* Any explicit constraints, success criteria, or stakeholders already mentioned

Do not over-search. The goal is to gather enough context to run a useful premortem, not to perform open-ended research.

### Step 2: Evaluate Sufficiency

Proceed if you can answer:

* What is the plan?
* Who is it for or who does it affect?
* What outcome would count as success?

If one or more of these is missing, ask the smallest useful question.

Ask one question at a time. Do not turn this into an intake form.

Examples:

* “What specifically are you about to launch, build, or decide?”
* “Who is this for?”
* “What would make this a win?”

If an answer can be reasonably inferred from context, infer it rather than asking.

## Premortem Procedure

### Step 1: Set the Frame

Once the minimum context is available, explicitly establish the premortem frame.

Use wording like:

> It is six months from now. This plan has failed. It did not merely underperform; it failed clearly enough that the team is looking back to understand what went wrong. We are now working backward to identify why it failed.

This frame is required. Without it, the response may drift into ordinary risk review.

### Step 2: Generate Raw Failure Reasons

Generate a comprehensive list of genuine failure reasons.

Instructions:

* Assume the plan failed six months from now.
* Identify every plausible, meaningful reason it failed.
* Be specific to the plan.
* Do not include generic risks that could apply to any plan.
* Do not pad the list.
* Do not stop early if there are more real failure modes.

Each failure reason should be one to two sentences.

Use as many failure reasons as the plan deserves. Some plans may have four. Others may have nine or more.

### Step 3: Deep-Dive Each Failure Mode

For each failure reason, conduct an independent deep dive.

If the environment supports parallel sub-agents or parallel task execution, run one investigator per failure reason in parallel. If parallel execution is not available, simulate separate independent passes and avoid letting earlier failure analyses bias later ones.

Use this prompt structure for each deep dive:

```text
You are an investigator in a premortem analysis. You have been assigned one specific failure reason to analyze in depth.

The plan:
---
[Summarize the full relevant context: what it is, who it is for, what success looks like, and any constraints or source context.]
---

PREMORTEM FRAME: It is six months from now. This plan has failed.

YOUR ASSIGNED FAILURE REASON:
[Insert the specific failure reason.]

Your job is to go deep on this one failure. Write the story of how it actually played out. Be specific. Use details from the plan. Make it feel like a realistic case study.

Your output must include:

1. THE FAILURE STORY
A 2-3 paragraph narrative of how this specific failure played out. Name the moments where things went wrong and explain why.

2. THE UNDERLYING ASSUMPTION
The one thing the user was taking for granted that made this failure possible. State it in one sentence.

3. EARLY WARNING SIGNS
1-2 concrete, observable signals that would indicate this failure mode is beginning to happen. These should be measurable or visible, not vague feelings.

Keep the response under 300 words. Be direct. Do not hedge. Do not sugarcoat.
```

### Step 4: Synthesize the Results

After the deep dives, produce a synthesis report.

The synthesis must include:

## Stress Test Report

### 1. Most Likely Failure

Force a ranking.

Identify the single failure scenario most likely to happen based on the available context.

Do not hedge between multiple equally likely outcomes unless the evidence genuinely supports a tie.

Explain:

* Why this failure is the most probable
* What assumptions make it likely
* What evidence or patterns support the ranking

### 2. Most Dangerous Failure

Force a ranking.

Identify the single failure scenario that would cause the most damage if it happened, even if it is not the most likely.

Explain:

* Why this failure is the most dangerous
* What second-order effects it creates
* Why the impact would compound if ignored

### 3. Cheapest Failure to Prevent

Identify the failure mode where a relatively small intervention now would significantly reduce risk later.

Explain:

* Why prevention is inexpensive or low-friction
* What specific action would reduce the risk
* Why teams often fail to address it early even though it is preventable

### 4. Hidden Assumption

Identify the single biggest assumption the user appears to be making across the plan.

This should be the assumption that is most likely to go unquestioned because it feels obvious to the user.

### 5. Revised Plan

Provide concrete changes that would make the plan more resilient.

Each revision must map directly to one or more failure modes.

Avoid vague advice such as:

* “Consider testing the idea.”
* “Improve communication.”
* “Think about stakeholders.”

Use concrete advice such as:

* “Run a 20-person pilot before committing to the full launch.”
* “Require written approval from the two stakeholder groups before announcing the date.”
* “Test the pricing with 10 target buyers before building the full offer.”

### 6. Pre-Launch Checklist

Provide 3-5 specific things the user should verify, test, or put in place before executing.

Each checklist item should prevent or detect one of the identified failure modes.

### 7. Base Rates

Whenever possible, estimate how commonly this category of project fails in the identified ways.

Do not fabricate statistics.

Use:

* Historical patterns
* Industry norms
* Comparable project classes
* Organizational dynamics
* Known failure tendencies in similar launches, transformations, tools, or strategic initiatives

Examples:

* “Internal tooling adoption projects commonly fail because workflow disruption was underestimated.”
* “Cross-functional reporting initiatives frequently stall due to unclear ownership.”
* “AI enablement efforts often fail because teams optimize for tool usage rather than operational integration.”

The goal is to anchor the analysis in reality rather than treating every failure mode as equally novel.

If precise base rates are unavailable, provide directional estimates and clearly label them as qualitative judgment.

## Optional File Outputs

When the environment supports file creation, generate two files:

```text
premortem-report-[timestamp].html
premortem-transcript-[timestamp].md
```

### HTML Report Requirements

Create a single self-contained HTML file with inline CSS.

Use:

* Dark background
* Clean typography
* Scannable cards
* Prominent synthesis section at the top
* One visual card per failure mode
* Severity and likelihood indicators for each failure mode
* A grid showing the number of investigator passes and their findings
* Footer with timestamp and the item being premortemed

The report should prioritize readability over decoration.

### Transcript Requirements

Create a Markdown transcript containing:

* Context gathered
* Raw failure reasons
* Deep dives for each failure mode
* Full synthesis
* Final checklist

## Chat Response Format

After completing the premortem, provide a short chat summary.

Keep it to three sentences or fewer:

1. Most likely failure
2. Hidden assumption
3. Single most important revision

Example:

> The most likely failure is audience mismatch: the people who show up are not the buyers the plan depends on. The hidden assumption is that the target audience is reachable through the channel you plan to use. The most important revision is to run a small pilot with the intended audience before committing to the full launch.

## Quality Bar

A good premortem is:

* Specific
* Uncomfortable
* Practical
* Grounded in context
* Focused on preventable failure
* Clear about what to change next

A weak premortem is:

* Generic
* Overly polite
* Filled with obvious risks
* Detached from the user’s actual plan
* Heavy on categories but light on judgment
* Full of vague recommendations

## Example

User request:

> Premortem this: I am about to launch a $297 live workshop on how to use Claude for marketing teams. It has 50 seats and targets marketing managers at companies with 10-50 employees.

Raw failure reasons might include:

1. Marketing managers at this company size may need approval to spend $297, creating more purchase friction than expected.
2. The tool-specific pitch may be too narrow for buyers who are still trying to understand whether AI is relevant to their work at all.
3. The people most likely to buy may be solopreneurs rather than marketing managers, creating a mismatch between content and audience.
4. The workshop may require realistic marketing data, demos, and multi-seat scenarios that take longer to prepare than expected.
5. Testimonials from the wrong audience may weaken future cohorts.
6. The maximum revenue may not justify the preparation time compared with other opportunities.

Synthesis example:

> The most likely failure is audience mismatch: the offer attracts solopreneurs rather than marketing managers. The most dangerous failure is that the wrong early audience produces testimonials and case studies that make future marketing less credible. The hidden assumption is that “marketing managers at 10-50 person companies” are a reachable and self-identifying audience. The most important revision is to run a smaller paid pilot first and use it to validate who actually buys before building the full workshop.

## Important Distinction

This skill is not a general review and not a multi-perspective council.

A review asks, “Is this good?”
A council asks, “What would different perspectives say?”
A stress test asks, “This failed. Why?”

Use the stress test only when that failure-first frame is the right tool.
