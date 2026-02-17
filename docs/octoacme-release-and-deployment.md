# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (verified by DevOps Engineer)
- **Release notes drafted** (Owner: Technical Writer, input from PM and Product Manager)
- **User documentation updated** (Owner: Technical Writer)
- Rollback / mitigation plan documented (Owner: DevOps Engineer)
- Smoke tests prepared (Owner: QA/Testing)
- **Customer Support briefed** on release changes, known issues, and FAQs (Owner: Product Manager)
- **Stakeholder notifications prepared** (Owner: Project Manager)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable) — **DevOps Engineer**
- [ ] Deploy to staging and run smoke tests — **DevOps Engineer, QA/Testing**
- [ ] Deploy to production (automated pipeline preferred) — **DevOps Engineer**
- [ ] Run post-deploy verifications — **QA/Testing, DevOps Engineer**
- [ ] **Verify monitoring and alerts are functioning** — **DevOps Engineer**
- [ ] Announce release to stakeholders and support — **Project Manager**
- [ ] **Update user-facing documentation** (help center, API docs) — **Technical Writer**
- [ ] **Notify Customer Support** with release summary and support guide — **Product Manager**
- [ ] **Update status page** (if applicable) — **DevOps Engineer**

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **DevOps Engineer** triggers incident response and notifies on-call
  - **Project Manager** coordinates communication to stakeholders
  - **DevOps Engineer** executes rollback to last known-good release if necessary
  - **Customer Support** monitors incoming tickets and provides updates to affected customers
  - **Technical Writer** updates status page and incident communications
  - Cross-functional team (PM, PdM, DevOps, Developer, QA) triages root cause and captures action items
  - **Business Analyst** assesses customer and business impact
  
For detailed role responsibilities during incidents, see [Roles and Personas](octoacme-roles-and-personas.md).

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
