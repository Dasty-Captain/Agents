---
name: legal-work
description: Triage legal tasks, assess risk, and draft decision-ready legal support with explicit escalation and confirmation gates.
---

# Legal Work

Use this skill for legal operations support such as contract review, policy/compliance checks, dispute prep, and legal research briefs.

## Required Behavior

- Always call `@context-engineer` first before analysis or drafting.
- Propose a short plan before execution and apply quality standards.
- Treat outputs as legal operations support, not licensed legal advice.
- Ask for explicit user confirmation before any external send/filing/escalation action.

## Required Inputs

- Request type: contract review, compliance, policy, dispute, filing prep, or research.
- Business objective and desired outcome.
- Jurisdiction/governing law assumptions (if known).
- Deadline, impact level, and decision owner.
- Source artifacts (contracts, prior redlines, policies, notices, evidence).

If inputs are missing, ask only for the minimum needed values.

## Workflow

1. Classify request type and legal risk surface.
2. Call `@context-engineer` for prior decisions, related notes, and open action context.
3. Gather and normalize source materials.
4. Build a risk-tiered issue list:
   - Critical: potential severe legal/financial exposure.
   - High: meaningful exposure or deadline risk.
   - Medium: manageable risk with clear mitigations.
   - Low: routine/administrative updates.
5. Produce a recommendation package:
   - Key issues and rationale.
   - Proposed edits/checklist/actions.
   - Assumptions and unknowns.
   - Decision points with owner and due date.
6. For Critical/High or uncertain jurisdiction, escalate to licensed counsel before execution.
7. Present draft and wait for user approval before external actions.

## Output Format

Return in this exact section order:

1. Legal Request Snapshot
2. Context and Assumptions
3. Risk Matrix (Critical/High/Medium/Low)
4. Recommended Actions
5. Escalation Needs
6. Decisions Needed
7. Confirmation Request

Use this confirmation prompt exactly:
"I drafted the legal support package. Reply with APPROVE to execute, or specify changes."

## Guardrails

- Do not represent output as legal advice or substitute for licensed counsel.
- Do not send documents, emails, or filings externally without explicit approval.
- Flag missing jurisdiction/fact assumptions before final recommendations.
- Preserve an evidence trail for each key claim (document/page/section reference).
- Prefer reversible, low-regret actions when risk is uncertain.

## Escalation Triggers

Escalate to licensed legal counsel when any of the following are true:

- Cross-border, regulatory, IP, employment, privacy, or litigation-sensitive issues.
- Financial or reputational downside could be material.
- Contract language is ambiguous in high-impact clauses.
- Deadlines involve formal legal submission or enforcement windows.
