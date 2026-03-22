# Execution Modes

This document defines the supported execution styles for teams using this OS.

The core process stays the same in every mode.
Only the execution and transport style changes.

## Default Operating Assumption
- The default operating model is single-operator PM-first.
- Brian is the human product operator and product authority.
- Brian normally hands work to Kade after product definition is ready.
- Kade is the default downstream technical lead and execution coordinator.
- Kade returns to Brian only when a product decision is needed or when the solution/outcome is ready for review.
- Brian does not normally wake Mason, Case, or Ledger directly except in Manual Mode or when Brian explicitly chooses an exception path.

## Supported Modes

### Mode 1 - Fully Manual
- Brian manually initiates role transitions.
- Use this as an optional fallback or debug mode for smaller tasks, experiments, process debugging, or sensitive / unclear work.

### Mode 2 - Guided Handoffs
- Roles use the documented handoff packages and message templates.
- Brian still initiates or approves most transitions through Kade.
- Good when the team wants more structure without much autonomy.

### Mode 3 - Authorized Role-Triggered Flow
- Brian hands product-ready work to Kade.
- Kade triggers Mason when the execution package is ready.
- Mason may trigger Case directly when the documented readiness rules are satisfied.
- Case may trigger Ledger directly when the documented readiness rules are satisfied.
- Mason, Case, and Ledger may trigger Kade on defined escalation conditions.
- This is the preferred default for many teams.

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
- how much downstream coordination Kade performs directly versus through tool-assisted handoffs

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
- Treat Mode 3 as the normal default unless there is a reason to stay lower.
- Use Mode 1 when the team wants tighter human control or is debugging the process itself.
- Move up only after the lower mode is working predictably.
- A higher automation mode is optional; it is not a maturity requirement by itself.

## Relationship To Future Tooling
- This OS can support validator-assisted or automated handoff patterns later.
- It should define compatible operating modes, not become the orchestration engine itself.
