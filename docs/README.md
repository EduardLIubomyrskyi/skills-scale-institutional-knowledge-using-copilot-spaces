# OctoAcme Project Management Docs

Welcome to the OctoAcme project management documentation hub. This README is the entry point for understanding how OctoAcme plans, executes, and ships work. The docs below capture the practices, templates, and checklists that keep our cross-functional teams aligned and moving fast.

## Overview of OctoAcme Project Management Processes

OctoAcme follows a structured lifecycle that moves from **initiation** through **planning**, **execution and tracking**, **release**, and finally **retrospective**. Each phase has clear deliverables—such as a Project One-pager, Sprint Backlog, Release Checklist, and Retrospective Action Items—so that work is always visible and decisions are traceable. Projects are approved at defined decision gates (e.g., go/no-go after initiation) to ensure teams invest effort only in validated, well-scoped work.

Delivery relies on a set of clearly defined **personas and roles**: the Project Manager (PM) coordinates schedules, risks, and communications; the Product Manager (PdM) owns the vision, backlog priority, and success metrics; Developers implement features and maintain testability; QA/Testing validates acceptance criteria and quality gates; and Stakeholders provide inputs, approvals, and ongoing alignment. Clear ownership—every project has a named PM and Product Lead—is one of OctoAcme's core principles.

**Communication** is predictable and documented. Twice-weekly standups keep the delivery team synchronized, a weekly PM–PdM sync drives cross-functional alignment, and monthly stakeholder updates maintain executive visibility. A single source of truth (the project README or release doc) is the authoritative status record, backed by standardized templates for weekly status reports and incident communications. Escalation paths run from the team level up through the PM, Product Lead, and Sponsor so blockers never stall silently.

**Quality assurance** is built into every phase. Acceptance criteria and a Definition of Done are defined during planning, continuous integration and security scans run on every pull request, and code reviews are standard practice. Before any release, all PRs must be merged with passing CI, smoke tests must pass in staging, and a rollback plan must be documented. After release, post-deploy verifications and a blameless retrospective close the loop and feed improvements back into the backlog.

---

## Document Index

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and the high-level lifecycle |
| [Project Initiation](octoacme-project-initiation.md) | How to validate and authorize new work; the Project One-pager template and initiation checklist |
| [Project Planning](octoacme-project-planning.md) | Scope definition, milestone planning, backlog preparation, and the planning checklist |
| [Execution and Tracking](octoacme-execution-and-tracking.md) | Sprint ceremonies, daily standups, progress tracking, and managing scope changes |
| [Risks and Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, stakeholder communication templates |
| [Release and Deployment](octoacme-release-and-deployment.md) | Release types, deployment checklist, rollback playbook, and release notes template |
| [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retrospective structure, action item tracking, and continuous improvement culture |
| [Roles and Personas](octoacme-roles-and-personas.md) | Detailed responsibilities and communication patterns for each persona |
| [Definition of Ready & Done](octoacme-definition-of-ready-and-done.md) | Standardized DoR/DoD criteria and role handoff points |
| [Templates and Checklists](octoacme-templates-and-checklists.md) | Decision log, risk register, RACI-lite table, and handoff checklists |

---

## How to Use These Docs

1. **New to OctoAcme?** Start with the [Project Management Overview](octoacme-project-management-overview.md) and [Roles and Personas](octoacme-roles-and-personas.md) to understand the principles and who does what.
2. **Starting a new project?** Follow the [Project Initiation](octoacme-project-initiation.md) guide to complete the One-pager and pass the decision gate before investing in detailed planning.
3. **In active delivery?** Use [Execution and Tracking](octoacme-execution-and-tracking.md) for sprint ceremonies and [Risks and Communication](octoacme-risks-and-communication.md) for status updates and escalations.
4. **Preparing a release?** Follow the [Release and Deployment](octoacme-release-and-deployment.md) checklist end-to-end, including staging smoke tests and post-deploy verification.
5. **After a sprint or release?** Run a retrospective using the [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) guide and feed action items back into the backlog.
6. **Using Copilot Spaces?** Copy the relevant docs into your `.copilot/` folder so Copilot can use them as context when answering project-specific questions.
