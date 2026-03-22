# Execution Handoff Model

This document defines the current practical handoff model between roles.

The goal is to make execution flow explicit without introducing orchestration-platform assumptions.

## Preferred Default Path
- Brian -> Kade -> Mason -> Case -> Ledger
- Brian normally hands product-ready work to Kade, and Kade coordinates downstream execution.
- Brian does not normally wake Mason, Case, or Ledger directly except in Manual Mode or when Brian explicitly chooses an exception path.

## 1. Execution Package

This is the minimum package Mason must receive before implementation starts.

### Required Artifacts
- Product Brief / 6-Pager
- PRD
- JTBD / User Stories
- Technical Implementation Plan
- Acceptance / Test Plan
- Sprint Spec

### Required Context
- explicit constraints / exclusions
- open risks / escalation notes

### Trigger
- Kade hands work to Mason when the product and planning package is ready for sprint execution.
- Brian's normal handoff is to Kade, not directly to Mason.

### Rule
- Mason must not begin implementation until this execution package exists in instantiated working form.

## 2. Validation Package

This is the minimum package Case must receive when Mason finishes implementation work for validation.

### Required Artifacts
- Sprint Spec
- Acceptance / Test Plan

### Required Context
- implementation summary
- verification results
- drift / deviation notes
- known limitations

### Trigger
- Mason hands work to Case when the sprint is ready for validation.

## 3. Governance Review Package

This is the minimum package Ledger must receive after validation.

### Required Artifacts
- Sprint Spec

### Required Context
- implementation summary
- verification results
- Case validation summary
- drift notes
- docs/process follow-up context

### Trigger
- Case hands work to Ledger when validation is complete, or when governance/process issues are the next blocking concern.

## 4. Trigger Rules

### Brian -> Kade
- Trigger when product definition is ready for technical shaping and execution planning.

### Kade -> Mason
- Trigger when the execution package is ready and the sprint can start.

### Mason -> Case
- Trigger when implementation is complete enough for validation.

### Case -> Ledger
- Trigger when validation is complete or a governance/process issue is exposed.

### Mason / Case / Ledger -> Kade
- Trigger when significant issues require technical triage, sequencing guidance, or cross-role resolution.

## 5. Minimum Handoff Format

Use this short repeatable structure for manual handoffs:

- package ready: yes/no
- artifacts included:
- open risks:
- expected next action:
- escalation needed: yes/no

## Escalation To Kade

Escalate to Kade when:
- technical ambiguity is blocking execution
- acceptance ambiguity is blocking validation
- governance/process conflicts cannot be resolved within role boundaries
- the package is incomplete in a way that materially affects the next role

Kade provides triage, recommendation, and downstream coordination, and routes back to Brian when product definition is the real blocker.
