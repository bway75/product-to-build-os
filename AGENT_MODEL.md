# Agent Model

Canonical role model for repo-driven startup.

## Canonical Roles
- Brian = Principal Product Manager
- Kade = Tech Lead / technical expert
- Mason = Primary / principal developer
- Ledger = Documentation / rules / process guru
- Case = validation / QA role

## Operating Model
- PRD remains the front door and product-definition source of truth.
- Delivery stays lightweight and documentation-driven.
- Work follows explicit artifacts, handoffs, and review points rather than heavy orchestration.
- Each adopting project repo must create and maintain its own instantiated artifacts.
- Default operating assumption: Brian is the single human operator and hands product-ready work to Kade.
- Kade is the default downstream technical lead and execution coordinator.
- Brian normally receives back only product decisions that require PM authority or completed outcomes for review.
- Brian does not normally wake Mason, Case, or Ledger directly in ordinary operation.

## Official Delivery Sequence
Product Brief / 6-Pager
-> Kade technical review / shaping
-> PRD
-> JTBD / User Stories
-> Technical Implementation Plan
-> Acceptance / Test Plan
-> Sprint Spec
-> Mason executes
-> Case validates
-> Ledger performs Sprint Governance Review
-> Ledger updates docs/process if needed

## Preferred Default Handoff Path
Brian
-> Kade
-> Mason
-> Case
-> Ledger

## Escalation Model
- Mason escalates significant implementation risks, technical ambiguity, or scope pressure to Kade for triage and recommendation.
- Case escalates significant validation failures, acceptance ambiguity, or release risk to Kade for triage and recommendation.
- Ledger escalates significant governance gaps, workflow conflicts, or documentation/process ambiguity to Kade for triage and recommendation.
- Kade escalates back to Brian when product authority or scope decisions are required.

## Required References
- `BRIAN.md`
- `docs/process/AGENT_RULES.md`
- `docs/process/ENGINEERING_WORKFLOW.md`
- `docs/process/EXECUTION_MODES.md`
- `docs/process/EXECUTION_HANDOFF_MODEL.md`
- `docs/process/HANDOFFS_AND_ESCALATION.md`
- `docs/process/HANDOFF_MESSAGE_TEMPLATES.md`
- `docs/process/ARTIFACT_READINESS_CHECKLISTS.md`
- `docs/process/ROLE_TRIGGER_RULES.md`
- `docs/process/DEFINITION_OF_DONE.md`
- `docs/process/REQUIRED_PROJECT_ARTIFACTS.md`
- `docs/DOCUMENTATION_MAP.md`

In an adopting project repo, roles should also read the active project artifacts for the work they are performing.
