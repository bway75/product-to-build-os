# Product to Build OS

Reusable operating model for turning product definition into implementation-ready sprint execution.

This repo is the methodology layer, not a project repo. It defines:
- role-based startup files
- workflow and governance rules
- project adoption guidance
- product-to-engineering handoff expectations
- templates for the instantiated artifacts each project must create

## What This Repo Is For
- Establish a lightweight, documentation-driven operating model
- Preserve explicit handoffs between product, technical shaping, implementation, validation, and governance
- Give Mason, Case, and Ledger clear rules for what must exist before sprint work starts
- Require each adopting project to maintain its own instantiated artifacts

## What This Repo Is Not
- It does not contain project-specific current state, decisions, drift, worklog, sprint specs, architecture, deployment, API, or environment docs.
- It does not contain application code, infrastructure code, or runtime implementation.
- It does not replace a project's own repo-local artifacts.

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

## Required Project Artifacts
Every project repo that adopts this OS should create and maintain its own instantiated project artifact set, including:
- `docs/CURRENT_STATE.md`
- `docs/DECISIONS.md`
- `docs/DRIFT_NOTES.md`
- `docs/WORKLOG.md`
- `docs/sprints/`
- instantiated Technical Implementation Plans
- instantiated Acceptance / Test Plans
- instantiated Sprint Governance Review records
- `docs/DOCUMENTATION_MAP.md`

Projects should also create architecture, deployment, API, integration, and runbook docs when those concerns exist.
Teams can start with this minimum required artifact set and expand the process only as project complexity requires.

Template files alone do not satisfy sprint-start requirements. Before implementation begins, the active sprint must have instantiated working artifacts for:
- Technical Implementation Plan
- Acceptance / Test Plan
- Sprint Spec

## Read This First
- [AGENT_MODEL.md](AGENT_MODEL.md)
- [docs/DOCUMENTATION_MAP.md](docs/DOCUMENTATION_MAP.md)
- [docs/process/ADOPTION_GUIDE.md](docs/process/ADOPTION_GUIDE.md)
- [docs/process/PROJECT_BOOTSTRAP_CHECKLIST.md](docs/process/PROJECT_BOOTSTRAP_CHECKLIST.md)
- [docs/process/ENGINEERING_WORKFLOW.md](docs/process/ENGINEERING_WORKFLOW.md)
- [docs/process/AGENT_RULES.md](docs/process/AGENT_RULES.md)
- [docs/process/HANDOFFS_AND_ESCALATION.md](docs/process/HANDOFFS_AND_ESCALATION.md)
- [docs/process/REQUIRED_PROJECT_ARTIFACTS.md](docs/process/REQUIRED_PROJECT_ARTIFACTS.md)

## Role Entrypoints
- [KADE.md](KADE.md)
- [MASON.md](MASON.md)
- [LEDGER.md](LEDGER.md)
- [CASE.md](CASE.md)

## Templates
- [docs/templates/TECHNICAL_IMPLEMENTATION_PLAN_TEMPLATE.md](docs/templates/TECHNICAL_IMPLEMENTATION_PLAN_TEMPLATE.md)
- [docs/templates/ACCEPTANCE_TEST_PLAN_TEMPLATE.md](docs/templates/ACCEPTANCE_TEST_PLAN_TEMPLATE.md)
- [docs/templates/SPRINT_SPEC_TEMPLATE.md](docs/templates/SPRINT_SPEC_TEMPLATE.md)
- [docs/templates/CURRENT_STATE_TEMPLATE.md](docs/templates/CURRENT_STATE_TEMPLATE.md)
- [docs/templates/DECISIONS_LOG_TEMPLATE.md](docs/templates/DECISIONS_LOG_TEMPLATE.md)
- [docs/templates/DRIFT_LOG_TEMPLATE.md](docs/templates/DRIFT_LOG_TEMPLATE.md)
- [docs/templates/WORKLOG_TEMPLATE.md](docs/templates/WORKLOG_TEMPLATE.md)
- [docs/templates/SPRINT_GOVERNANCE_REVIEW_TEMPLATE.md](docs/templates/SPRINT_GOVERNANCE_REVIEW_TEMPLATE.md)
- [docs/templates/DOCUMENTATION_MAP_TEMPLATE.md](docs/templates/DOCUMENTATION_MAP_TEMPLATE.md)
