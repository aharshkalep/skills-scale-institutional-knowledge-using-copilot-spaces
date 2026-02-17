# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with clear ownership tied to roles defined in [Roles and Personas](octoacme-roles-and-personas.md):
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- **Owner** (specific role and person, e.g., "DevOps Engineer - [Team Member Name]")
- Mitigation plan
- Status
- **Escalation contact** (if owner cannot resolve)

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication

Identify stakeholder groups and tailor communication based on their needs and roles. Reference [Roles and Personas](octoacme-roles-and-personas.md) for detailed communication patterns.

### Stakeholder Groups & Communication Needs
- **Engineering team** (Developers, DevOps, QA): Daily standups, technical design reviews, PR comments
- **Product & Design** (Product Manager, UX Designer, Business Analyst): Weekly sync, backlog prioritization, user research findings
- **Documentation & Support** (Technical Writer, Customer Support): Release planning, feature briefs, customer feedback sessions
- **Leadership & Sponsors**: Monthly updates, milestone reviews, escalation of risks/issues
- **External partners/vendors**: As-needed coordination through designated liaison

### Communication Principles
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- **Tailor message to audience**: Technical details for engineers, business impact for leadership, customer implications for support
- **Proactive communication**: Share risks and blockers early, don't wait for stakeholders to ask

## Communication Templates

### Weekly Status Template
**From**: Project Manager  
**To**: Team + Stakeholders  
**Content**:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:
- **Role-specific updates**:
  - Development: [features completed, PRs merged]
  - QA: [testing status, critical bugs]
  - DevOps: [deployment readiness, infrastructure updates]
  - UX: [design reviews completed, user testing findings]
  - Documentation: [docs status, release notes progress]
  - Support: [customer feedback, support ticket trends]

### Incident Communication
**From**: DevOps Engineer (technical lead) + Project Manager (coordination)  
**To**: Stakeholders + affected teams  
**Content**:
- Triage summary
- Actions being taken (specify which roles are involved)
- Expected timeline
- Customer impact and mitigation (input from Customer Support)
- Post-incident blameless retrospective scheduled
- **Communication lead**: Project Manager coordinates updates
- **Technical lead**: DevOps Engineer drives resolution

### Release Communication
**From**: Product Manager + Project Manager  
**To**: All stakeholders  
**Content**:
- Release summary and business value
- Key features and changes (from Product Manager)
- Technical details (from DevOps Engineer)
- Documentation links (from Technical Writer)
- Support readiness (from Customer Support Specialist)
- Success metrics to track (from Business Analyst)

## Escalation Paths

Clear escalation paths ensure issues are resolved at the appropriate level. All roles and contacts are defined in [Roles and Personas](octoacme-roles-and-personas.md).

### Standard Escalation Hierarchy
**Level 1 - Team Resolution** (0-24 hours)
- **For technical issues**: Developer → Tech Lead → DevOps Engineer (if infrastructure-related)
- **For quality issues**: QA/Testing → Developer → Tech Lead
- **For design questions**: Developer → UX Designer → Product Manager
- **For documentation gaps**: Any team member → Technical Writer

**Level 2 - Cross-Team / Resource Escalation** (1-3 days)
- **Project Manager** coordinates resolution across teams
- Escalates to: Product Lead, dependent team leads, specialized roles
- Involves: Business Analyst (for business impact), Customer Support (for customer impact)

**Level 3 - Executive / Business Escalation** (urgent)
- **Product Manager** or **Project Manager** escalates to Sponsor/leadership
- Requires: Business case from Business Analyst, customer impact from Customer Support
- Examples: Major scope changes, budget issues, strategic pivots, critical security vulnerabilities

### Role-Specific Escalation Contacts
- **Infrastructure/deployment issues**: DevOps Engineer → Infrastructure Lead → CTO
- **Security incidents**: Follow security runbook, notify Security on-call immediately
- **Product direction**: Product Manager → VP Product
- **Customer-impacting bugs**: Customer Support → Product Manager → Engineering Lead
- **Resource constraints**: Project Manager → Resource Manager → Department Lead
- **Design conflicts**: UX Designer → Design Lead → Product Manager
- **Documentation delays**: Technical Writer → Project Manager → Product Manager

### Escalation Guidelines
- Always try team-level resolution first (Level 1)
- Document the issue and attempted solutions before escalating
- Use the escalation communication template (see above)
- Loop in appropriate roles based on issue type (reference [Roles and Personas](octoacme-roles-and-personas.md))
- For urgent production issues, escalate immediately to Level 2 or 3 as appropriate
