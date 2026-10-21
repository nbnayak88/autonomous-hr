# Autonomous HR — Origin Story Source Template

> Version: 1.0 | Status: Planning source of truth | Owner: SuccessLabs Academy
> Scope: Universal, platform-independent interactive-learning specification
> Initial reference course: SAP SuccessFactors Compensation — The Origin Story
> Levels: Origin Story → Pre-Foundation → Foundation → Intermediate → Advanced → Ultimate
> Build targets: Lovable, Vercel, Google AI Studio, Emergent, and comparable AI coding platforms

## 1. Mission

Build a scalable, accessible, delightfully minimalist interactive learning application where **every lesson ends in a meaningful action**. Never unlock the next mission solely because content was viewed or a timer expired.

**Progression contract:** Discover → Act → Submit evidence → Validate → Give feedback → Unlock.

The product must be reusable across SAP modules, enterprise functions, architecture streams, industry contexts, and learning townships. Initial scope is only the Origin Story level; other levels are defined for planning, not implemented in the MVP.

## 2. Learning philosophy and outcomes

- Reduce passive consumption; maximize discovery and practice.
- One primary objective and one principal call to action per screen.
- Favor curiosity, useful feedback, reflection, and incremental mastery over rigid syllabi.
- Keep learners oriented: where am I, what should I do, why does it matter, what unlocks next?
- Provide a recoverable failure loop: feedback → hint → revise → retry.
- Gamify with mastery points, micro-celebrations, earned badges, and opt-in leaderboards. Avoid punitive streak pressure, manipulation, or shame.
- Make accessibility foundational: keyboard navigation, screen-reader labels, strong contrast, reduced motion, captions, and touch targets.
- Compare student outcomes and feedback across build platforms using the same specification and test protocol.

### Origin Story outcome

Learners recognize **why a product exists**, the business problem it solves, how it evolved, its high-level capabilities, its role in an enterprise solution landscape, and where it might create value in their industry.

### Six-level ladder

| Level | Dominant action | Typical evidence |
| --- | --- | --- |
| The Origin Story | Discover, distinguish, explain | Problem statement, timeline, reflection |
| Pre-Foundation | Identify, interpret, map | Business process map |
| Foundation | Analyze and model | Solution blueprint |
| Intermediate | Configure and test | Working configuration plus test evidence |
| Advanced | Design and optimize | Enterprise implementation case |
| Ultimate | Synthesize, innovate, defend, mentor | Production-grade architecture, innovation portfolio, peer review |

Ultimate is a future learning level; do not expose it as a completed pathway in the Origin Story MVP.

## 3. Initial course configuration

| Attribute | Value |
| --- | --- |
| Enterprise platform | SAP |
| Domain | Human Capital Management |
| Product | SAP SuccessFactors Compensation |
| Architecture stream | Applied Application Architecture (AA) |
| Lab track | PIL — Product Innovation Lab |
| Learning intent | Discover |
| Industry | Energy |
| Starting level | The Origin Story |
| Target level | Pre-Foundation |
| Target active duration | 120 minutes |
| Learning model | Eight sequential, evidence-gated missions |
| Completion | Every mission passed and final reflection submitted |

### One-sentence learning promise

“In two hours, explain the origin, purpose, evolution, product landscape, and basic application architecture of SAP SuccessFactors Compensation, then apply that understanding to an energy company.”

## 4. Universal mission engine

Each mission MUST have:

1. Stable ID, title, estimate, instructional intent, and prerequisite IDs.
2. Curiosity hook or realistic scenario.
3. Micro-content with a concise concept and optional authoritative resources.
4. A learner **action** that creates measurable evidence.
5. Explicit pass criteria or rubric.
6. Feedback explaining what was demonstrated and what to improve.
7. Retry path, hint, and save/resume support.
8. A verified completion state that unlocks the next mission.

### State machine

`locked → available → in_progress → submitted → (needs_revision | passed) → completed`

