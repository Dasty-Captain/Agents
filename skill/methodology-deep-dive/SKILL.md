---
name: methodology-deep-dive
description: Design and stress-test first-principles methodologies for problems where standard playbooks do not exist.
---

# Methodology Deep Dive

Use this skill when the user needs a new method for an unsolved or novel problem and existing frameworks are insufficient.

## Required Behavior

- Start from first principles, not analogy-first copying.
- Make assumptions explicit and testable.
- Compare candidate approaches before selecting one.
- Include failure modes, boundary conditions, and validation plan.

## Required Inputs

- Problem statement and target outcome.
- Constraints (time, resources, risk, regulation, ethics).
- What has already been tried and why it failed.
- Success metrics and adoption context.

If inputs are missing, ask only for the minimum needed values.

## Workflow

1. Define problem in invariant terms (what must be true for success).
2. Decompose into first principles and hard constraints.
3. Map unknowns and high-risk assumptions.
4. Generate multiple candidate methodologies.
5. Evaluate candidates against criteria:
   - Feasibility
   - Scalability
   - Reversibility
   - Risk exposure
   - Learning speed
6. Select recommended method and specify implementation steps.
7. Create validation plan with experiments, checkpoints, and kill criteria.
8. Document adaptation rules for different contexts.

## Output Format

Return in this exact section order:

1. Problem and Constraints
2. First-Principles Decomposition
3. Candidate Methodologies
4. Selected Method and Why
5. Implementation Blueprint
6. Validation and Experiment Plan
7. Failure Modes and Mitigations
8. When Not to Use This Method

## Guardrails

- Do not claim novelty without checking adjacent known methods.
- Do not skip falsifiability; every key assumption needs a test.
- Keep early implementation reversible until evidence improves.
- Flag ethical, legal, and safety boundaries explicitly.

## Escalation Triggers

- High-impact decisions with weak evidence and tight deadlines.
- Safety, legal, or reputational downside is material.
- Validation results contradict core assumptions.
