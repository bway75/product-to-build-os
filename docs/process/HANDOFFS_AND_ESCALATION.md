# Handoffs And Escalation

This document makes the role-triggered handoffs and Kade escalation boundary explicit.

## Preferred Default Path
- Brian -> Kade -> Mason -> Case -> Ledger
- Brian normally hands off to Kade and does not manually coordinate the downstream roles in ordinary operation.
- Manual Mode remains available when tighter human control or process debugging is needed.

## Official Role-Triggered Handoffs

### Brian -> Kade
Trigger:
- product direction is ready for technical shaping and execution planning

Handoff includes:
- Product Brief / 6-Pager
- PRD
- JTBD / User Stories when available
- explicit product constraints, exclusions, and open decisions

### Mason -> Case
Trigger:
- implementation for the sprint is complete enough for validation

Handoff includes:
- active Sprint Spec
- active Technical Implementation Plan
- active Acceptance / Test Plan
- verification status
- known risks or limitations

### Case -> Ledger
Trigger:
- validation is complete or blocked by a governance/process issue

Handoff includes:
- validation outcome
- acceptance gaps or pass/fail notes
- whether drift was observed
- whether artifact or workflow problems were discovered

### Mason / Case / Ledger -> Kade
Trigger:
- significant technical ambiguity
- material scope conflict
- acceptance ambiguity
- repeated cross-role disagreement
- governance/process conflict that cannot be resolved within role boundaries

Kade provides:
- triage
- recommendation
- sequencing guidance
- escalation back to Brian when product definition is the real blocker

## Within-Role Resolution

### Mason can resolve within role
- normal implementation decisions inside approved sprint scope
- local refactors inside approved scope
- ordinary test/verification issues tied to implementation work

### Kade can resolve within role
- ordinary downstream coordination after Brian hands off the work
- routine sequencing decisions between Mason, Case, and Ledger
- normal technical clarification that does not change product intent

### Case can resolve within role
- routine validation execution
- ordinary pass/fail reporting against the Acceptance / Test Plan
- minor clarification requests that do not change scope

### Ledger can resolve within role
- small, unambiguous docs/process cleanups
- documentation consistency fixes
- Sprint Governance Review recording and follow-up notes

## Must Escalate To Kade

### Mason must escalate
- unclear technical direction
- architectural risk
- material scope pressure
- conflicts between implementation guidance and accepted scope

### Case must escalate
- unclear acceptance criteria
- significant release risk
- lack of instantiated Acceptance / Test Plan
- repeated mismatch between delivered behavior and accepted scope

### Ledger must escalate
- conflicting governance/process signals
- unclear workflow ownership
- documentation/process issues that materially alter team workflow

## Bottleneck Prevention Rule
- Kade should be used for triage and recommendation, not for routine execution decisions that can be resolved within role.
- Brian should not normally mediate implementation questions, perform governance triage, or translate between downstream roles.
- Mason, Case, and Ledger should resolve ordinary in-role work directly and escalate only when the issue is significant, cross-role, or materially risky.
