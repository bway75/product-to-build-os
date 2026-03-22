# Role Trigger Rules

These rules define when roles may proceed directly and when they must escalate to Kade instead.

## Default Trigger Path
- Brian normally triggers Kade, not Mason, Case, or Ledger directly.
- Kade normally triggers Mason once the execution package is ready.
- Mason may trigger Case directly when the validation-start rules are satisfied.
- Case may trigger Ledger directly when the governance-review rules are satisfied.
- Brian may still use Manual Mode for smaller tasks, experiments, process debugging, or sensitive / unclear work.

## Mason May Trigger Case Directly When
- the active Sprint Spec exists
- the Acceptance / Test Plan is instantiated
- implementation is complete enough for validation
- verification results are available
- there is no significant unresolved technical ambiguity blocking validation

## Case May Trigger Ledger Directly When
- validation is complete, or complete enough to state the result clearly
- the Sprint Spec is available
- the Acceptance / Test Plan was used for validation
- any drift or artifact issues are known and can be reported clearly
- the issue is now governance/process follow-up rather than technical ambiguity

## Roles Must Escalate To Kade Instead Of Proceeding When
- the package for the next role is materially incomplete
- the next action depends on unresolved technical ambiguity
- acceptance intent is unclear
- governance/process conflicts change who should act next
- cross-role disagreement is significant enough that ordinary handoff is unsafe

## Scope Boundary
- These rules are for predictable, low-ambiguity handoffs.
- When the situation is materially ambiguous or risky, escalate rather than forcing the next role to infer intent.
