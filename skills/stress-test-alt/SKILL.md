---
name: stress-test
description: Structured failure-first review for plans, launches, strategies, delivery commitments, and organizational decisions.
---

# Stress Test Skill

## Purpose

Test meaningful plans before commitment by assuming failure and working backward to explain why. This surfaces risks, hidden assumptions, weak signals, and organizational friction that ordinary reviews miss.

**Goal:** Make the plan harder to break.

**Output:** A Cassandra Assessment—credible failure modes, hidden assumptions, and preventable risks surfaced early enough to act upon.

---

## Relationship to Risk Reduction

```text
Stress Test → Potential Failures → Risk Reduction → Mitigation Backlog → Execution
```

**Stress Test answers:** How does this fail?  
**Risk Reduction answers:** Which failures should we prevent right now?

---

## Operating Modes

### Default Mode (Standard)

Use for: release reviews, strategy reviews, operational changes, organizational initiatives, leadership preparation, first-pass risk analysis.

**Prioritizes:** Signal over completeness, actionability over explanation, decision support over exhaustive analysis.

**Output limits:**
- 5 failure modes max
- 3 organizational failure patterns max
- 5 recommendations max
- 5 checklist items max
- 5 early warning indicators max

### Deep Dive Mode (Explicit Request Only)

Use for: workshops, executive planning sessions, major strategic initiatives, high-cost commitments, detailed investigation of specific failure modes.

**May include:** Failure narratives, expanded assumptions, detailed warning signs, prevention strategies, workshop-level analysis.

---

## When To Use This Skill

**Use when:**
- Concrete plan exists
- Cost of being wrong is meaningful
- Plan can still be changed
- Decision, commitment, launch, strategy, or organizational change is being considered

**Good candidates:** Product/feature launches, AI adoption, organizational changes, migrations, process changes, executive proposals, delivery commitments, strategic initiatives.

**Do not use for:** Factual questions, vague brainstorming, editing requests, purely creative work, irreversible decisions.

---

## Minimum Context

Before running, understand:
1. What is being stress-tested?
2. Who is affected?
3. What does success look like?

If already available from conversation/documents, proceed. Otherwise, ask one question at a time. Infer reasonable context rather than creating an intake form.

---

## Organizational Failure Modes

Always evaluate whether failure could emerge from:
- Unclear ownership
- Cross-functional dependency friction
- Overloaded teams
- Conflicting executive incentives
- Metrics distortion
- Timeline pressure overwhelming quality controls
- AI accelerating unstable processes
- Communication gaps between leadership and delivery teams
- Hidden operational work not in plans
- Governance slowing local decision-making
- Reporting overwhelming delivery

---

## Output Format

**Primary artifact:** Self-contained HTML file (default: `examples/[descriptive-name]-stress-test.html`)

**HTML requirements:**
- Inline CSS, readable typography, clear headers, bordered HTML tables
- No external dependencies, no JavaScript
- Suitable for copying into Google Docs
- Include timestamp/generated date

**If file creation unavailable:** Use clean GitHub-flavored markdown tables.

**Never use:** ASCII tables, Unicode box-drawing characters (┌ ┬ ┐ ├ ┼ ┤ └ ┴ ┘ │)

---

## Stress-Test Procedure

### Step 1: Establish the Frame

Use failure-first framing:

> It is six months from now. This plan has failed. It did not merely underperform; it failed clearly enough that people are looking back to understand what went wrong. We are now working backward to explain why.

### Step 2: Generate Failure Modes

Generate plausible failure modes that are:
- Specific to the plan
- Realistic and meaningful
- Grounded in context
- Not generic risks applicable to any initiative

### Step 3: Prioritize Failure Modes

Rank based on: likelihood, impact, preventability, decision usefulness.

**Default Mode:** Select only the 5 highest-value failure modes.  
**Deep Dive Mode:** May include up to 8 failure modes with expanded narrative analysis.

---

## Default Mode Report Structure

### Executive Summary

**Most Likely Failure**
- Failure:
- Why:
- Assumption:

**Most Dangerous Failure**
- Failure:
- Why:

**Cheapest Failure to Prevent**
- Failure:
- Action:

**Hidden Assumption**
- Assumption:

**Readiness Recommendation**

Choose one:
- Ready for Risk Reduction
- Conditionally Ready for Risk Reduction
- Not Ready for Risk Reduction

Provide no more than 5 supporting bullets.

---

### Failure Modes (HTML table)

Columns: Failure Mode | Likelihood | Impact | Warning Sign

Limit to 5 highest-value modes. Keep warning signs brief. Use short phrases, not paragraphs.

---

### Base-Rate Analysis (HTML table)

Columns: Failure Mode | Probability | Base-Rate Rationale

Limit rationale to one sentence per row. Use qualitative judgment when precise data unavailable. Do not invent statistics.

---

### Organizational Failure Patterns (HTML table)

Columns: Pattern | Why It Matters

Include no more than 3 patterns. Keep each explanation to one sentence.

---

### Revised Plan Recommendations (HTML table)

Columns: Priority | Recommendation | Failure Modes Addressed

Include no more than 5 recommendations. Recommendations should be concrete and actionable. Each should map to one or more failure modes.

---

### Pre-Launch Checklist

No more than 5 items. Each should validate a critical assumption OR prevent a high-impact failure.

---

### Early Warning Indicators (HTML table)

Columns: Indicator | Why It Matters

Include no more than 5 indicators. Avoid timelines, phases, and extended commentary.

---

### Recommended Follow-Up

If Ready/Conditionally Ready: Recommend running risk-reduction skill.  
If Not Ready: State minimum clarification or validation needed first.

---

## Default Mode Prohibitions

Must not:
- Generate failure stories, workshop narratives, or investigator reports
- Deep-dive every failure mode
- Provide exhaustive analysis
- Exceed output limits (5 failure modes, 5 recommendations, 5 checklist items, 5 early warning indicators)

Narrative exploration belongs exclusively in Deep Dive Mode.

---

## Deep Dive Mode Rules

For each selected failure mode, may include:

**Failure Story:** Realistic narrative of how failure unfolded  
**Underlying Assumption:** The assumption that enabled failure  
**Early Warning Signs:** Observable indicators failure is beginning  
**Prevention Options:** Actions that could have prevented/reduced failure

Still avoid generic risks and vague advice. Generate HTML artifact (default: `examples/[descriptive-name]-stress-test-deep-dive.html`)

---

## Chat Response Format

After completing analysis:

1. Generated file path
2. Most Likely Failure
3. Most Important Revision

Limit chat summary to three sentences. Do not paste full report into chat if HTML artifact was generated.

---

## Quality Bar

**Good Stress Test:** Specific, uncomfortable, practical, grounded in context, focused on preventable failure, clear about what should change next, delivered in easy-to-read/share/reuse format.

**Weak Stress Test:** Generic, overly polite, exhaustive for its own sake, detached from context, vague recommendations, poorly formatted.

---

## Important Distinction

**Review asks:** Is this a good idea?  
**Council asks:** What would different perspectives say?  
**Stress Test asks:** This failed. Why?

Use this skill when failure-first analysis is the right tool.
