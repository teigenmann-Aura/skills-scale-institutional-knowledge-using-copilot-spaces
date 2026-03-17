# OctoAcme Project Management Docs

This folder is the home for OctoAcme's program and process documentation. It contains the core guides, templates, and references that cross-functional teams use to plan, execute, and ship work consistently across all product initiatives.

## Process Overview

OctoAcme's project management approach follows a lightweight but structured lifecycle: **Initiation → Planning → Execution/Tracking → Release/Deployment → Close/Retrospective**. New initiatives begin with a **Project Initiation** step focused on validating the business need and aligning stakeholders. The minimum deliverables are intentionally small—a **Project One-pager** (problem, goal, success metrics), a stakeholder/communications plan, a high-level timeline with milestones, and an initial risks/dependencies list—followed by a clear decision gate to proceed into planning once success metrics, priority, and team availability are confirmed.

In **Project Planning**, the team turns an approved initiative into an actionable plan by breaking work into shippable increments, creating a prioritized backlog with explicit acceptance criteria, and estimating scope (e.g., T-shirt sizing or story points). Planning also includes documenting a **Definition of Done**, identifying dependencies and integration points, and drafting an initial QA approach and test plan. Responsibilities are organized around clear personas: **Project Manager / PM** (coordination, delivery, risks, comms), **Product Manager / PdM** (outcomes, prioritization, success measurement), **Developers** (implementation, testing, estimation, technical risk mitigation), plus **QA/Testing** and broader **Stakeholders** for inputs and approvals.

Day-to-day **execution and tracking** is managed through a project board workflow (Backlog → Ready → In Progress → In Review → QA → Done) supported by a consistent team rhythm: daily standups to surface progress and blockers, a weekly delivery sync for status updates and risk flagging, and demos/reviews at sprint or milestone boundaries. Communication emphasizes transparency and a single source of truth for status, using templates like weekly status updates (progress, next steps, risks/blockers, and asks/decisions). Risks are tracked in a **risk register** (impact, likelihood, owner, mitigation, status) with defined escalation paths that move from team triage to PM/Product Lead escalation and—when needed—sponsor-level involvement.

Quality assurance is treated as part of the workflow rather than a separate phase: new logic should have unit tests, broader integration tests are used where appropriate, and critical flows get end-to-end smoke testing before release. The PR process favors small changes linked back to issues and acceptance criteria, with CI (tests, linting, security scanning) and required review approval prior to merge. Releases follow a standardized checklist—acceptance criteria complete, CI/security checks passing, release notes and rollback plan prepared, staging and smoke tests, production deploy, post-deploy verification, and stakeholder announcements—and each sprint or milestone concludes with a **retrospective** that turns learnings into owned, time-bound action items tracked back in the backlog.

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](./octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and the project lifecycle at a glance |
| [Project Initiation](./octoacme-project-initiation.md) | How to kick off a new initiative: one-pager, stakeholders, timeline, and decision gate |
| [Project Planning](./octoacme-project-planning.md) | Breaking work into increments, building the backlog, estimating scope, and defining done |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Board workflow, standups, delivery sync cadence, and status reporting |
| [Risks & Communication](./octoacme-risks-and-communication.md) | Risk register, escalation paths, and stakeholder communication strategy |
| [Release & Deployment](./octoacme-release-and-deployment.md) | Release checklist, deploy process, smoke tests, rollback, and incident response |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Blameless retros, action items, and how learnings feed back into the backlog |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Detailed responsibilities and communication patterns for each role |

---

> Update this README whenever new process documents are added or existing ones are significantly revised.
