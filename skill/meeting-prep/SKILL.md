---
name: meeting-prep
description: Prepare monthly retrospective, sprint planning/retro, or manager sync meetings using last-meeting context and targeted prep questions.
---

# Meeting Prep

Use this skill to prepare one of three meeting types:

1. Monthly Retrospective
2. Sprint Planning/Retro (1 week = 1 sprint)
3. Manager Sync (quarter/monthly OKR alignment)

## Mandatory First Step

Always ask: "Which meeting type are we preparing: 1) Monthly Retrospective, 2) Sprint Planning/Retro, or 3) Manager Sync?"

Then call `@context-engineer` first to retrieve:

- Last meeting notes and outcomes for that meeting type.
- Open decisions and unresolved blockers.
- Relevant KR/OKR progress context for this meeting.

Do not draft the agenda before context-engineer results are returned.

## Workflow

1. Confirm meeting type and participants.
2. Retrieve context with `@context-engineer`.
3. Build a tailored prep packet:
   - Agenda with time boxes.
   - Decision items.
   - Key metrics snapshot.
   - Risks and escalations.
4. Ask user focused prep questions before finalizing.

## Prep Questions By Meeting Type

### Monthly Retrospective

- What was the biggest win this month?
- Which commitments slipped and why?
- What one process change should we test next month?

### Sprint Planning/Retro

- What did we complete vs commit last sprint?
- What blocked delivery and who owns resolution?
- What is the highest-impact scope for next sprint?

### Manager Sync

- Which monthly KRs are off trajectory?
- Where do we need staffing or cross-team support?
- Which quarterly outcomes need escalation this week?

## Output Format

Return in this exact section order:

1. Meeting Type and Objective
2. Last-Meeting Context (from @context-engineer)
3. Draft Agenda (time-boxed)
4. Discussion Prompts
5. Decisions to Capture
6. Pre-Meeting Checklist

## Guardrails

- Keep agendas brief and decision-focused.
- Link every discussion item to an objective or KR.
- Ask concise prep questions; avoid broad open-ended questionnaires.
