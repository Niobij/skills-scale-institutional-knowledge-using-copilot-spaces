# OctoAcme — Definition of Done

## Purpose
Provide a shared, team-wide checklist of criteria that every piece of work must satisfy before it is considered "Done." Using a consistent Definition of Done (DoD) reduces ambiguity, prevents rework, and gives every role a clear view of what "complete" means.

> **Note:** This document is referenced in [Execution & Tracking](octoacme-execution-and-tracking.md). Update this DoD as the team's practices evolve; communicate changes in a retrospective action item.

---

## Team-Wide Definition of Done

The following criteria apply to **all** work items (features, bugs, improvements) unless a role-specific exception is explicitly documented in the issue or PR.

### Code & Implementation
- [ ] Code written and reviewed by at least one other Developer
- [ ] All automated tests pass (unit, integration, and any applicable end-to-end tests)
- [ ] No new linting or static-analysis errors introduced
- [ ] Security scanning (SAST/dependency check) passes in CI

### Documentation
- [ ] Inline code comments added where logic is non-obvious
- [ ] User-facing changes reflected in release notes or changelog
- [ ] Any new configuration or environment variables documented in the repo README or runbook

### Quality & Acceptance
- [ ] Acceptance criteria from the linked issue are verified
- [ ] QA Lead sign-off obtained (manual testing complete where required)
- [ ] No open P1 or P2 defects against this work item

### Deployment Readiness
- [ ] Feature flag or rollout strategy documented (if applicable)
- [ ] Rollback plan identified and communicated to the team
- [ ] Monitoring/alerting updated or confirmed sufficient for the change

### Process
- [ ] Pull Request linked to the relevant issue
- [ ] Issue/ticket status updated to "Done" on the project board
- [ ] Any follow-up items captured as new issues in the backlog

---

## Role-Specific Expectations

### Developers
- Unit tests cover all new or changed business logic
- PR description summarizes what changed, why, and how to verify it
- No known TODOs left untracked (link to a follow-up issue if work is deferred)

### QA Lead
- Test plan or exploratory test notes attached to the issue or PR
- Automated regression suite updated to cover new acceptance criteria
- Defect count and severity documented in the sprint review artifacts

### DevOps Engineer
- CI/CD pipeline updated to handle any new build, test, or deployment steps
- Infrastructure changes reviewed, applied, and reflected in IaC source control
- Runbook updated for any new operational procedures

### UX Designer
- Final design artifacts (specs, annotated screenshots) linked from the issue
- Usability acceptance criteria verified — either through test sessions or stakeholder sign-off
- Design system components updated or new components documented

### Product Manager
- Acceptance criteria confirmed as met
- Success metrics baseline captured (before/after data plan in place)
- Stakeholder demo or review completed (if required for this item)

### Project Manager
- Work item status updated in the project tracker
- Any scope changes reflected in the project plan and communicated to Stakeholders
- Risks or dependencies resolved or carried forward to the risk register

---

## Updating This Document
1. Propose changes in a retrospective or team discussion.
2. Open a PR updating this file; request review from all role leads.
3. Merge and announce the updated DoD in the next team standup.
