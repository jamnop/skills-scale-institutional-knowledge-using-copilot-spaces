```markdown
# OctoAcme Project Management Docs

This folder centralizes OctoAcme's project management processes, artifacts, and templates. It's intended as the primary entry point for new team members, cross-functional collaborators, and stakeholders who need a concise orientation and direct links to process documents.

## Project Management Processes — At a Glance

OctoAcme follows an iterative lifecycle that moves from lightweight initiation through planning, execution, release, and continuous improvement. Projects start with a Project One-pager to capture problem statements, success metrics, primary stakeholders, and a basic timeline. Planning converts approved initiatives into prioritized backlogs with acceptance criteria, estimates, a Definition of Done (DoD), and a release/milestone plan so the team can pull shippable increments into timeboxed sprints or iterations.

Execution emphasizes predictable flow and quality: teams use a project board (Backlog → Ready → In Progress → In Review → QA → Done), create small pull requests with clear acceptance criteria, run CI (tests, linting, security scans), and require code review and QA before merges. Releases are governed by pre-release checks (passing CI, release notes, rollback plans, and smoke tests) and by a documented deployment checklist and incident/rollback playbook for safety. After each sprint, milestone, or incident, teams run retrospectives to capture action items, track them in the backlog, and measure the impact of changes.

Roles and communications are explicit to reduce ambiguity. Core personas include Product Managers (define outcomes and prioritize), Project Managers (coordinate delivery, risks, and stakeholder communications), Developers (implement, test, and document), QA (validate acceptance), and Sponsors/Stakeholders (provide approvals and inputs). Cadence includes daily standups for blockers and progress, weekly PM+PdM syncs, sprint demos/reviews, and monthly stakeholder updates. A simple escalation path (team → PM → Product Lead → Sponsor) is used for blockers, with a separate security incident path when required.

Quality assurance is a mix of automated and manual practices: unit and integration tests, end-to-end smoke tests for critical flows, security scanning in CI, small PRs with acceptance criteria, and manual QA for feature acceptance when necessary. Key artifacts (Project One-pager, Release Plan, Risk Register, Definition of Done, and Retrospective action items) are maintained in this repo to act as a single source of truth.

## Process Documentation Index

- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

## Acceptance / Ready Checklist

- [ ] Project One-pager exists and is up-to-date for active projects
- [ ] Definition of Done documented for the project
- [ ] Release plan & risk register maintained in the project folder
- [ ] Retrospective action items tracked in the backlog

## How to use these docs

- Keep the Project One-pager and release notes updated in the project folder as the single source of truth.
- Add project-specific templates or context into `.copilot/` if you want Copilot Spaces to use them as in-repo context.
- To propose edits to these process documents, use the process doc issue template in `.github/ISSUE_TEMPLATE/`.
```
