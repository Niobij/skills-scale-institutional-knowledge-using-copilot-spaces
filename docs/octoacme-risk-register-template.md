# OctoAcme — Risk Register Template

## Purpose
Provide a structured template for identifying, assessing, and tracking project risks. The Project Manager owns the risk register, but every team member is responsible for surfacing risks. Review and update the register at each weekly delivery sync.

> **Note:** This template is referenced in [Risk Management & Communication](octoacme-risks-and-communication.md) and [Project Planning Guide](octoacme-project-planning.md). For release-specific risks, also review the [Release Readiness Checklist](octoacme-release-readiness-checklist.md).

---

## How to Use This Template

1. **Copy** this file to your project folder (e.g., `docs/risks-<project-name>.md`) or maintain the register inline in your project README.
2. **Add rows** to the Risk Register table as new risks are identified.
3. **Update status** at each weekly delivery sync.
4. **Close risks** by moving them to the Resolved Risks section when they are no longer active.

---

## Risk Register

| ID | Description | Category | Impact | Likelihood | Risk Score | Owner | Mitigation Plan | Contingency Plan | Status | Last Updated |
|---|---|---|---|---|---|---|---|---|---|---|
| R-001 | _Example: Key engineer unavailable during release week_ | Resource | High | Med | High | PM | Identify backup resource; document runbook | Delay release by one sprint | Open | YYYY-MM-DD |
| R-002 | _Example: Third-party API SLA may not meet our latency requirements_ | Technical | Med | Low | Low | Lead Dev | Prototype integration early; define fallback | Implement caching layer | Open | YYYY-MM-DD |

### Field Definitions

| Field | Description |
|---|---|
| **ID** | Unique identifier (R-001, R-002, …) |
| **Description** | Clear, concise description of the risk event |
| **Category** | Technical / Resource / Schedule / External / Compliance / Other |
| **Impact** | Effect if the risk materializes: High / Med / Low |
| **Likelihood** | Probability of occurrence: High / Med / Low |
| **Risk Score** | Derived priority: High (H×H or H×M), Med (M×M or H×L), Low (M×L or L×L) |
| **Owner** | Role or individual responsible for monitoring and mitigating the risk |
| **Mitigation Plan** | Actions taken now to reduce impact or likelihood |
| **Contingency Plan** | Actions to take if the risk materializes |
| **Status** | Open / In Mitigation / Escalated / Resolved |
| **Last Updated** | Date the row was last reviewed or changed |

---

## Risk Lifecycle

```
Identify → Assess → Mitigate → Monitor → Close
```

| Stage | Activity | Frequency |
|---|---|---|
| **Identify** | Surface new risks during planning, standups, or any team discussion | Ongoing |
| **Assess** | Estimate impact and likelihood; assign owner and initial mitigation | At identification |
| **Mitigate** | Execute mitigation actions; update plan if circumstances change | Ongoing |
| **Monitor** | Review all open risks; update status, score, and notes | Weekly delivery sync |
| **Close** | Mark resolved once the risk window has passed or risk is fully mitigated | As appropriate |

---

## Escalation Thresholds

| Risk Score | Action |
|---|---|
| **High** | Escalate to Product Lead and relevant Stakeholders within 24 hours of identification |
| **Med** | Review at next weekly sync; PM decides if stakeholder visibility is needed |
| **Low** | Track in register; review at next sprint/milestone boundary |

---

## Resolved Risks

Move closed risks here to maintain a historical record and inform future retrospectives.

| ID | Description | Resolution | Closed Date |
|---|---|---|---|
| | | | |
