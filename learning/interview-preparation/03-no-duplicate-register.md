# HR Tech Interview Preparation — No-Duplicate Register

## Rule

No duplicate scenario content across the HR ecosystem.

Existing detailed stream repositories remain the source of truth for their own content.

## Decision Logic

1. Exact duplicate — do not create.
2. Same competency and same scenario — do not create.
3. Same competency with materially different context — may create.
4. Same question with only wording changed — do not create.
5. Existing scenario that satisfies a BAISI theme — map it first.
6. Cross-stream scenario is allowed only when the architecture interaction itself is the competency.

## Required Audit Locations

• nbnayak88/autonomous-hr
• relevant 12 domain repositories
• labs/11-scale-school-of-career-acceleration
• existing Interview Preparation / SCALE folders
• existing 20-unit / 22-step mastery journeys

## Existing verified example

SAP SuccessFactors Onboarding contains a 22-step interview/mastery journey and detailed scenario-based interview files.

That content must be cross-mapped, not regenerated.

## Unique ID

HR-[STREAM]-B[THEME]-Q[NUMBER]

## Evidence before creation

• searched source repositories
• identified nearest existing scenario
• recorded why the new scenario is materially different
• assigned one BAISI theme
• assigned one stream
• assigned one stable ID

Principle: Audit first. Map second. Create only the gap.
