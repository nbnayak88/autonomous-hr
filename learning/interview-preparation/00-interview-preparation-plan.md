# HR Tech Interview Preparation — BAISI PAHACHA Master Plan

## North Star
Build HR Tech Interview Preparation using the same structural discipline as the Finance interview-preparation architecture, while reusing existing HR repository assets.

Target progression:
HR Practitioner → HR Technology Consultant → HR Tech Solution Architect → HR Transformation Architect → Trusted HR Tech Advisor

Interview journey:
Understand HR → Understand HR Technology → Design → Integrate → Implement → Validate → Operate → Transform → Advise

## 1. Canonical Architecture

12 HR Tech Streams:
01 AWF1 — HCM Core & Employee Central
02 ATA2 — Recruiting & Talent Acquisition
03 APH3 — Performance, Goals & Talent
04 AGL4 — Succession & Career Development
05 ARP5 — Compensation & Rewards
06 ALM6 — Learning & Development
07 APE7 — Payroll & Workforce Management
08 AWT8 — Time Operations
09 AWI9 — HR Analytics & People Intelligence
10 ADX0 — Employee Experience
11 AAI1 — AI-Powered HR
12 AIG2 — Connected HR / Integration

## 2. BAISI PAHACHA — 22 Interview Themes

KNOW
01 Domain Foundation
02 Product / Technology Knowledge
03 Process & Business Context
04 Data & Information Model

DESIGN
05 Requirement Analysis
06 Solution Design
07 Configuration / Development
08 Integration & Architecture

DELIVER
09 Testing & Quality Assurance
10 Deployment & Release
11 Migration & Cutover
12 Operations & Support

SOLVE
13 Troubleshooting & Root Cause Analysis
14 Scenario-Based Problem Solving
15 Risk, Controls & Security
16 Performance & Optimization

INFLUENCE
17 Stakeholder Management
18 Communication & Consulting
19 Presales / Leadership / Decision Making

TRANSFORM
20 Transformation & Roadmap
21 Innovation & Emerging Technology
22 Enterprise Architecture & Business Value

These are assessment dimensions, not generic lessons. Every scenario must be HR-Tech-specific to its owning stream.

## 3. Target Scenario Architecture

12 Streams × 22 BAISI Pahacha Themes × 20 STAR Scenarios = 5,280 scenario positions.

Scenario format:
Question → Situation → Task → Action → Result → SME Probe → Reflection

Action should demonstrate relevant combinations of:
Business → Process → People → Data → Technology → Integration → Security → Experience → Outcome

## 4. No-Duplicate Gate

Before creating any scenario:
1. Search the HR master repository.
2. Search the relevant domain repository.
3. Check the SCALE / Interview Preparation folder.
4. Check existing 20-unit / 22-step mastery files.
5. Check whether an equivalent scenario already exists.
6. If it exists, reuse and map it; do not recreate it.
7. Create only genuine coverage gaps.

Stable ID:
HR-[STREAM]-B[THEME]-Q[01-20]

## 5. Existing Content Reuse

Verified example: SAP SuccessFactors Onboarding already contains a mature 22-step interview journey and detailed scenario-based interview files.

Existing ONB content will be cross-mapped into the BAISI Pahacha assessment themes rather than rewritten.

The ONB 22-step journey and the BAISI Pahacha 22-theme assessment model must not be assumed to be identical. Coverage must be mapped before counting.

## 6. Repository Strategy

Use nbnayak88/autonomous-hr as the orchestration/reference layer.

Do not copy detailed stream content into the master repository.

Recommended master layer:
learning/interview-preparation/
README.md
00-interview-preparation-plan.md
01-baisi-pahacha-22-theme-framework.md
02-coverage-matrix.md
03-no-duplicate-register.md
streams/
mappings/

Detailed scenario content remains in the owning stream repository unless centralization is justified.

## 7. Build Sequence

Phase 1 — Architecture & Audit
• establish the 22-theme framework
• establish the 12-stream matrix
• audit existing interview assets
• build crosswalk
• establish duplicate control

Phase 2 — Coverage
For each stream, map existing scenarios, identify missing themes, weak STAR coverage, missing architecture dimensions and missing SME probes.

Phase 3 — Scenario Creation
Create only missing scenarios. Each completed theme should contain 20 unique scenario-based questions, STAR answers, SME probes, reflection prompts, architecture signals, anti-patterns and quality gates.

Phase 4 — Cross-Stream Mastery
Add only genuinely cross-stream scenarios such as EC ↔ Recruiting, EC ↔ Onboarding, EC ↔ Payroll, Compensation ↔ Payroll, HR ↔ Finance, HR ↔ Identity, HR ↔ Integration Suite, HR ↔ Analytics and HR ↔ AI.

Phase 5 — Capstone
Design a Connected & Intelligent HR Enterprise using Business, Process, Data, Application/Solution, Integration, Security, Experience, AI, Technology, Industry and Enterprise architecture lenses.

## Definition of Done

All 12 streams have BAISI Pahacha coverage; existing content is reused; missing coverage is explicit; new themes have 20 unique STAR scenarios; cross-stream architecture is tested; and the final capstone demonstrates transformation and business value.

Principle: Audit first. Map second. Create only the gap.