- `locked`: prerequisite requirements unmet.
- `available`: all prerequisites met.
- `in_progress`: started and draft autosaved.
- `submitted`: evidence captured, grading pending.
- `needs_revision`: criteria not met; provide actionable feedback.
- `passed`: grading criteria satisfied.
- `completed`: durable record written; next mission eligible to unlock.

Never trust only a client-side “Next” button for gate enforcement. Persist authoritative progress server-side in production. Keep grading results and events auditable.

## 5. SAP SuccessFactors Compensation — eight-mission Origin Story sprint

The following are approximate active learning budgets, totaling 120 minutes.

| # | Minutes | Mission | Learner action | Evidence / gate |
| --- | ---: | --- | --- | --- |
| 01 | 10 | Discover the Problem | Identify spreadsheet-based compensation risks for an energy company | Three distinct risks with impacts; rubric pass |
| 02 | 20 | Explore the Evolution | Build an evolution story from manual reviews to strategic rewards | Four logically ordered stages with explanations |
| 03 | 20 | Decode the Product | Distinguish Compensation Planning, Variable Pay, and Reward and Recognition | Match each capability to realistic use cases; ≥80% |
| 04 | 25 | Map the Architecture | Draw major inputs, actors, systems, approvals, and outcomes | Employee data, Compensation, HR/managers, approvals, downstream outputs |
| 05 | 20 | Apply to Energy | Solve an annual salary review scenario at fictional OmniVerse Energy | Written rationale; ≥80% rubric |
| 06 | 15 | Analyze Dependencies | Map data ownership, integration, confidentiality, and governance | Dependency matrix with risks and controls |
| 07 | 5 | Demonstrate Understanding | Complete a short scenario-based knowledge check | ≥80%; retry with feedback |
| 08 | 5 | Reflect and Commit | Explain the product in plain language and identify one open question | Concise submission accepted |

### Mission 01 — Discover the Problem

**Hook:** OmniVerse Energy employs 8,000 people across plants, engineering, field operations, and corporate functions. Annual salary recommendations circulate in spreadsheets.

**Learn:** Budget overruns, inconsistent decisions, manual consolidation, limited traceability, fragmented approvals, and exposure of sensitive pay data.

**Action:** Identify three distinct business risks and explain why structured compensation planning helps.

**Feedback:** Praise the specific risk-impact connection; if an answer only lists features, ask for business consequences.

### Mission 02 — Explore the Evolution

**Learn:** Conceptual progression: manual administration → structured salary planning → integrated enterprise processes → strategic total rewards. Clarify that these are conceptual stages, not asserted SAP release milestones.

**Action:** Arrange four stages, match each to the corresponding business pain point, and write a two-sentence evolutionary narrative.

**Gate:** Correct sequence and meaningful explanations.

### Mission 03 — Decode the Product

**Learn:** 
- Compensation Planning: salary review and relevant long-term incentive planning.
- Variable Pay: short-term incentive compensation planning.
- Reward and Recognition: cash/points-based recognition programs.
- Employee Central compensation information: employee-related master information, distinct from planning workflows.

**Action:** Classify sample energy-sector scenarios and justify a tricky boundary case.

**Gate:** ≥80% and correct explanation of the difference between a planning workflow and an employee record.

### Mission 04 — Map the Architecture

**Learn:** Conceptual ecosystem: workforce context / Employee Central → compensation review setup → budget and eligibility → manager worksheets → review/approval → finalization → appropriate employee record or downstream process. Real implementations differ.

**Action:** Assemble a diagram with components and labeled arrows.

**Gate:** Required nodes and relationships present. Do not require a specific vendor integration pattern without evidence.

### Mission 05 — Apply to Energy

**Hook:** A multinational energy company must review salaries across engineering, plant operations, and corporate roles while respecting budgets, employment conditions, and confidentiality.

**Action:** Recommend a high-level operating approach: stakeholders, major process steps, differentiated populations, budget checks, approvals, and expected outputs.

