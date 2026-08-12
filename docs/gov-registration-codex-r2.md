No files were edited.

## MUST-FIX

- `AGENT_MODEL.md:5,51` — The new precedence rule is self-ratifying. It makes this file final on roster and authority boundaries, while the withdrawal record says, “**Kade owns this file**.” Nothing requires a Brian-authorized, durable decision reference before a roster or authority change is recorded. An adversarial Kade can therefore write authority into the canonical source and have it override every charter. Require Brian authorization plus a named decision-record reference for every roster/boundary/activation change; Kade may record it, not ratify it.

- `AGENT_MODEL.md:15,17`; `BOB.md:5-9` — Registration and activation remain non-reproducible. `BOB.md` is untracked, yet the activation test requires reviewing that charter and clearing its banner. A fresh clone cannot evaluate the condition. The problem is broader under the new canonical-roster claim: `ATHENA.md` is also untracked, and the referenced `POLARIS.md`, `IRIS.md`, and `VERA.md` are not tracked. The precedence paragraph does not cure missing source artifacts. Track the charters or remove/defer the affected registrations until their canonical artifacts are versioned.

- `AGENT_MODEL.md:19` — Routing Bob’s end condition to Brian is not a fix while activation remains possible without it. The text expressly says “temporary” is “intent, not a constraint”; it supplies neither a deadline nor a condition that prevents activation. Bob need not be removed from the registered roster, but activation must require Brian’s dated retirement/review trigger, or registration must wait.

## SHOULD-FIX

- `BOB.md:5-9,104-108` — The operative banner and withdrawn lead mechanism still appear in Bob’s charter: “**STATUS: OPERATIVE**,” “the lead is the seat that owns the domain,” and “unrecorded designation does not exist.” `AGENT_MODEL.md:5,15,47` formally defeats those claims, so this is not a remaining legal path to authority; it is still a hazardous contradictory instruction for a reader. Replace it before activation.

- `AGENT_MODEL.md:23` — The acceptance split is substantively correct and compatible with `CASE.md:10-16` and `LEDGER.md:18-27`; it preserves Kade’s infrastructure ownership. But “requires an INDEPENDENT review before production use” names neither the reviewer nor what independence means. For a non-Acceptance/Test-Plan infrastructure change, this is unenforceable. Name the review holder and required evidence.

- `AGENT_MODEL.md:92-93`; `CASE.md:24-25` — Bob and Dean route acceptance-criteria ambiguity to Case, but Case must route unclear criteria to Kade. That is not a loop, but the canonical route should say “Case, then Kade for criteria ambiguity” so Case is not mistaken for the criteria owner.

- `AGENT_MODEL.md:5,21,37,94`; `ATHENA.md:41` — Precedence resolves this in Kade’s favor, but Athena’s charter still says a separate PM-bus deployment “doesn’t require [Kade’s] sign-off.” The current model says all infrastructure, including a PM-cluster bus, routes to Kade and is not Athena’s machinery. Align the charter to avoid an implementation instruction that conflicts with the canonical boundary.

## Disposition check

1. Lead withdrawal: complete in `AGENT_MODEL.md`; no seat can formally claim lead under line 47. The stale Bob language above should be removed.
2. Dangling bus record: resolved. `AGENT_MODEL.md:53` is historical explanation, not an operative requirement.
3. Pick-your-state: structurally resolved by `AGENT_MODEL.md:15`; Bob’s banner cannot prevail. It remains operationally unsafe because the charter is untracked and stale.
4. Gates versus acceptance: resolved in principle; Kade implements/operates, Case accepts, Ledger observes. The independent-review mechanics remain unspecified.
5. Temporary status: unresolved; it must become an activation constraint.
6. Dean/Kade and Dean/Reeve: resolved. For a capture-gate feasibility issue, Kade supplies the technical assessment and Dean cites/relays it; once Mason accepts Brian’s decision, Reeve tracks it.
7. Escalation: infrastructure coverage is now complete; the acceptance-criteria handoff needs the clarification above.
8. Reproducibility: not resolved, and now broader than Bob.

## NIT

- None.

**VERDICT: NOT CLEAN — 3 MUST-FIX findings.**