# Example Project Instantiation

This is a generic example of how a new project might instantiate the OS.

## Example Project
Project name: `customer-insights-platform`

## Example Project-Local Artifact Layout
```text
/product
  PRD.md
  DELIVERY_PLAN.md
/docs
  CURRENT_STATE.md
  DECISIONS.md
  DRIFT_NOTES.md
  DOCUMENTATION_MAP.md
  WORKLOG.md
  /sprints
    SPRINT_001.md
  /plans
    TECHNICAL_IMPLEMENTATION_PLAN_SPRINT_001.md
    ACCEPTANCE_TEST_PLAN_SPRINT_001.md
  /governance
    SPRINT_GOVERNANCE_REVIEW_SPRINT_001.md
```

## Example Flow
1. Brian finalizes the PRD.
2. Kade shapes the work and reviews the implementation direction.
3. The project instantiates:
   - Sprint Spec
   - Technical Implementation Plan
   - Acceptance / Test Plan
4. Mason executes against those instantiated sprint artifacts.
5. Case validates against the instantiated Acceptance / Test Plan.
6. Ledger performs Sprint Governance Review and updates docs/process artifacts if needed.

## Example Rule In Practice
If the project only copied template files into `/docs/templates` but did not create a sprint-specific Technical Implementation Plan, Acceptance / Test Plan, and Sprint Spec, Mason must not start implementation yet.
