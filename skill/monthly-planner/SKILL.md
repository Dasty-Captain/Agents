---
name: monthly-planner
description: Plan monthly OKRs, verify alignment to quarterly key results, and flag gaps with concrete correction actions.
---

# Monthly Planner

Use this skill to build or review monthly OKRs against quarterly key results.

## Outcomes

- Produce a monthly OKR draft with measurable key results.
- Score alignment to quarterly key results and company KPIs.
- Highlight risk early and propose corrective actions.

## Required Inputs

- Current quarter goals and key results.
- Current month target metrics and baseline metrics.
- Team ownership map and available capacity.
- Current sprint progress snapshot.

If inputs are missing, ask only for the minimum needed values.

## Workflow

1. Extract quarterly key results and convert each into measurable monthly outcomes.
2. Draft monthly OKRs using this structure:
   - Objective: qualitative and directional.
   - Key Results: numeric target, baseline, due date, owner.
3. Run alignment checks for each KR:
   - Directional fit: does it move a quarterly KR?
   - Magnitude fit: is the monthly target proportional to quarter plan?
   - Feasibility fit: does assigned capacity support the target?
4. Compute status forecast:
   - On track: >= 90% confidence.
   - At risk: 60-89% confidence.
   - Off track: < 60% confidence.
5. For At risk or Off track, propose a recovery plan with:
   - Scope reductions.
   - Owner rebalance.
   - Fast experiments with decision deadlines.

## Output Format

Return in this exact section order:

1. Monthly OKR Draft
2. Alignment Matrix (Monthly KR -> Quarterly KR)
3. Risk Assessment
4. Recommended Corrections
5. Open Questions

## Guardrails

- Do not produce vague KRs; every KR must be measurable.
- Avoid adding more than 5 KRs per objective unless explicitly requested.
- Prioritize outcomes that directly support ARR/MRR and strategic product milestones.
