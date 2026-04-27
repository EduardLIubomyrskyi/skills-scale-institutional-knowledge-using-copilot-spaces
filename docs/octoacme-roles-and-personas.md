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

## QA Lead / Test Engineer

### Role Summary
The QA Lead owns the overall test strategy and quality assurance process. They coordinate testing activities across sprints and releases, validate that acceptance criteria are met, and act as a quality gate before features are shipped to production.

### Responsibilities
- Define and maintain the test strategy, test plans, and test cases
- Coordinate unit, integration, regression, and exploratory testing activities
- Validate that features meet Definition of Done and acceptance criteria
- Maintain test environments and coordinate QA readiness for releases
- Identify, document, and track defects to resolution
- Advocate for quality standards in sprint ceremonies and PR reviews

### Goals
- Prevent defects from reaching production
- Reduce regression risk through systematic test coverage
- Ensure a shared understanding of quality expectations across the team

### Typical Communication / Interaction
- Participates in sprint planning, reviews, and retrospectives
- Collaborates daily with Developers during active development and bug triage
- Works with PdM to clarify acceptance criteria and Definition of Ready
- Provides QA sign-off to PM before releases proceed
- Escalates unresolved quality blockers to PM

### Interaction with Existing Roles
- **PM**: Reports QA status; flags quality-related blockers for escalation.
- **PdM (Product Manager)**: Aligns on acceptance criteria and priority of defects; seeks clarification on expected behavior.
- **Developers**: Reviews code changes for testability, pairs on bug reproduction, and verifies fixes.

---

## UX Designer / Product Designer

### Role Summary
UX Designers ensure that features are usable, accessible, and aligned with user needs. They translate product requirements into wireframes, prototypes, and design specifications that guide development.

### Responsibilities
- Conduct user research, usability testing, and design reviews
- Produce wireframes, prototypes, and design assets for features
- Define and maintain the design system and component library
- Ensure designs meet accessibility standards
- Participate in sprint ceremonies to provide design context and feedback
- Collaborate with developers on design implementation fidelity

### Goals
- Deliver user experiences that are intuitive, accessible, and consistent
- Reduce rework by resolving UX ambiguity before development starts
- Establish and enforce design patterns that scale across the product

### Typical Communication / Interaction
- Works ahead of development sprints to provide designs before work begins
- Reviews implemented features against design specs before QA sign-off
- Participates in sprint reviews to give UX feedback
- Shares research insights with PdM and PM to inform prioritization decisions

### Interaction with Existing Roles
- **PM**: Coordinates design timelines so assets are ready before sprint kickoff.
- **PdM (Product Manager)**: Translates product goals and user insights into design direction; validates design decisions against success metrics.
- **Developers**: Provides detailed design specs, answers implementation questions, and reviews built features for design fidelity.

---

## Tech Lead / Engineering Lead

### Role Summary
The Tech Lead provides technical leadership for the delivery team. They guide architectural decisions, uphold engineering standards, and support developers in solving complex technical challenges. They are the primary technical point-of-contact for cross-team integrations.

### Responsibilities
- Make or facilitate key architectural and technical design decisions
- Set and enforce coding standards, review practices, and tech debt policies
- Unblock developers on complex technical issues
- Identify and communicate technical risks and dependencies
- Contribute to estimation and planning from an engineering perspective
- Mentor and grow the technical skills of the development team

### Goals
- Maintain a healthy, sustainable codebase
- Align technical decisions with product goals and business constraints
- Reduce technical risk before it becomes a delivery blocker

### Typical Communication / Interaction
- Attends sprint planning and backlog refinement to provide technical input
- Pairs with PdM and PM to translate technical constraints into planning decisions
- Reviews complex PRs and approves technical design documents
- Reports technical risks to PM for the risk register

### Interaction with Existing Roles
- **PM**: Communicates technical risks, blockers, and dependency updates; assists in timeline estimation.
- **PdM (Product Manager)**: Advises on technical feasibility and trade-offs during backlog grooming and feature scoping.
- **Developers**: Provides technical guidance, performs code reviews, and mentors on best practices.

---

## Security Champion

