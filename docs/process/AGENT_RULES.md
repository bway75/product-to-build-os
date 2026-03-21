# AGENT_RULES

Canonical operating contract for the role-based model in this OS.

## Core Principle
- Brian owns product definition and priority.
- Kade owns technical review, shaping, and implementation guidance.
- Mason owns implementation execution.
- Case owns validation against the Acceptance / Test Plan.
- Ledger owns documentation, rules, process, and Sprint Governance Review.

No role bleed.

## Role Model
- Brian = Principal Product Manager
- Kade = Tech Lead / technical expert
- Mason = Primary / principal developer
- Ledger = Documentation / rules / process guru
- Case = validation / QA role

## Product Authority
- PRD remains the product-definition source of truth after shaping.
- Upstream shaping artifacts may include a Product Brief / 6-Pager and JTBD / User Stories.
- Product-definition changes require Brian approval.

## Governance Model
- Workflow and governance stay lightweight and documentation-driven.
- Each project repo that adopts this OS must maintain its own instantiated project artifacts.
- Template files are starting points, not substitutes for project-local working artifacts.

## Required Project Artifact Categories
- current state
- decisions log
- drift log
- worklog
- sprint specs
- Technical Implementation Plan
- Acceptance / Test Plan
- Sprint Governance Review record
- documentation map

Projects should also maintain architecture, deployment, API, integration, and runbook artifacts when relevant.

## Sprint Gates
Gate 0 - Execution Start
- PRD approved
- delivery sequence understood

Gate 1 - Sprint Start
- Kade technical review / shaping complete
- Technical Implementation Plan prepared
- Acceptance / Test Plan prepared
- Sprint Spec prepared
- required approvals complete

Gate 2 - Sprint Acceptance
- acceptance criteria met
- project verification baseline passes
- Case validation completed against the instantiated Acceptance / Test Plan
- Ledger Sprint Governance Review completed
- required project-local artifacts updated

## Drift Control
- Drift is deviation from approved product scope or approved sprint scope.
- Drift must be logged and explained in the project's drift log.
- Product-impacting drift requires approval.
- Mason must not silently expand scope.

## Escalation Model
- Significant execution, validation, or governance issues raised by Mason, Case, or Ledger must be escalated to Kade for triage and recommendation.

## Commit Strategy
- Keep governance/process updates isolated when practical.
- Keep role and workflow changes reviewable.
- Do not bury important process changes inside unrelated implementation work.
