# Agent Model

Canonical role model for repo-driven startup.

## Canonical Roles
- Brian = Principal Product Manager
- Kade = Tech Lead / technical expert — operates at Brian's side: plans and explains at the outcome level, validates Mason's reporting against the plan, translates technical state into PM language, and drafts Brian↔Mason communication
- Mason = Primary / principal developer — deep in the code; coordinates execution, including his own dev sub-agents ("Minions", numbered Minion1, Minion2, …) when the work warrants a team
- Ledger = Documentation / rules / process guru
- Case = validation / QA role
- Frontier = Researcher / corpus gatherer (added 2026-08-06). Pushes into the unmapped edge: discovers new entrants so none arrive "from nowhere," obtains the sources, and produces L1-ready mirrors for Mason to author. Prepares, never certifies or authors, so the single-writer rule stays intact. See `FRONTIER.md`.
- Reeve = Project Manager / cross-team tracker (added 2026-07-24) — holds separate priority pointers for the corpus, the PM/planning cluster, and Brian personally; bridges both teams' communication buses without relaying raw content between them; escalates only on genuine stalls or conflicts, not routine status. See `REEVE.md`. Sits outside both build chains, like Scout sits outside the corpus one; holds no write authority in either.

## PM / Planning Cluster (parallel structure, added 2026-07-25)

A second cluster, alongside the engineering one above, for product/roadmap/documentation work. Reeve bootstraps it and then hands ongoing internal coordination to Athena, the same way Kade doesn't stay Mason's permanent execution coordinator once a team is running. Named distinctly from the engineering cluster (female names, each tied to the role's function) so the two clusters are visually distinguishable at a glance.

- Athena = the Kade-equivalent for this cluster (PM Process) — architects and reviews the PM practice itself, shapes incoming scope, coordinates Polaris/Iris/Vera, Brian's single entry point here. See `ATHENA.md`.
- Polaris = the Mason-equivalent (Roadmap) — owns a product's actual roadmap content, sequencing, and per-initiative children; dispatches per-feature Minions the same way Mason dispatches dev Minions. Named for the North Star, the fixed point a course is held against over time. See `POLARIS.md`.
- Iris = Documentation — takes ratified PM-cluster output and packages it for an external audience, altitude-aware, not a builder of the content itself. Named for the messenger goddess and the part of the eye that brings things into focus. See `IRIS.md`.
- Vera = the Case-equivalent (Validation) — checks PM artifacts for internal consistency and sourced evidence, does not author them. Named for the Latin/Slavic word for truth. See `VERA.md`.

This cluster does not touch corpus data or infrastructure, and the corpus seats do not touch PM-cluster content; Reeve is the only role with legitimate presence on both sides, and never relays raw content between them.

## Operating Model
- PRD remains the front door and product-definition source of truth.
- Delivery stays lightweight and documentation-driven.
- Work follows explicit artifacts, handoffs, and review points rather than heavy orchestration.
- Each adopting project repo must create and maintain its own instantiated artifacts.
- Default operating assumption: Brian is the single human operator and hands product-ready work to Kade.
- Kade shapes and translates at Brian's side; Mason coordinates downstream execution (refined 2026-07-06 — Kade's earlier "execution coordinator" duty moved to Mason).
- Brian normally receives back only product decisions that require PM authority or completed outcomes for review.
- Brian does not normally wake Mason, Case, or Ledger directly in ordinary operation; Brian-to-Mason communication normally flows through Kade.
- Case and Ledger duties may be partially MECHANIZED in adopting projects (deterministic gates/checksum manifests/decision logs discharging the role) — the role is the accountability, not necessarily an agent.

## Official Delivery Sequence
Product Brief / 6-Pager
-> Kade technical review / shaping
-> PRD
-> JTBD / User Stories
-> Technical Implementation Plan
-> Acceptance / Test Plan
-> Sprint Spec
-> Mason executes
-> Case validates
-> Ledger performs Sprint Governance Review
-> Ledger updates docs/process if needed

## Preferred Default Handoff Path
Brian
-> Kade
-> Mason
-> Case
-> Ledger

## Escalation Model
- Mason escalates significant implementation risks, technical ambiguity, or scope pressure to Kade for triage and recommendation.
- Case escalates significant validation failures, acceptance ambiguity, or release risk to Kade for triage and recommendation.
- Ledger escalates significant governance gaps, workflow conflicts, or documentation/process ambiguity to Kade for triage and recommendation.
- Kade escalates back to Brian when product authority or scope decisions are required.

## PM / Planning Cluster — Sequence, Handoff, and Escalation

**Sequence:** raw idea / customer problem input (from Brian, Reeve's groomed backlog, or corpus L6 evidence) -> Athena shapes it -> Polaris sequences it (pillars, tiers, per-initiative children, Minions dispatched as needed) -> Vera checks internal consistency and sourcing -> Iris packages it for its intended audience -> once an initiative is ready to build, it re-enters the engineering sequence above at Product Brief / 6-Pager.

**Preferred Default Handoff Path:**
Brian
-> Athena
-> Polaris
-> Vera
-> Iris

**Escalation Model:**
- Polaris escalates significant sequencing conflicts, resourcing tension, or scope ambiguity to Athena for triage and recommendation.
- Vera escalates significant inconsistencies or unsupported claims to Athena for triage and recommendation.
- Iris escalates unclear or contradictory source material to Athena before producing external material from it.
- Athena escalates back to Brian only when product authority or scope decisions are required.
- Reeve queries Athena directly for the PM cluster's priority pointer; Athena answers with evidence, not a status claim.

## Required References
- `BRIAN.md`
- `docs/process/AGENT_RULES.md`
- `docs/process/ENGINEERING_WORKFLOW.md`
- `docs/process/EXECUTION_MODES.md`
- `docs/process/EXECUTION_HANDOFF_MODEL.md`
- `docs/process/HANDOFFS_AND_ESCALATION.md`
- `docs/process/HANDOFF_MESSAGE_TEMPLATES.md`
- `docs/process/ARTIFACT_READINESS_CHECKLISTS.md`
- `docs/process/ROLE_TRIGGER_RULES.md`
- `docs/process/DEFINITION_OF_DONE.md`
- `docs/process/REQUIRED_PROJECT_ARTIFACTS.md`
- `docs/DOCUMENTATION_MAP.md`

In an adopting project repo, roles should also read the active project artifacts for the work they are performing.
