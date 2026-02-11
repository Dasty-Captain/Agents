---
name: gap-analysis
description: Conduct research-grade gap analysis by comparing current state vs target state, quantifying impact, and prioritizing corrective actions.
---

# Gap Analysis

Use this skill to identify what is missing between the current state and the desired outcome, then produce a prioritized, execution-ready correction plan.

## When to Use This Skill

- The user asks what is missing to reach a goal.
- The user needs a current-vs-target assessment with priorities.
- The user needs strategic or operational bottleneck diagnosis.
- The user asks for roadmap correction based on evidence.

## Outcomes

- A clear map of gaps by category, impact, and root cause.
- A prioritized action plan with owners, sequencing, and risks.
- Decision support for where to invest first.

## Required Inputs

- Scope and objective (team, product, process, market, or thesis).
- Current state evidence (metrics, artifacts, process docs, or outputs).
- Target state definition with measurable criteria.
- Constraints (time, budget, headcount, policy, tooling).

If inputs are missing, ask only for the minimum needed values.

## Workflow

1. Define analysis scope and success criteria in measurable terms.
2. Build the baseline (current state) from available evidence.
3. Define target state and acceptance thresholds.
4. Identify and classify gaps:
   - Capability gap
   - Process gap
   - Resource gap
   - Knowledge gap
   - Governance/risk gap
5. Score each gap using:
   - Impact (1-5)
   - Urgency (1-5)
   - Confidence (1-5)
   - Priority score = Impact x Urgency x Confidence
6. Produce root-cause analysis and corrective actions per top gaps.
7. Sequence actions into now/next/later with dependencies and owners.

## Output Format

Return in this exact section order:

1. Objective and Scope
2. Current State Snapshot
3. Target State Definition
4. Gap Register (scored)
5. Prioritized Action Plan
6. Risks and Dependencies
7. Decisions Needed

## Guardrails

- Do not label a gap without explicit current and target evidence.
- Separate observed facts from inference.
- Prefer reversible, high-leverage actions first.
- Highlight low-confidence conclusions and what evidence would raise confidence.
