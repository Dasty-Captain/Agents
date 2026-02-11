---
name: reference-find
description: Find, validate, and rank high-quality references to support or challenge a thesis with precise citation details.
---

# Reference Find

Use this skill to locate the strongest possible references for a thesis, including exact source location details and reliability ranking.

## When to Use This Skill

- The user asks for citations to support a claim or thesis.
- The user needs source validation before publishing.
- The user needs contradictory or balancing references.
- The user requests deep-research style evidence collection.

## Outcomes

- A ranked reference set with direct links and relevance rationale.
- Claim-to-source mapping for fast verification.
- Citation-ready outputs with confidence and risk notes.

## Required Inputs

- Thesis or claim set to support/check.
- Preferred domains or excluded domains (if any).
- Evidence standard (academic, policy, industry, legal, journalistic).
- Citation style (APA, MLA, Chicago, inline URL, etc.) if required.

If inputs are missing, ask only for the minimum needed values.

## Workflow

1. Decompose thesis into atomic claims.
2. Build search queries per claim using synonyms and counter-terms.
3. Retrieve candidate sources from diverse, credible domains.
4. Validate each source for authority, recency, and methodological quality.
5. Extract precise citation context (page/section/paragraph when available).
6. Rank sources by tier:
   - Tier 1: Primary/official/high-authority evidence
   - Tier 2: Strong secondary synthesis with clear methodology
   - Tier 3: Contextual or directional support only
7. Produce both supportive and contradictory references where relevant.

## Output Format

Return in this exact section order:

1. Thesis and Claim Breakdown
2. Search Strategy
3. Tiered Reference List
4. Claim-to-Citation Map
5. Contradictory Evidence
6. Citation Quality Risks
7. Recommended Core Citation Set

For each reference, include:

- Reference title
- Why it is relevant
- Reliability tier
- Publication date
- Direct URL
- Exact location details (page/section/paragraph if available)

## Guardrails

- Do not cite sources that cannot be directly accessed or verified.
- Do not hide contradictory evidence.
- Mark weak or indirect citations clearly.
- Prefer original sources over derivative summaries.
