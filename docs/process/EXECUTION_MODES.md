# Execution Modes

This document defines the supported execution styles for teams using this OS.

The core process stays the same in every mode.
Only the execution and transport style changes.

## Supported Modes

### Mode 1 - Fully Manual
- Brian manually initiates each role transition.
- Best for early projects, sensitive work, or teams with low automation comfort.

### Mode 2 - Guided Handoffs
- Roles use the documented handoff packages and message templates.
- Brian still initiates most transitions.
- Good when the team wants more structure without much autonomy.

### Mode 3 - Authorized Role-Triggered Flow
- Mason may trigger Case directly when the documented readiness rules are satisfied.
- Case may trigger Ledger directly when the documented readiness rules are satisfied.
- Mason, Case, and Ledger may trigger Kade on defined escalation conditions.
- This is likely the default high-leverage mode for many teams.

### Mode 4 - Bounded Delegated Execution
- Roles may delegate bounded subtasks or use sub-agents within approved scope.
- Handoffs may be assisted or automated.
- Authority boundaries, artifact requirements, validation, governance review, and escalation rules still apply.

## Invariants Across All Modes
- required artifacts exist
- instantiated artifact rules remain in force
- readiness gates apply
- validation is not bypassed
- governance review is not bypassed
- escalation rules remain in force
- product authority stays with Brian
- technical arbitration stays with Kade unless explicitly delegated

## What May Vary By Mode
- who manually triggers the next role
- whether handoff templates are used manually or generated automatically
- whether readiness checks are done manually or validator-assisted
- whether bounded sub-agent delegation is allowed inside a role's approved scope

## Allowed Automation
- role-triggered handoffs when the documented readiness rules are satisfied
- bounded sub-agent delegation within approved scope
- wake / sleep review patterns
- automated readiness checks later
- validators for required files or completion states later

## Disallowed Automation
- scope changes without Brian
- bypassing Kade on required technical arbitration
- bypassing Case validation
- bypassing Ledger governance review
- cross-role authority violations
- open-ended agent autonomy outside approved boundaries

## Practical Guidance
- Start with the lowest mode that the team can run reliably.
- Move up only after the lower mode is working predictably.
- A higher automation mode is optional; it is not a maturity requirement by itself.

## Relationship To Future Tooling
- This OS can support validator-assisted or automated handoff patterns later.
- It should define compatible operating modes, not become the orchestration engine itself.
