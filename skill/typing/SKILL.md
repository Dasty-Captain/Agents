---
name: typing
description: Turn rough user prompts into high-quality writing tailored to audience, purpose, and context with a fast, evidence-aware editing workflow.
---

# Typing

Use this skill to transform raw notes, drafts, or prompts into polished writing without changing the user's core intent.

## When to Use This Skill

- The user has messy ideas and wants clean, professional writing.
- The user asks for rewrite, polish, tighten, simplify, or reframe.
- The user needs writing adapted for a specific audience or channel.
- The user wants multiple quality variants (short, executive, technical, persuasive).

## Outcomes

- Preserve original meaning while improving clarity and structure.
- Match tone, formality, and length to the target audience.
- Deliver publication-ready copy with minimal follow-up edits.

## Required Inputs

- Source text (notes, draft, or prompt).
- Target audience and use case (email, memo, post, report, etc.).
- Desired tone and length.
- Non-negotiables (key claims, terms, phrases to keep, banned wording).

If inputs are missing, ask only for the minimum needed values.

## Workflow

1. Identify intent, audience, and the one-sentence core message.
2. Extract constraints: tone, length, structure, and keep/remove rules.
3. Rewrite for logical flow: opening, support, close, and clear transitions.
4. Tighten language: remove redundancy, passive clutter, and vague claims.
5. Run quality pass:
   - Clarity: plain-language and concrete wording.
   - Coherence: paragraph flow and argument continuity.
   - Correctness: grammar, punctuation, and terminology consistency.
6. Provide final version plus optional variants when useful.

## Output Format

Return in this exact section order:

1. Writing Goal Snapshot
2. Improved Draft
3. Alternative Versions (optional)
4. Edits Made (what changed and why)
5. Open Assumptions

## Guardrails

- Do not invent facts, numbers, or citations.
- Preserve user intent; do not smuggle in new positions.
- Keep edits proportional to requested change level.
- Flag missing context that could alter meaning materially.
