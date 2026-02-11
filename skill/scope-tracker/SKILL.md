---
name: scope-tracker
description: Track backlog scope, monitor delivery risk, and propose controlled scope changes with confirm-before-execute workflow.
---

# Scope Tracker

Use this skill to scale backlog management and control delivery risk.

## Required Behavior

- Accept a Notion backlog link as primary source.
- Analyze current scope, priorities, dependencies, and risk.
- Write a draft plan in chat first.
- Ask for explicit user confirmation before performing any task execution.

## Workflow

1. Parse backlog from the provided Notion link.
2. Group items by:
   - Strategic alignment (quarter/monthly KR fit)
   - Delivery urgency
   - Dependency chain and owner availability
3. Build a risk table with top threats:
   - Scope creep
   - Resource contention
   - Cross-team dependency delay
   - Ambiguous acceptance criteria
4. Propose scope actions:
   - Keep
   - Defer
   - Split
   - Drop
   - Escalate
5. Draft response in chat and wait for user approval.
6. Only after approval, execute agreed updates/tasks.

## Output Format

Return in this exact section order:

1. Backlog Snapshot
2. Scope Change Proposals
3. Risk Register
4. Recommended Execution Plan
5. Confirmation Request

Use this confirmation prompt exactly:
"I drafted the scope/risk plan. Reply with APPROVE to execute, or specify changes."

## Guardrails

- Never execute updates without explicit confirmation.
- Keep recommendations reversible when possible.
- Tie each scope decision to business impact.
