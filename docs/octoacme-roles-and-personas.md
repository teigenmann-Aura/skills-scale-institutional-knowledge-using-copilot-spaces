# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
The Release Manager owns the end-to-end release process, coordinating deployment planning, ensuring all pre-release criteria are met, managing rollback readiness, and communicating release status to the team and stakeholders.

### Responsibilities
- Own and maintain the release calendar and deployment windows
- Ensure all pre-release requirements are met before approving a release (CI passing, acceptance criteria closed, rollback plan in place)
- Coordinate smoke tests and post-deploy verifications
- Manage rollback procedures and incident response during deployments
- Publish release notes and communicate deployment outcomes
- Maintain and improve the release checklist and runbooks

### Goals
- Ship releases predictably with minimal production incidents
- Reduce deployment risk through consistent process compliance
- Ensure fast, low-friction rollback when needed

### Typical Communication
- Release readiness reviews with PM and Developers before each deployment
- Deployment status announcements to stakeholders and support teams
- Post-release retros when incidents or near-misses occur
- Maintains the [Release Handoff Checklist](./octoacme-release-handoff-checklist.md)

### Interactions with Existing Roles
| Role | Interaction |
|---|---|
| Project Manager | Aligns on release dates, windows, and risk tolerance; escalates blocking issues |
| Product Manager | Confirms acceptance criteria are closed and release notes are accurate |
| Developers | Coordinates deployment steps, rollback scripts, and post-deploy verification tasks |
| QA Automation Specialist | Confirms automated test suites pass before release approval |

### Handoff / Collaboration Touchpoints
- **Planning**: Participates in sprint planning to flag release-impacting dependencies
- **Execution**: Reviews PR merges and CI status throughout the sprint
- **Release**: Leads the release readiness review; executes or coordinates the deployment
- **Retrospective**: Contributes deployment metrics and incident data to retros

---

## QA Automation Specialist

### Role Summary
The QA Automation Specialist designs, builds, and maintains automated test suites that validate product quality. They partner with Developers and the Release Manager to integrate testing into CI/CD pipelines and reduce reliance on manual testing effort.

### Responsibilities
- Design and implement automated test suites (unit, integration, end-to-end)
- Maintain and triage test failures in CI/CD pipelines
- Define coverage targets and track trends over time
- Collaborate with Developers to ensure new features are testable and covered
- Support performance, regression, and smoke test automation
- Document testing strategies and contribute to the Definition of Done

### Goals
- Maximize automated test coverage to catch defects early
- Reduce manual QA effort and release cycle time
- Provide fast, reliable feedback loops for the development team

### Typical Communication
- Sprint planning and backlog refinement to clarify testing scope
- PR review comments to flag missing test coverage
- CI/CD pipeline status reports and coverage dashboards
- Release readiness sign-off with the Release Manager

### Interactions with Existing Roles
| Role | Interaction |
|---|---|
| Project Manager | Reports test coverage trends and flags risks caused by insufficient test coverage |
| Product Manager | Clarifies acceptance criteria to ensure test scenarios are complete and correct |
| Developers | Pairs on test design, reviews PRs for testability, and co-owns the test suite |
| Release Manager | Provides automated test results as a pre-release gate |

### Handoff / Collaboration Touchpoints
- **Planning**: Adds test tasks to stories and ensures Definition of Done includes coverage targets
- **Execution**: Runs automated suites on every PR; flags regressions immediately
- **Release**: Certifies passing automated test results as part of the release gate
- **Retrospective**: Shares flaky test counts, coverage trends, and improvement proposals

---

## Stakeholder Engagement Lead

### Role Summary
The Stakeholder Engagement Lead is responsible for coordinating communication with external and internal stakeholders, managing feedback loops, and ensuring cross-business alignment throughout the project lifecycle.

### Responsibilities
- Identify and map key stakeholders for each project
- Facilitate regular stakeholder updates, demos, and feedback sessions
- Capture stakeholder input and translate it into actionable items for the PM and PdM
- Manage escalations and resolve cross-team communication blockers
- Maintain a stakeholder communication plan and contact registry
- Ensure visibility into project status for leadership and business units

