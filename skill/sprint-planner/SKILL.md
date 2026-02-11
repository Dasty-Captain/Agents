---
name: sprint-planner
description: Build weekly sprint plans aligned to monthly OKRs, assign owners, assess delivery risk, and auto-suggest recovery plans.
---

# Sprint Planner

Use this skill for weekly sprint planning (1 week = 1 sprint) tied to monthly OKRs.

## Outcomes

- Convert monthly OKRs into sprint-sized deliverables.
- Assign each task to a specific owner.
- Assess achievability and risk before sprint commitment.
- Auto-suggest corrective actions when behind plan.

## Required Inputs

- Monthly OKRs with targets and deadlines.
- Current progress per KR (actual vs target).
- Team members, ownership areas, and capacity.
- Known blockers, dependencies, and constraints.

## Workflow

1. Break each monthly KR into sprint tasks with explicit Definition of Done.
2. Assign tasks by owner based on role fit and available capacity.
3. Estimate expected sprint impact per task on monthly KR progress.
4. Run risk scoring for each task and for the sprint overall:
   - Impact: low/medium/high
   - Probability: low/medium/high
   - Risk score: probability x impact
5. Evaluate monthly achievability after this sprint:
   - Forecast month-end trajectory from current pace.
   - Label as On track, At risk, or Behind.
6. If At risk or Behind, auto-generate a recovery plan:
   - Drop or defer low-impact work.
   - Reallocate ownership to remove bottlenecks.
   - Add a short-cycle milestone with a checkpoint date.
   - Escalate dependencies with clear owner and due date.

## Output Format

Return in this exact section order:

1. Sprint Plan (Tasks, Owners, DoD)
2. KR Contribution Map
3. Risk Register
4. Achievability Assessment
5. Auto-Recovery Suggestions
6. Decisions Needed

## Guardrails

- Never assign a task without a named owner.
- Avoid hidden dependencies; call them out explicitly.
- Keep sprint scope realistic for a one-week cadence.