**Gate:** Clear response to the business problem, realistic scope, sound controls, and accurate application boundaries.

### Mission 06 — Analyze Dependencies

**Action:** Complete a matrix with columns `data element | source of truth | consuming process | risk | control`. Cover employee hierarchy, current compensation, eligibility, approved changes, and downstream integration.

**Gate:** Correctly identify ownership questions, data quality, access control, and delivery validation.

### Mission 07 — Demonstrate Understanding

**Action:** Answer five questions about the business need, the three product areas, manager worksheet purpose, Employee Central relationship, and architect responsibilities.

**Gate:** Four out of five correct, with formative feedback and retry.

### Mission 08 — Reflect and Commit

**Action:** Give a three-minute-equivalent plain-language explanation (written or recorded), identify one unknown, and select a next exploration question.

**Gate:** Evidence submitted and accepted. Award the Origin Story completion badge only after all preceding gates pass.

## 6. Shared mission screen UX

Use Apple-inspired design principles **without copying proprietary Apple assets or interfaces**:

- Intentional whitespace; clear hierarchy; calm typography; neutral surface palette and one restrained accent.
- Single primary CTA; no dense dashboards during a mission.
- Tiny progress indicator (“Mission 3 of 8”), estimated effort, and an obvious Back/Save option.
- Micro-interactions are short, optional, and reduced-motion aware.
- Short information cards, progressive disclosure, accessible drag-and-drop alternatives.
- No autoplay sound, surprise modals, hard-to-dismiss overlays, or leaderboard distractions.
- Positive, specific feedback; failures are learning opportunities rather than punishments.
- Navigation must make locked steps visible but not actionable, with clear unlock requirements.
- Mobile-first responsive behavior; full keyboard support on desktop.

### Screens

1. Welcome and learning promise.
2. Minimal course map (eight missions; locked/unlocked state).
3. Active mission: hook → micro-lesson → action → evidence entry.
4. Results: pass, specific feedback, reward, next unlock.
5. Revision: why not yet passed, targeted hint, retry.
6. Lightweight progress view and optional competition panel.
7. Final completion reflection and next-level preview.
8. Author preview for course creators.

## 7. Engagement system

- Mastery points awarded **only** for valid actions, not page views.
- Optional streaks should support flexibility (grace period and easy recovery), never penalize life interruptions.
- Badges: Problem Spotter, Evolution Explorer, Product Decoder, Architecture Mapper, Energy Strategist, Dependency Detective, Concept Communicator.
- Healthy competition: opt-in cohorts, transparent point calculation, anonymized display names, no public failure rankings.
- Curiosity prompts: “What could go wrong?”, “Which system owns the decision?”, “Why did the industry need this?”
- Explainability: show the rubric for assessed work and why feedback was produced.
- Avoid incentivizing meaningless rapid clicking, repeated guessing, or inflated participation.

## 8. Content architecture for scaling

**Curriculum as data, app as engine.** Separate course-specific JSON/Markdown from reusable UI and validation logic.

Suggested structure:

```text
autonomous-hr/
  Origin-Story/
    source-template.md
    courses/
      sap-successfactors-compensation/
        course.json
        missions/
          01-discover.md
          02-evolution.md
          03-product.md
          04-architecture.md
          05-energy.md
          06-dependencies.md
          07-knowledge-check.md
          08-reflection.md
  app/
    components/
    engine/
    data/
    integrations/
    tests/
```

Suggested course schema:

