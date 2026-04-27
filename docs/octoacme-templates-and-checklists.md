# OctoAcme — Templates & Checklists

## Purpose
Provide lightweight, reusable templates and ownership tables for common project management activities. These templates reduce ad-hoc tracking and ensure consistent documentation across projects.

---

## Decision Log Template

Use this log to record significant decisions made during a project. Maintain one decision log per project, stored in the project's `docs/` or repo root.

| ID | Date | Decision | Rationale | Alternatives Considered | Owner | Status |
|---|---|---|---|---|---|---|
| D-001 | YYYY-MM-DD | Short description of the decision | Why this option was chosen | Other options evaluated | Name/Role | Accepted / Superseded |
| D-002 | | | | | | |

**Fields:**
- **ID**: Sequential identifier for cross-referencing (e.g., in risk entries or PRs).
- **Date**: When the decision was made.
- **Decision**: A concise statement of what was decided.
- **Rationale**: The key reason(s) for choosing this option.
- **Alternatives Considered**: Other options that were evaluated and why they were not selected.
- **Owner**: The person or role accountable for the decision (typically PM or PdM).
- **Status**: `Accepted` (active), `Superseded` (replaced by a later decision), or `Deferred`.

> **Tip**: Link decision IDs in PR descriptions, risk entries, and retrospective notes for full traceability.

---

## Risk Register Template

Maintain one risk register per project. Review and update at every weekly PM sync. See [Risks and Communication](octoacme-risks-and-communication.md) for the risk lifecycle.

| ID | Description | Category | Impact | Likelihood | Score | Owner | Mitigation Plan | Status | Last Reviewed |
|---|---|---|---|---|---|---|---|---|---|
| R-001 | Short risk description | Technical / Schedule / Resource / External | High / Med / Low | High / Med / Low | H×H=High | Name/Role | Steps to reduce or accept the risk | Open / Mitigated / Closed | YYYY-MM-DD |
| R-002 | | | | | | | | | |

**Score guidance** (Impact × Likelihood):
- High × High = **Critical** — escalate immediately
- High × Med or Med × High = **High** — active mitigation required
- Med × Med = **Medium** — monitor weekly
- Low × any = **Low** — log and revisit if status changes

**Categories:**
- **Technical**: architecture, performance, security, dependencies
- **Schedule**: timeline, resource availability, external deadlines
- **Resource**: staffing, budget, tooling
- **External**: third-party services, regulatory, market changes

> **Owner**: PM facilitates the risk register; each risk has an individual owner responsible for executing the mitigation plan.

---

## RACI-Lite Ownership Table

This table maps common project activities to the primary roles. Use it as a starting point and adjust to reflect your team's actual structure.

**Key:**
- **R** = Responsible (does the work)
- **A** = Accountable (final decision-maker / sign-off)
- **C** = Consulted (provides input)
- **I** = Informed (kept up to date)

| Activity | PM | PdM | Tech Lead | Developers | QA Lead | UX Designer | Security Champion | DevOps/Release Eng | Stakeholder/Sponsor |
|---|---|---|---|---|---|---|---|---|---|
| Project initiation & One-pager | R | C | C | I | I | I | I | I | A |
| Backlog grooming & prioritisation | C | A | C | C | C | C | C | I | I |
| Sprint planning | A | C | C | R | C | C | I | I | I |
| Technical design & architecture | I | C | A | R | C | C | C | C | I |
| UX design & prototyping | I | C | I | C | C | A | I | I | I |
| Feature development | I | I | C | R | I | C | C | I | I |
| Code review | I | I | A | R | I | I | C | I | I |
| Security review | C | I | C | C | I | I | A | C | I |
| QA testing & sign-off | C | C | I | R | A | I | I | I | I |
| Release preparation & deployment | A | C | C | C | C | I | C | R | I |
| Post-deploy verification | C | I | C | C | C | I | C | A | I |
| Stakeholder status updates | R | C | I | I | I | I | I | I | A |
| Risk register maintenance | A | C | C | C | I | I | C | C | I |
| Decision log maintenance | A | C | C | I | I | I | I | I | I |
| Retrospective facilitation | A | C | C | R | R | R | R | R | I |

---

## Handoff Checklist Templates

### Planning → Execution Handoff
Used at the end of sprint planning or project planning to confirm readiness to start execution.

- [ ] Sprint goal is documented and agreed by PM and PdM
- [ ] All sprint items meet the [Definition of Ready](octoacme-definition-of-ready-and-done.md)
- [ ] UX designs are available for all user-facing items
- [ ] Tech Lead has reviewed technical approach for complex items
- [ ] Security Champion has flagged any security considerations
- [ ] Risk register is up to date for the sprint period
- [ ] Decision log updated with any planning decisions made

### Development → QA Handoff
Used when a developer marks a feature as ready for QA.

- [ ] PR is merged or a test branch is deployed to the test environment
- [ ] CI is green (all tests pass, no new security scan findings)
- [ ] PR description includes acceptance criteria and testing notes
- [ ] Developer has performed a basic smoke test
- [ ] Known limitations or deferred items are documented in the PR

### QA → Release Handoff
Used when QA Lead approves a feature/release candidate for deployment.

- [ ] All acceptance criteria verified and documented
- [ ] Regression tests updated and passing
- [ ] Release notes entry confirmed
- [ ] DevOps/Release Engineer notified of release readiness
- [ ] Rollback plan confirmed with DevOps/Release Engineer
- [ ] PM informed of QA sign-off

### Release → Stakeholder Handoff
Used after a successful production deployment.

- [ ] Post-deploy verification completed by DevOps/Release Engineer
- [ ] Release notes published or distributed
- [ ] Stakeholders/Sponsor notified (PM sends update)
- [ ] Monitoring dashboards confirmed healthy
- [ ] Retrospective or release review scheduled (if applicable)

---

## Related Documents
- [Definition of Ready & Done](octoacme-definition-of-ready-and-done.md) — entry and exit criteria for backlog items
- [Roles and Personas](octoacme-roles-and-personas.md) — full role descriptions and interaction models
- [Risks and Communication](octoacme-risks-and-communication.md) — risk lifecycle and communication templates
- [Project Planning](octoacme-project-planning.md) — backlog item template and planning checklist
- [Execution and Tracking](octoacme-execution-and-tracking.md) — board workflow and PR conventions
- [Release and Deployment](octoacme-release-and-deployment.md) — deployment checklist and rollback playbook
