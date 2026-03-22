# Adoption Guide

Use this guide when adopting Product to Build OS in a new project repo.

## Goal
- Install the methodology with the smallest useful set of role files, process docs, and instantiated project artifacts.
- Keep the project repo lightweight and documentation-driven.

## Recommended Adoption Sequence
1. Copy the role entry files into the new project repo:
   - `KADE.md`
   - `MASON.md`
   - `LEDGER.md`
   - `CASE.md`
   - `AGENT_MODEL.md`
2. Copy the core process docs the project wants to enforce:
   - `docs/process/AGENT_RULES.md`
   - `docs/process/ENGINEERING_WORKFLOW.md`
   - `docs/process/DEFINITION_OF_DONE.md`
   - `docs/process/REQUIRED_PROJECT_ARTIFACTS.md`
   - `docs/process/SPRINT_GOVERNANCE_REVIEW.md`
   - `docs/process/HANDOFFS_AND_ESCALATION.md`
3. Copy the templates needed for project-local instantiation.
4. Instantiate the required project-local artifacts.
5. Update the project's documentation map so contributors can find the active artifacts quickly.
6. Start sprint work only after the instantiated sprint-start artifacts exist.

## Minimum Project-Local Instantiation
At minimum, the project repo should instantiate:
- current state
- decisions log
- drift log
- worklog
- sprint specs
- Technical Implementation Plan
- Acceptance / Test Plan
- Sprint Governance Review record
- documentation map

## Non-Negotiable Sprint Start Rule
Before Mason starts sprint implementation, the active sprint must have instantiated working artifacts for:
- Technical Implementation Plan
- Acceptance / Test Plan
- Sprint Spec

Template files alone do not satisfy this requirement.

## Practical Adoption Advice
- Start with the minimum artifact set and add architecture, deployment, API, and runbook docs only when the project actually needs them.
- Keep the role model explicit from the first day of the project.
- Keep handoffs visible in the docs rather than relying on implied ownership.