```json
{
  "id": "sap-sf-comp-origin",
  "title": "SAP SuccessFactors Compensation — The Origin Story",
  "platform": "SAP",
  "domain": "HCM",
  "product": "SAP SuccessFactors Compensation",
  "learningLevel": "origin-story",
  "targetLevel": "pre-foundation",
  "architectureStream": "AA",
  "labTrack": "PIL",
  "learningIntent": "Discover",
  "industry": "Energy",
  "durationMinutes": 120,
  "sequenceMode": "mastery-gated",
  "missions": [
    {"id":"01","title":"Discover the Problem","durationMinutes":10,"prerequisites":[]},
    {"id":"02","title":"Explore the Evolution","durationMinutes":20,"prerequisites":["01"]},
    {"id":"03","title":"Decode the Product","durationMinutes":20,"prerequisites":["02"]},
    {"id":"04","title":"Map the Architecture","durationMinutes":25,"prerequisites":["03"]},
    {"id":"05","title":"Apply to Energy","durationMinutes":20,"prerequisites":["04"]},
    {"id":"06","title":"Analyze Dependencies","durationMinutes":15,"prerequisites":["05"]},
    {"id":"07","title":"Demonstrate Understanding","durationMinutes":5,"prerequisites":["06"]},
    {"id":"08","title":"Reflect and Commit","durationMinutes":5,"prerequisites":["07"]}
  ]
}
```

Suggested mission schema fields: `id, title, learningIntent, hook, concepts, resourceLinks, prompt, evidenceType, rubric, passThreshold, prerequisites, estimatedMinutes, hints, feedbackRules, points, badge, accessibilityAlternative`.

Suggested relational entities: `courses`, `missions`, `learners`, `enrollments`, `attempts`, `evidence`, `evaluations`, `completion_events`, `cohorts`, `feedback`. Record timestamps and rubric versions.

## 9. Assessment and gating requirements

- Multiple choice: deterministic server-side scoring.
- Ordering, matching, and sorting: deterministic scoring.
- Writing: rubric-based grading with explicit evidence expectations; if AI grading is used, permit human review and record model/rubric version.
- Diagrams: evaluate required entities and labeled relationships; consider structured node/edge input for reliable assessment.
- Audio/video: provide accessible text alternative; do not claim transcription or scoring without a configured service.
- Prevent bypass by changing URLs, refreshing, or clearing local state.
- After passing, store the completion event and make the next mission available.
- Support repeated submissions while retaining history and latest accepted evidence.
- Prevent duplicate points for retries; no reward farming.
- Privacy: protect employee, learner, and assessment data; never use real compensation records in demos.

## 10. SAP SuccessFactors Learning integration planning

Deploy a standalone interactive app first. LMS integration is a distinct production phase.

Candidate approaches:
- SCORM-compatible packaging when the deployment model and runtime support it.
- Supported integration via the customer's Learning environment and approved standards/APIs.
- Track completion and score without marking completion merely on content launch.

Before go-live, test bookmarking, session resume, gating persistence, pass/fail status reporting, mobile behavior, accessibility, and the actual tenant's supported content settings. Do not imply direct LMS integration exists in the MVP.

## 11. Learner research and platform bake-off

Build the **same course**, using the **same eight missions, copy, rubric, and success criteria**, on Lovable, Vercel, Google AI Studio, Emergent, or other contenders. Compare outcomes rather than appearance alone.

### Metrics

- Time to first meaningful action.
- Mission-1 completion rate.
- Overall completion rate.
- Fraction of learners who can give an accurate plain-language explanation.
- Number of retries and eventual mastery rate.
- Resume success after exit.
- Usability score and cognitive load.
- Mobile usability and accessibility defects.
- Learner-reported curiosity, autonomy, and desire to continue.
- Developer time, maintainability, portability, exportability, and operational cost.

### Feedback questions

1. What did you expect to happen next?
2. At what point did you feel confused?
3. Did each action help you understand the product?
4. Did the feedback help you improve?
5. Were badges and competition motivating or distracting?
6. Would you voluntarily start the next mission?
7. What single change would most improve this experience?

Use opt-in consent for analytics and feedback. Avoid collecting unnecessary personal information.

## 12. One-hour prototype sprint

| Time | Task | Deliverable |
| --- | --- | --- |
| 0–10 min | Upload this file; generate navigation and design tokens | Welcome + mission map |
| 10–25 min | Implement missions 1–3 using structured content | Three functional actions |
| 25–40 min | Add submission, rubric feedback, persistence, server-side gate validation | Reliable unlock flow |
| 40–50 min | Polish mobile, keyboard accessibility, copy, and reduced-motion mode | Usable prototype |
| 50–60 min | Test fail → retry → pass → exit → resume; capture first learner impressions | Demo + defect list |

