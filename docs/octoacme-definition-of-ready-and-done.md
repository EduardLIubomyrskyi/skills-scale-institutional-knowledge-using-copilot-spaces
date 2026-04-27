# OctoAcme — Definition of Ready & Definition of Done

## Purpose
Standardize the entry and exit criteria for backlog items so that the entire team shares a common understanding of when work can begin and when work is complete.

---

## Definition of Ready (DoR)

A backlog item is **Ready** to be pulled into a sprint when **all** of the following criteria are met:

### Story / Feature Level
- [ ] A clear problem statement or user story exists (e.g., "As a [persona], I want [goal] so that [outcome]")
- [ ] Acceptance criteria are written and reviewed by PdM and QA Lead
- [ ] The item is estimated (story points or T-shirt size)
- [ ] Dependencies are identified and either resolved or have a mitigation plan
- [ ] UX designs or wireframes are available (for user-facing features)
- [ ] Security considerations have been noted by the Security Champion (for sensitive features)
- [ ] The item fits within the team's sprint capacity

### Bug / Hotfix Level
- [ ] Steps to reproduce are documented
- [ ] Expected vs. actual behaviour is described
- [ ] Severity and priority are assigned
- [ ] A fix approach has been agreed with the Tech Lead

> **Owner**: PdM owns DoR compliance for features; PM is responsible for ensuring the sprint backlog only contains Ready items at sprint kickoff.

---

## Definition of Done (DoD)

A backlog item is **Done** when **all** of the following criteria are met:

### Code & Development
- [ ] Code is implemented and reviewed (at least one approval from a peer or Tech Lead)
- [ ] All automated tests pass (unit, integration, and any relevant end-to-end tests)
- [ ] No new linting or static analysis warnings introduced
- [ ] Security scan passes with no new critical or high findings (reviewed by Security Champion if flagged)

### Quality & Testing
- [ ] Acceptance criteria verified by QA Lead (or agreed team member for low-risk items)
- [ ] Manual exploratory testing completed for user-facing changes
- [ ] Regression tests updated or new tests added to cover the change
- [ ] Defects found during QA are either fixed or explicitly deferred (with PdM sign-off)

### Documentation & Handoffs
- [ ] PR description includes a link to the issue and a summary of changes
- [ ] Relevant documentation updated (README, API docs, runbooks, or user guides)
- [ ] Release notes entry drafted (if applicable)
- [ ] Feature flag configuration documented (if applicable)

### Deployment Readiness
- [ ] Change is merged to the target branch and CI is green
- [ ] Deployed to staging and smoke tests passed
- [ ] Rollback plan or feature flag toggle documented (for significant changes)

> **Owner**: QA Lead is the primary gate-keeper for DoD compliance. PM confirms DoD is met before marking items as complete on the project board.

---

## Role Handoff Points

| Handoff | From | To | Gate |
|---|---|---|---|
| Item enters sprint | PdM | Developers | DoR met |
| Development complete, awaiting QA | Developers | QA Lead | PR approved, CI green |
| QA approved, awaiting release | QA Lead | DevOps/Release Engineer | DoD met |
| Release complete, stakeholder update | DevOps/Release Engineer | PM | Post-deploy verification passed |

---

## Related Documents
- [Project Planning](octoacme-project-planning.md) — backlog item template and planning checklist
- [Execution and Tracking](octoacme-execution-and-tracking.md) — board workflow and PR conventions
- [Release and Deployment](octoacme-release-and-deployment.md) — deployment checklist
- [Templates and Checklists](octoacme-templates-and-checklists.md) — decision log, risk register, and RACI-lite table
