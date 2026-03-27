# Project Bootstrap Checklist

Use this checklist when instantiating the OS in a new project repo.

## Step 1: Copy Role Files

Copy and adapt each role file from the OS repo root into the new project repo root:
- `BRIAN.md` — adapt to the specific project context
- `MASON.md` — adapt to the specific technology stack
- `KADE.md` — adapt to the specific technical domain
- `LEDGER.md` — adopt as-is or adapt governance scope
- `CASE.md` — adopt as-is or adapt validation scope
- `AGENT_MODEL.md` — adopt as-is

## Step 2: Copy Process Docs

Copy the following from `docs/process/` into the new project's `docs/process/` (or `docs/` per project convention):
- `AGENT_RULES.md`
- `ENGINEERING_WORKFLOW.md`
- `DEFINITION_OF_DONE.md`
- `EXECUTION_MODES.md`
- `HANDOFFS_AND_ESCALATION.md`
- `ROLE_TRIGGER_RULES.md`
- `SPRINT_GOVERNANCE_REVIEW.md`

## Step 3: Instantiate Runtime Artifacts

Create these files in the new project repo by copying from `docs/templates/` and populating with project-specific content. Do not leave them as empty templates — they must contain real project content before sprint work begins.

| File to create | Source template | Notes |
|---|---|---|
| `docs/CURRENT_STATE.md` | `docs/templates/CURRENT_STATE_TEMPLATE.md` | Describe the real starting state of the project |
| `AI_WORKLOG.md` | `docs/templates/WORKLOG_TEMPLATE.md` | Start with a bootstrap entry |
| `docs/DECISIONS.md` | `docs/templates/DECISIONS_LOG_TEMPLATE.md` | Log any early architectural decisions |
| `docs/DRIFT_NOTES.md` | `docs/templates/DRIFT_LOG_TEMPLATE.md` | Start empty; append when drift occurs |
| `docs/DOCUMENTATION_MAP.md` | `docs/templates/DOCUMENTATION_MAP_TEMPLATE.md` | Map all active docs for the project |

## Step 4: Instantiate Sprint Artifacts

Before any sprint begins, create instantiated (not template) versions of:
- Sprint Spec (`docs/sprints/SPRINT_001_<name>.md`) — from `docs/templates/SPRINT_SPEC_TEMPLATE.md`
- Technical Implementation Plan — from `docs/templates/TECHNICAL_IMPLEMENTATION_PLAN_TEMPLATE.md`
- Acceptance / Test Plan — from `docs/templates/ACCEPTANCE_TEST_PLAN_TEMPLATE.md`

Template files alone do not satisfy the sprint start gate. Each artifact must be populated with real sprint content.

## Ready-To-Execute Check

The project is ready for sprint implementation only when:
- All role entry files are in place and adapted
- All runtime artifacts exist with real content (not blank templates)
- The active sprint has an instantiated Technical Implementation Plan
- The active sprint has an instantiated Acceptance / Test Plan
- The active sprint has an instantiated Sprint Spec
- Contributors know where the active project artifacts live
