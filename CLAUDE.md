# Product to Build OS — Operator File

## What This Repo Is

A reusable, documentation-driven operating model for product-to-engineering
delivery: role-based startup files (Brian → Kade → Mason → Case → Ledger),
governance rules, and templates that an *adopting project repo* instantiates.
This repo is methodology only — no app code, no project-specific state.
**Status: active-by-reference** — last direct commit 2026-04-22, but its role
model is currently borrowed live by the OT-security-research corpus
(Claude-as-Kade, Mason as manager window, Minions as numbered sub-agents).
Treat the roles below as in-use, not archived.

## How To Use It

Prompt-driven methodology, not a program — no build/test/run command exists
(confirmed: no `package.json`/scripts/code anywhere outside `.git`). It is
"run" by having an AI session adopt a role:

1. Open the role entrypoint file at repo root: `BRIAN.md`, `KADE.md`,
   `MASON.md`, `CASE.md`, or `LEDGER.md`.
2. Each says "You are `<Role>`... find all instructions in `<ROLE>.md`" and
   lists Identity, Scope, Responsibilities, Out of Scope, Escalation Rules,
   and Required References (always incl. `AGENT_MODEL.md`).
3. In an adopting project repo, the role also reads that project's
   instantiated PRD/Technical Implementation Plan/Acceptance Test Plan/
   Sprint Spec/current-state doc per its "also read..." line.

Verified by direct inspection, not execution: read `README.md`,
`AGENT_MODEL.md`, and all five role files this session — the sequence,
escalation paths, and scopes above are what those files actually say.

## Repo-Specific Rules

**1. Sprint-start artifact gate** — Trigger: Mason about to begin sprint
implementation. Behavior: confirm *instantiated* (not template-only)
Technical Implementation Plan, Acceptance/Test Plan, and Sprint Spec exist
first. Prevents: implementation on an unshaped/unscoped sprint. Check: all
three instantiated docs exist and are linked from the sprint.

**2. Escalation routes through Kade, not Brian** — Trigger: Mason/Case/
Ledger hits a significant risk or gap. Behavior: escalate to Kade for
triage; Kade routes to Brian only for product-authority/scope decisions.
Prevents: Brian absorbing downstream coordination the model assigns to
Kade. Check: escalation names Kade, not Brian, unless intent itself is
in question.

**3. Minions report to Mason only** — Trigger: Mason dispatches sub-agent
("Minion") work. Behavior: Minion output returns to Mason; Mason verifies
(proof over narrative) before it surfaces upward. Prevents: sub-agents
self-reporting to Brian/Kade, bypassing Mason's verification. Check: no
Minion output reaches Brian/Kade without a Mason-verified summary.

**4. No project-specific state in this repo** — Trigger: about to write
CURRENT_STATE/DECISIONS/DRIFT_NOTES/WORKLOG/a sprint spec. Behavior: put it
in the *adopting project's* repo, not here (README "What This Repo Is Not").
Prevents: this methodology repo accumulating one project's history and
becoming unreusable elsewhere (incl. the OT-corpus reuse case). Check: any
new non-template/non-role/non-process file here gets redirected.

**5. Role invocation requires reading the role file, not just naming it**
— Trigger: a session/sub-agent told to "act as Kade/Mason/Case/Ledger."
Behavior: actually read `<ROLE>.md` + `AGENT_MODEL.md` (+ project artifacts
if applicable) first — nothing enforces this automatically in a doc-only
repo. Prevents: role drift — claiming a role's authority without its
constraints loaded. Check: session can cite which role file it read.

## What NOT To Restate

Global operating rules (proof-of-done, bounded autonomy, irreversible-action
gate, etc.) live in one place:
`~/ai-workspace/GitHub/ai-knowledge-base/shared/skills/model-operating-rules.md`.
Don't duplicate them here — this file covers only what's specific to how
this repo's role model actually breaks.
