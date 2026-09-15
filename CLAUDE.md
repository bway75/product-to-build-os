# Product to Build OS — Operator File

## ⚠️ SEAT BOOT, READ FIRST (fires the moment you are named as a role)

If this session's opening instruction identifies you as a role in this repo's model ("I am Kade",
"You are Mason", "You are Polaris", "You are Athena", or similar, for ANY role in `AGENT_MODEL.md`'s
current roster — that file governs which roles exist, not the stale list two paragraphs below), that
identification IS your first task. Run the boot sequence below as your FIRST action, before
answering anything, picking up any work, or offering a menu of options. A named role that starts
answering without booting is not up.

**Precondition, working directory — advisory, not a hard stop here.** This repo is methodology
only; the natural home for a role's live work is the *adopting project repo* (e.g. this model is
borrowed live by `ot-security-research` for the engineering cluster). If your working directory is
neither this repo nor a clear adopting project, note that explicitly in your boot report and read
this repo's files by full path rather than silently assuming relative paths resolve. **Operating a
role cross-repo by full path from another session is an accepted pattern** (Brian confirmed this for
Athena from an `ot-security-research` session, 2026-08-31) — flag the mismatch once, then proceed if
the user confirms, don't refuse or loop on it.

**Boot steps (all roles):**
1. Read `AGENT_MODEL.md` (canonical roster, authority boundaries, activation state) and your own
   `<ROLE>.md` charter in full.
2. Read every file your charter's **Required References** section names — this is where each role's
   actual reading list lives; do not substitute a shorter guess. For a PM-cluster role that also
   means the relevant `pm-process/` methodology files (sibling repo,
   `~/ai-workspace/GitHub/pm-process/`) your charter cites.
3. Check current state: `docs/CURRENT_STATE.md` for the engineering cluster, or — per your charter's
   "In an adopting product context, also read..." line — the adopting product's current Initiative
   Brief / roadmap draft / capability breakdown for the PM cluster. If it's an unfilled template,
   say so; don't infer state that isn't there.
4. Check for already-running peer sessions (`ListAgents`) and, if your cluster has a message bus
   set up yet, its current status/inbox — so you don't duplicate or contradict work already in
   flight. Absence of a bus is a valid finding, not a blocker to report on.
5. **Report**, in one paragraph: which role, what you read, what live state you found (including
   "nothing is in flight yet" if true, and any repo/cwd mismatch from the precondition above), and
   hand back for direction rather than guessing next steps.

This supersedes Repo-Specific Rule 5 below on *how* invocation works; Rule 5's principle (read the
file, don't just claim the role) stands, this section is its enforcement mechanism.

## What This Repo Is

A reusable, documentation-driven operating model for product-to-engineering
delivery: role-based startup files, governance rules, and templates that an
*adopting project repo* instantiates. **The current roster is `AGENT_MODEL.md`
— do not treat the "Brian → Kade → Mason → Case → Ledger" shorthand elsewhere
in this file as complete;** it predates Frontier, Reeve, Bob, Dean, Scout,
Warden, and the whole PM/Planning cluster (Athena, Polaris, Iris, Vera).
This repo is methodology only — no app code, no project-specific state.
**Status: active-by-reference** — last direct commit 2026-04-22, but its role
model is currently borrowed live by the OT-security-research corpus
(Claude-as-Kade, Mason as manager window, Minions as numbered sub-agents).
Treat the roles below as in-use, not archived.

## How To Use It

Prompt-driven methodology, not a program — no build/test/run command exists
(confirmed: no `package.json`/scripts/code anywhere outside `.git`). It is
"run" by having an AI session adopt a role:

1. Open the role entrypoint file at repo root — one `<ROLE>.md` per name in
   `AGENT_MODEL.md`'s current roster (currently: `BRIAN.md`, `KADE.md`,
   `MASON.md`, `CASE.md`, `LEDGER.md`, `SCOUT.md`, `FRONTIER.md`, `REEVE.md`,
   `ATHENA.md`, `POLARIS.md`, `IRIS.md`, `VERA.md`, plus `BOB.md`/`DEAN.md`
   registered-not-active and `WARDEN.md` a hat, not a bootable seat — see
   `AGENT_MODEL.md` for which of these currently hold authority). Do not
   treat this as a fixed five-file list; a role missing from here that
   exists in `AGENT_MODEL.md` is this line falling behind, not evidence the
   role has no entrypoint.
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
— Trigger: a session/sub-agent told to "act as" ANY role in `AGENT_MODEL.md`
(not only the original five). Behavior: run the SEAT BOOT sequence at the
top of this file — nothing enforces this automatically in a doc-only repo
otherwise. Prevents: role drift — claiming a role's authority without its
constraints loaded. Check: session can cite which role file and which
Required References it actually read.

## What NOT To Restate

Global operating rules (proof-of-done, bounded autonomy, irreversible-action
gate, etc.) live in one place:
`~/ai-workspace/GitHub/ai-knowledge-base/shared/skills/model-operating-rules.md`.
Don't duplicate them here — this file covers only what's specific to how
this repo's role model actually breaks.
