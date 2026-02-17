# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation

Clear escalation paths ensure blockers are resolved quickly. Reference specific role owners from [Roles and Personas](octoacme-roles-and-personas.md) for targeted escalation.

### Escalation Levels
- **Level 1 - Team-level triage** (within 24 hours)
  - Raised in: Daily standup
  - Resolved by: Developers, QA, or DevOps Engineer
  - Examples: Code review delays, test environment issues, clarification on acceptance criteria
  
- **Level 2 - Cross-team or resource escalation** (within 2-3 days)
  - Raised to: Project Manager
  - PM escalates to: Product Lead, dependent teams, or specialized roles (UX Designer, DevOps Engineer, Technical Writer)
  - Examples: Dependency on another team, infrastructure provisioning delays, design decisions needed, resourcing gaps
  
- **Level 3 - Business or strategic escalation** (urgent, executive attention)
  - Raised to: Sponsor or executive leadership
  - Involves: Product Manager, Business Analyst for business impact assessment
  - Examples: Scope changes affecting delivery date, budget overruns, critical external dependencies, security vulnerabilities
  
### Role-Specific Escalation Contacts
- **Technical blockers**: Tech Lead → DevOps Engineer (infrastructure) or Developers
- **Quality issues**: QA/Testing → Developers → Project Manager
- **Design questions**: UX Designer → Product Manager
- **Documentation delays**: Technical Writer → Project Manager
- **Customer impact**: Customer Support Specialist → Product Manager → Business Analyst
- **Infrastructure/deployment**: DevOps Engineer → Infrastructure Lead → CTO
- **Business requirements**: Business Analyst → Product Manager → Sponsor

### Escalation Communication Template
When escalating, provide:
- **Issue description**: Clear summary of the blocker
- **Impact**: How it affects timeline, quality, or scope
- **Attempted resolutions**: What has been tried
- **Requested action**: Specific help needed
- **Urgency**: Timeline for resolution

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled (include cross-functional stakeholders: PM, PdM, UX, Support)
- [ ] Risk register updated weekly
- [ ] **Role assignments clear for all active work items** (Developer, QA, DevOps owner identified)
- [ ] **Design handoffs completed** (UX Designer → Developers, with clear specifications)
- [ ] **Documentation tracking in place** (Technical Writer aligned on release notes and user docs)
- [ ] **Customer Support prepared** for upcoming features (training, FAQ updates)
- [ ] **Escalation paths documented and communicated** to all team members (see [Roles and Personas](octoacme-roles-and-personas.md))
