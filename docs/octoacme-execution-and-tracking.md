# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
  - Items move to **Ready** only when they meet the [Definition of Ready](octoacme-definition-of-ready-and-done.md)
  - Items move to **Done** only when they meet the [Definition of Done](octoacme-definition-of-ready-and-done.md)
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
  - Tech Lead reviews PRs for complex or high-risk changes
  - Security Champion reviews PRs that touch authentication, authorisation, or data handling

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (findings reviewed by Security Champion)
- Manual QA for feature acceptance when needed (coordinated by QA Lead)
- QA Lead provides sign-off before items move to Done — see [Definition of Done](octoacme-definition-of-ready-and-done.md)

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly (see [Templates and Checklists](octoacme-templates-and-checklists.md))
- [ ] [Definition of Ready and Done](octoacme-definition-of-ready-and-done.md) shared with and agreed by the team
- [ ] QA Lead identified and test approach confirmed
- [ ] Tech Lead identified for technical reviews
- [ ] Security Champion engaged for security-sensitive features