### Goals
- Maintain strong stakeholder relationships and confidence in the team
- Surface business needs and feedback early to prevent late-stage rework
- Reduce escalations by proactively managing expectations

### Typical Communication
- Monthly (or milestone-based) stakeholder briefings
- Executive status summaries and decision-point notifications
- Feedback intake forms and interview notes shared with the PM and PdM
- Coordination with PM on communication plans and escalation paths

### Interactions with Existing Roles
| Role | Interaction |
|---|---|
| Project Manager | Co-owns the communication plan; aligns on escalation thresholds and messaging |
| Product Manager | Channels stakeholder feedback into the backlog; validates roadmap priorities with business sponsors |
| Developers | Arranges demos and Q&A sessions so stakeholders can see progress and provide input |
| Release Manager | Coordinates release communications and post-release stakeholder notifications |

### Handoff / Collaboration Touchpoints
- **Initiation**: Leads stakeholder identification and kickoff communication
- **Planning**: Facilitates alignment meetings to validate scope and priorities with sponsors
- **Execution**: Organizes mid-sprint demos and feedback reviews
- **Release**: Manages pre-release announcements and post-release stakeholder notifications
- **Retrospective**: Gathers stakeholder sentiment feedback and contributes to process improvement discussions

---

## Cross-Functional Integrator

### Role Summary
The Cross-Functional Integrator identifies and facilitates collaboration points across teams and systems, resolves integration blockers, and maintains shared documentation to ensure smooth delivery of work that spans multiple teams or platforms.

### Responsibilities
- Map inter-team dependencies and monitor their status
- Facilitate cross-team planning, alignment meetings, and escalation paths
- Maintain shared integration documentation, API contracts, and decision logs
- Identify integration risks early and coordinate mitigations
- Ensure shared environments and staging resources are available and aligned
- Act as the single point of contact for cross-team technical queries

### Goals
- Eliminate integration blockers before they impact the sprint
- Maintain a shared, up-to-date view of inter-team dependencies
- Reduce rework caused by misaligned assumptions across teams

### Typical Communication
- Cross-team syncs and dependency review meetings
- Integration risk updates in the project risk register
- Shared documentation and decision logs in the project wiki
- Escalations to PM when integration blockers cannot be resolved at team level

### Interactions with Existing Roles
| Role | Interaction |
|---|---|
| Project Manager | Reports integration risks and blockers; collaborates on dependency management and escalations |
| Product Manager | Flags scope assumptions that may conflict with other product areas or teams |
| Developers | Coordinates API contracts, shared service boundaries, and environment setup |
| Release Manager | Confirms cross-team readiness before deployment; coordinates joint release activities |

### Handoff / Collaboration Touchpoints
- **Initiation**: Identifies external dependencies and integration risks during project scoping
- **Planning**: Reviews cross-team work items and coordinates joint sprint commitments
- **Execution**: Monitors integration test environments; facilitates unblocking sessions across teams
- **Release**: Coordinates multi-team deployment sequencing and validates end-to-end integration
- **Retrospective**: Captures cross-team friction points and proposes structural improvements

---

## Role-to-Activity RACI

The table below maps key project activities to the primary roles. Use this to clarify ownership and reduce ambiguity.

**Legend**: R = Responsible | A = Accountable | C = Consulted | I = Informed

| Activity | Project Manager | Product Manager | Developer | Release Manager | QA Automation Specialist | Stakeholder Engagement Lead | Cross-Functional Integrator |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Define project scope & charter | A | C | C | I | I | C | C |
| Stakeholder identification & communication plan | A | C | I | I | I | R | C |
| Backlog prioritization | C | A | C | I | I | C | C |
| Sprint planning | A | C | R | C | C | I | C |
| Feature implementation | I | I | R/A | I | C | I | I |
| Automated test design & maintenance | I | C | C | C | R/A | I | I |
| Cross-team dependency management | C | I | C | C | I | I | R/A |
| Release readiness review | A | C | C | R | C | I | C |
| Deployment execution | I | I | C | R/A | I | I | C |
| Stakeholder demos & feedback sessions | C | C | R | I | I | A | C |
| Post-release stakeholder notification | I | C | I | C | I | R/A | I |
| Retrospective facilitation | R/A | C | C | C | C | C | C |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

