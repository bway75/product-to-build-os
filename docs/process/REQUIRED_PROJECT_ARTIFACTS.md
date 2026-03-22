# Required Project Artifacts

Each project repo that adopts this OS must create and maintain its own instantiated project artifact set.

## Required In Every Project Repo
- `docs/CURRENT_STATE.md`
- `docs/DECISIONS.md`
- `docs/DRIFT_NOTES.md`
- `docs/WORKLOG.md`
- `docs/sprints/`
- Technical Implementation Plan
- Acceptance / Test Plan
- Sprint Governance Review record
- `docs/DOCUMENTATION_MAP.md`

## Recommended Naming Map
| Artifact category | Recommended filename or path |
|---|---|
| current state | `docs/CURRENT_STATE.md` |
| decisions log | `docs/DECISIONS.md` |
| drift log | `docs/DRIFT_NOTES.md` |
| worklog | `docs/WORKLOG.md` |
| documentation map | `docs/DOCUMENTATION_MAP.md` |
| sprint specs | `docs/sprints/` |
| Technical Implementation Plans | `docs/plans/TECHNICAL_IMPLEMENTATION_PLAN_<scope>.md` |
| Acceptance / Test Plans | `docs/plans/ACCEPTANCE_TEST_PLAN_<scope>.md` |
| Sprint Governance Reviews | `docs/governance/SPRINT_GOVERNANCE_REVIEW_<scope>.md` |

## Required Before Sprint Implementation Starts
- instantiated Technical Implementation Plan
- instantiated Acceptance / Test Plan
- instantiated Sprint Spec

Template files alone do not satisfy this requirement.

## Required When Relevant
- architecture docs
- deployment docs
- API or integration docs
- runbooks
- environment or operational guidance

## Maintenance Rule
- These artifacts must be maintained in the project repo where the work is actually executed.
- This methodology repo provides templates and rules, not instantiated project history.