### Role Summary
The Security Champion is an embedded team member (often a developer or engineer) who promotes security awareness and best practices within the delivery team. They are not a dedicated security officer but act as the team's security focal point.

### Responsibilities
- Identify and communicate security risks for new features during design and planning
- Review code changes and designs for common vulnerability patterns (e.g., OWASP Top 10)
- Ensure security scanning tools are enabled and findings are triaged
- Coordinate with the wider security team or Security on-call for incidents
- Champion secure-by-default practices in the team's engineering culture
- Maintain awareness of relevant compliance requirements

### Goals
- Reduce the likelihood of security vulnerabilities reaching production
- Build a culture of security awareness within the team
- Ensure a fast, clear path for escalating and resolving security findings

### Typical Communication / Interaction
- Participates in design reviews and threat modelling sessions
- Reviews PRs that touch authentication, authorisation, data handling, or infrastructure
- Reports unresolved security findings to PM and escalates to Security on-call where required
- Collaborates with DevOps/Release Engineer on pipeline security controls

### Interaction with Existing Roles
- **PM**: Flags security risks and compliance blockers; advises on security-related scope or timeline impacts.
- **PdM (Product Manager)**: Raises security constraints that may affect feature scope or design decisions.
- **Developers**: Provides security guidance during development, reviews sensitive code changes, and assists with vulnerability remediation.

---

## DevOps / Release Engineer

### Role Summary
The DevOps or Release Engineer owns the CI/CD pipelines, deployment infrastructure, and release processes. They ensure that software can be reliably built, tested, and deployed to any environment.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and deployment automation
- Manage environment configuration, infrastructure-as-code, and secrets management
- Coordinate and execute production deployments and rollbacks
- Monitor system health post-deployment and respond to infrastructure incidents
- Define and document the deployment checklist and rollback procedures
- Collaborate on feature flagging, canary releases, and blue/green deployments

### Goals
- Enable fast, reliable, and repeatable deployments with minimal manual steps
- Reduce deployment risk through automation and staged rollouts
- Maintain clear rollback procedures to minimise customer impact during incidents

### Typical Communication / Interaction
- Works closely with Developers on pipeline integration and build failures
- Coordinates with QA Lead on environment readiness for testing
- Executes releases in collaboration with PM per the release schedule
- Escalates infrastructure incidents and involves the Security Champion for security events

### Interaction with Existing Roles
- **PM**: Provides deployment status updates; confirms readiness for release windows; communicates infrastructure risks.
- **PdM (Product Manager)**: Advises on deployment constraints that may affect feature rollout plans (e.g., feature flags, phased rollouts).
- **Developers**: Supports build and test pipeline integration, reviews infrastructure-as-code changes, and provides deployment tooling guidance.

---

## Stakeholder / Sponsor

### Role Summary
Stakeholders and Sponsors are business owners or executive champions who provide strategic direction, fund the initiative, and approve key decisions. They ensure that project outcomes align with broader business goals.

### Responsibilities
- Provide and maintain executive or business sponsorship for the project
- Define and communicate business priorities, constraints, and success criteria
- Approve project scope, budget, and major milestones at decision gates
- Make or escalate high-level business decisions when the team is blocked
- Receive regular status updates and provide timely feedback
- Champion the project internally to remove organizational blockers

### Goals
- Achieve the intended business or customer outcomes
- Ensure the project remains aligned with strategic priorities
- Enable the team to move quickly by providing clear decisions and removing blockers

### Typical Communication / Interaction
- Attends project kickoff and major milestone reviews
- Receives monthly (or milestone-based) status updates from PM
- Is consulted when risks or blockers require business-level decisions
- Reviews and approves the Project One-pager and release communications

### Interaction with Existing Roles
- **PM**: Primary point of contact for status updates, escalations, and milestone approvals.
- **PdM (Product Manager)**: Aligns on product direction and priorities; approves major scope changes.
- **Developers**: Indirect interaction; may attend demos or review outputs but does not manage day-to-day work.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Templates and Checklists](octoacme-templates-and-checklists.md) for a RACI-lite ownership table mapping key activities to these roles.

