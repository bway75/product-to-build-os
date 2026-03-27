# Engineering Workflow

Official product-to-engineering delivery workflow for teams using this OS.

## Execution Model
- Main should remain stable.
- Default execution model is main-only unless a project explicitly chooses a different policy.
- Delivery stays lightweight and documentation-driven.
- PRD remains the front door and product-definition source of truth.

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

## Pre-Sprint Start Gate
Before sprint implementation starts:
- confirm Kade technical shaping is complete for the planned sprint scope
- confirm the PRD remains the authoritative product-definition source for the work
- confirm JTBD / User Stories exist when they are part of the product handoff
- confirm a Technical Implementation Plan exists and is the implementation handoff into sprint execution
- confirm an Acceptance / Test Plan exists and is the validation handoff for Case
- confirm a Sprint Spec exists and is the authoritative execution scope
- before sprint implementation starts, the following execution artifacts must exist for the sprint:
  - Technical Implementation Plan
  - Acceptance / Test Plan
  - Sprint Spec
- template files alone do not satisfy this requirement; the sprint must have instantiated working artifacts

## During Sprint Development
- Mason executes against the Sprint Spec, Technical Implementation Plan, and accepted product scope
- Tests must be written before implementation for application behavior changes (RED-GREEN-REFACTOR):
  - RED: Write a failing test that defines the expected behavior
  - GREEN: Write the minimum code to make the test pass
  - REFACTOR: Clean up the code without breaking the test
- Infrastructure, documentation, and pure configuration changes are exempt; validate those through the appropriate review and verification path instead
- If a bug is found, add or update a failing regression test before implementing the fix whenever practical
- deviations from sprint scope should be logged in the project's drift log

## Pre-Merge / Pre-Closeout Gate
Before finalizing sprint changes:
- run the project's declared verification baseline
- confirm acceptance criteria are met
- confirm required project-local artifacts are updated
- confirm unresolved drift is not being silently carried forward

## Validation + Governance Closeout
- Case validates the delivered sprint against the sprint's instantiated Acceptance / Test Plan
- Ledger performs a Sprint Governance Review and records:
  - process followed: yes/no
  - drift introduced: yes/no
  - drift documented: yes/no
  - required docs updated: yes/no
  - governance/process follow-ups: list or none
- significant execution, validation, or governance issues should be escalated to Kade for triage and recommendation
- if governance/process fixes are small and unambiguous, Ledger may update and commit the docs/process changes directly in the relevant project repo
