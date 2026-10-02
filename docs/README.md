# OctoAcme Project Management Docs

OctoAcme projects follow five stages: **Initiation, Planning, Execution, Release, and Close & Retrospective**. Initiation produces a Project One-pager, stakeholder list, high-level timeline, and initial risk list, followed by a go/no-go gate. Planning produces a prioritized backlog with acceptance criteria, a Definition of Done (DoD), a release plan, and a risk register. Execution tracks work on a board: Backlog, Ready, In Progress, In Review, QA, Done. Small PRs (<=400 lines when possible) link to issues and acceptance criteria, pass tests and linting in CI, and require at least one approval before merging.

The guiding principles are **customer-first, iterative delivery, clear ownership, data-informed decisions, and psychological safety**. Each project has a named Project Manager (PM) and Product Lead. The PM coordinates delivery, schedules, risks, and communication; the Product Manager (PdM) defines outcomes, prioritizes the backlog, and measures success. Developers design, build, test, and review software; QA/Testing validates quality and acceptance criteria; Stakeholders provide input and approvals.

Communication includes daily standups, a weekly delivery sync, a weekly PM+PdM sync, monthly stakeholder updates, and demos at each sprint or milestone. A single source of truth, such as the project README or release doc, carries status; the weekly status template covers progress, next steps, risks and blockers, and decisions needed. The risk register records impact, likelihood, ownership, mitigation, and status and is reviewed weekly. Blockers escalate through three levels: team triage, PM escalation to the Product Lead and dependent teams, then Sponsor escalation for business-impacting issues. Security incidents follow the security incident runbook and notify Security on-call.

Quality assurance combines unit tests, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA when needed. Before release, acceptance criteria must be met, PRs merged, CI and security scans passing, release notes drafted, a rollback plan documented, and smoke tests prepared. Deployment goes to staging with smoke tests, then production (preferably through an automated pipeline), followed by post-deploy verification and stakeholder notification. Failed deployments trigger incident response and rollback to the last known-good release if needed. Retrospectives after sprints, releases, milestones, or incidents last 45–75 minutes and produce 2–3 prioritized action items with owners and due dates, tracked in the backlog and reviewed at the weekly PM sync.

## Docs

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risks & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](octoacme-roles-and-personas.md)
