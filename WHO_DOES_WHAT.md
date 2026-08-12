# Who Does What

A one page introduction to the team: who leads which kind of work, and who to reach out to for a
given thing. Written for a person or a seat who needs the answer in ten seconds.

`AGENT_MODEL.md` is canonical. This page is the readable front door to it, not a second source of
truth. Where the two differ, `AGENT_MODEL.md` wins and this page is the defect.

Status: first pass, expected to need iteration (Brian, 2026-08-10). If a real piece of work does not
fit a row below, that is a gap to report, not a licence to improvise a lead.

---

## The rule in one line

**The lead follows the kind of work, not a rank.** If the task is building the corpus, Mason leads
and may ask for help. If the task is gathering sources into a mirror, Frontier leads. And so on.
Everyone helps whoever is leading. Helping does not make you the lead, and leading does not make you
the owner of someone else's domain.

When it is genuinely unclear what kind of work something is, **Brian names the lead.** Seats do not
settle that between themselves.

---

## Corpus cluster

| If the work is... | Lead | Reach out to them for |
|---|---|---|
| Writing, certifying, or locking corpus content at any layer (L1 to L6) | **Mason** | anything that changes what a corpus document says; track locks; authoring standards |
| Finding, capturing, staging, or recovering sources into the mirror | **Frontier** | a source we cannot get; a dead URL; which capture method to use; staging into `library/` |
| Building or running a tool, gate, harness, driver, service, or process | **Kade** | a broken tool; a gate that is wrong; anything about how the machinery works; **implementing** a process change |
| Program planning, sequencing, review and rebuild economics | **Bob** *(NOT YET ACTIVE)* | what the plan is; what a phase costs; whether a claim about the corpus is actually true |
| Carrying a decided Brian intent to the seats who act on it | **Dean** *(NOT YET ACTIVE)* | confirming what Brian actually decided, with the source |

> **Bob and Dean are REGISTERED but NOT YET ACTIVE** and hold no authority until activated. See the
> activation note in `AGENT_MODEL.md`. Their rows are listed so the roster is complete, not because
> work should be routed to them today. Until they activate, program planning questions go to Brian
> and Kade, and there is no relay lane: Brian's decisions come from Brian.
| Tracking and chasing work that was already accepted | **Reeve** | where something stands; what is stalled |
| A bounded experiment on copies, outside production | **Scout** | testing whether an approach works before anyone builds it |
| A read-only audit of whether we follow our own rules | **Brian**, who instantiates a Warden audit | there is no standing Warden to contact; ask Brian for an audit |

## PM and planning cluster

| If the work is... | Lead | Reach out to them for |
|---|---|---|
| How the PM practice itself works; shaping incoming scope | **Athena** | entry point for anything PM side |
| A product's roadmap content and its sequencing | **Polaris** | what is on the roadmap and in what order |
| Packaging ratified output for an outside audience | **Iris** | anything that leaves the building |
| Checking PM artifacts for consistency and sourcing | **Vera** | whether a PM claim is backed |

## Brian

Product authority. Scope, direction, money, credentials, and anything that costs something. A seat
that sends Brian an implementation question has made a mistake; Kade reframes it or sends it back.

---

## Three boundaries that cause most of the confusion

**1. Infrastructure is Kade's wherever it surfaces.** A tool, gate, harness, service, or bus failure
is infrastructure even when it breaks inside the PM cluster. It goes to Kade, not to that cluster's
process lead. Athena owns PM practice, not the machinery either cluster runs on.

**"Process" is three different things, so route by which one you mean.** Kade owns process
IMPLEMENTATION, the machinery that enforces a process. **Ledger** owns process and governance
DOCUMENTATION, the written rules and the catalog. **Athena** owns PM PRACTICE, how the planning
cluster works. "Process changes" is not automatically Kade's: only building or running the thing that
enforces it is.

**2. Specifying an instrument does not make it yours.** Bob writes the spec for a measurement
instrument or a gate; Kade builds, wires, owns, and reviews it. A measurement instrument is
infrastructure, not analysis.

**3. Nobody accepts their own work.** A gate's owner never treats its own gate as acceptance of that
gate, or of the work the gate was built to judge. A green gate is evidence. Acceptance is the
independent review, on record. This applies to Kade first, since Kade builds the gates.

---

## Two things that are not roles

- **Single writer on corpus content.** Only Mason and his dispatched team author or edit production
  corpus documents. Not Kade, not Bob, not Frontier, not a helper. Frontier prepares; Mason certifies.
- **Kade records the roster, Kade does not ratify it.** Changes to who exists, what authority a seat
  holds, or whether a seat is active need Brian's authorization and a named decision-record reference
  carried inline with the change. Kade writes it down; Kade does not grant it.

---

Full definitions: `AGENT_MODEL.md` for the roster and the boundaries, and each seat's own file
(`KADE.md`, `MASON.md`, `FRONTIER.md`, `BOB.md`, `DEAN.md`, `REEVE.md`, `ATHENA.md`, `POLARIS.md`,
`IRIS.md`, `VERA.md`, `CASE.md`, `LEDGER.md`) for how that seat works internally.