**One-hour build scope:** working vertical slice of the first three missions, not production-ready LMS integration, all eight mission authoring workflows, or complete analytics.

## 13. Master AI vibe-coding prompt

Copy the prompt below into any supported AI app-building tool. Give this file as the source of truth.

```text
Build a mobile-first interactive learning application called "Autonomous HR — Origin Story" for SuccessLabs Academy.

Use the accompanying Origin-Story/source-template.md as the authoritative product, curriculum, and interaction specification. This is a universal engine that will later serve many courses and industry townships. Seed it with the SAP SuccessFactors Compensation Origin Story course (AA stream, PIL Discover, Energy industry), lasting 120 minutes across eight mastery-gated missions.

Design: Apple-inspired minimalist principles: generous white space, calm neutral colors, legible system typography, one distinct CTA per screen, subtle progress, rounded surfaces used sparingly, zero visual clutter. Duolingo-inspired short actions, specific feedback, earned progress, curiosity and healthy opt-in competition; avoid copying either company's visual assets.

Core app screens: welcome; mission map; lesson; interactive action; evidence submission; contextual feedback/retry; successful completion/unlock; progress; course completion. Show future levels (Pre-Foundation, Foundation, Intermediate, Advanced, Ultimate) as a roadmap, not as available lessons.

Build a reusable curriculum engine driven by typed JSON/Markdown schema instead of hardcoding eight independent pages. Persist progress, attempts, evidence and completion. Enforce prerequisites from the authoritative state, not only disabled UI buttons. Support retries, hints, autosave and resume. For MVP, provide structured exercises and deterministic scoring for missions 1–3; scaffold the remaining five faithfully. Do not present mock auto-grading, LMS connectivity, or leaderboard backends as live.

Use accessible, responsive components and keyboard-operable interactions. Respect reduced motion. Provide realistic fictional energy-sector examples; never request real employee salary data. Include useful seed content, unit tests for gates and scoring, and a README with local run/deploy instructions.

Deliver a functional preview, explain what is real vs stubbed, and provide a concise backlog. Prioritize the learner's first successful action over decorative dashboards.
```

## 14. Definition of done

### One-hour prototype

- [ ] Learner lands on a clean course welcome page.
- [ ] Can enter mission 1 immediately.
- [ ] At least three missions have meaningful interactions.
- [ ] Incomplete/failed mission cannot unlock the next.
- [ ] Correct completion unlocks exactly the next eligible mission.
- [ ] Progress survives refresh/revisit.
- [ ] Failed answer provides useful correction and retry.
- [ ] No more than one dominant action per screen.
- [ ] Mobile and keyboard journeys function.
- [ ] Clearly label mock integrations and prototype-only scoring.

### Full Origin Story pilot

- [ ] All eight missions functional.
- [ ] Course-specific data is separate from UI logic.
- [ ] All assessments meet the declared rubrics.
- [ ] Learner can exit and resume accurately.
- [ ] Learner can finish and explain the product in three minutes.
- [ ] Feedback collection is consent-based.
- [ ] LMS integration is documented and tenant-tested before activation.
- [ ] Outcome metrics can be compared across build platforms.

## 15. Content governance

- This file is the reusable **source template**. Keep it platform-neutral and version-controlled.
- Specific courses should live in separate files and reference this template.
- Review SAP terminology and current product capabilities against official SAP Learning and SAP Help materials during course updates.
- Use fictional examples; avoid embedding actual learner or employee sensitive data.
- Document design decisions, rubric modifications, and migration implications in version history.
- Maintain a change log and use peer review for substantive updates.

## 16. Key principle

> **One discovery. One action. One demonstrated outcome. One earned unlock.**

Scale the content library, not learner cognitive load.
