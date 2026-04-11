# OctoAcme — Release Readiness Checklist

## Purpose
Ensure every release is deliberate, verified, and safe to ship. Complete this checklist before promoting any build to production. Skipped items must be documented with a rationale and owner.

> **Note:** This checklist is referenced in [Release & Deployment Guide](octoacme-release-and-deployment.md). For risk items surfaced during this review, log them in the [Risk Register Template](octoacme-risk-register-template.md).

---

## Release Metadata

| Field | Value |
|---|---|
| Release name / version | |
| Target release date | |
| Release manager | |
| Release type (Patch / Minor / Major) | |
| Related issue(s) / PR(s) | |

---

## 1. Code & Feature Completeness

- [ ] All planned work items are merged and the sprint/milestone is closed
- [ ] No open P1 or P2 defects against this release
- [ ] Feature flags configured correctly for production (enabled / disabled as planned)
- [ ] All items satisfy the team's [Definition of Done](octoacme-definition-of-done.md)

## 2. Quality Assurance

- [ ] Full regression test suite executed and passed
- [ ] Exploratory / manual QA completed for high-risk user flows
- [ ] Performance and load testing completed (if applicable)
- [ ] Accessibility checks completed for user-facing changes
- [ ] QA Lead has provided formal sign-off

## 3. Security & Compliance

- [ ] SAST and dependency vulnerability scans pass with no new critical/high findings
- [ ] Secrets, credentials, and API keys confirmed absent from source code and build artifacts
- [ ] Data privacy / compliance review completed (if handling PII or regulated data)
- [ ] Security team sign-off obtained (if required by policy)

## 4. Documentation & Communication

- [ ] Release notes drafted and reviewed
- [ ] User-facing documentation (help docs, API docs) updated
- [ ] Internal runbook / operations docs updated
- [ ] Stakeholder preview or demo completed (if required)
- [ ] Support team briefed on known issues and workarounds

## 5. Infrastructure & Deployment

- [ ] Deployment pipeline tested in staging environment
- [ ] Staging smoke tests passed
- [ ] Database migrations reviewed and tested (if applicable)
- [ ] Environment configuration (env vars, secrets, feature flags) verified for production
- [ ] Monitoring and alerting dashboards reviewed and updated
- [ ] Rollback plan documented and communicated to the team

## 6. Go / No-Go Decision

| Role | Name | Decision (Go / No-Go) | Notes |
|---|---|---|---|
| QA Lead | | | |
| DevOps Engineer | | | |
| Product Manager | | | |
| Project Manager | | | |
| Stakeholder (if required) | | | |

> **Policy:** All mandatory approvers must mark "Go" before deploying to production. Any "No-Go" blocks the release until the blocking issue is resolved and the approver re-reviews.

---

## Post-Release Verification

- [ ] Post-deploy smoke tests passed in production
- [ ] Key metrics and dashboards show expected behavior
- [ ] Release announcement sent to stakeholders and support team
- [ ] Any follow-up issues logged in the backlog
- [ ] Retrospective item created to capture lessons learned from this release
