# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles

OctoAcme projects are **cross-functional by design**, bringing together diverse specialists to deliver comprehensive solutions. Each role contributes unique expertise throughout the project lifecycle.

### Leadership & Coordination
- **Project Manager (PM)**: coordinates delivery, schedules, risk, communications.
- **Product Manager (PdM)**: defines outcomes, prioritizes backlog, and measures success.

### Delivery & Technical
- **Developers**: implement features, collaborate on design and testability.
- **DevOps Engineer**: builds CI/CD pipelines, manages infrastructure, ensures reliable deployments.
- **QA/Testing**: validate quality and acceptance criteria.

### User Experience & Documentation
- **UX Designer**: creates user-centered designs, conducts user research, ensures accessibility.
- **Technical Writer**: produces user guides, API docs, and release notes for clarity.

### Business & Support
- **Business Analyst**: gathers requirements, analyzes data, validates business outcomes.
- **Customer Support Specialist**: provides customer assistance, escalates issues, shares feedback.
- **Stakeholders**: provide inputs, approvals, and strategic guidance.

**For detailed responsibilities, goals, and communication patterns for each role, see [OctoAcme Roles and Personas](octoacme-roles-and-personas.md).**

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence & Stakeholder Engagement

Effective communication is essential for cross-functional success. OctoAcme emphasizes **proactive stakeholder engagement** throughout the project lifecycle, not just at milestones.

### Regular Cadence
- **Weekly sync**: PM + PdM alignment on priorities and risks
- **Twice-weekly standups**: Delivery team (developers, QA, DevOps) progress and blockers
- **Bi-weekly design reviews**: UX Designer shares prototypes with product and engineering
- **Monthly stakeholder updates**: Broad communication to leadership, support, and business stakeholders
- **Sprint demos**: Show working software to cross-functional stakeholders for feedback

### Continuous Engagement
- **Customer Support**: Daily ticket triage, weekly trends review with product/engineering
- **Business Analyst**: Regular requirement workshops and data reviews with stakeholders
- **Technical Writer**: Ongoing collaboration with developers and product for documentation accuracy
- **DevOps Engineer**: Infrastructure planning and incident response as needed

### Ad-hoc Communication
- Escalations for blockers, risks, or decisions
- Incident response and post-mortems
- Architecture and technical design reviews

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
