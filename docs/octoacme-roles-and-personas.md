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

## QA Lead

### Role Summary
The QA Lead oversees test planning, execution, and release readiness. They work with Developers and Product Managers to ensure requirements are testable and quality standards are met before any release.

### Responsibilities
- Define and maintain test strategies, test plans, and quality metrics
- Coordinate manual and automated test execution across sprints
- Own the team's [Definition of Done](octoacme-definition-of-done.md) and ensure it is applied consistently
- Lead defect triage, regression testing, and sign-off processes
- Gate releases against quality criteria using the [Release Readiness Checklist](octoacme-release-readiness-checklist.md)

### Goals
- Ship features that meet acceptance criteria and are free of critical defects
- Establish and improve test automation coverage over time
- Provide clear quality signals to the team before every release

### Typical Communication
- Sprint ceremonies (planning, review, retrospective)
- Defect reports and QA status updates shared with the Project Manager
- Acceptance sign-off and go/no-go recommendations to the Project Manager

### Interaction
- **Developers**: Collaborates during implementation and code review to review testability; triages defects together.
- **Product Managers**: Clarifies acceptance criteria and confirms when features meet stated requirements.
- **Project Managers**: Reports on quality status and provides input for go/no-go release decisions.
- **DevOps Engineers**: Partners on CI/CD test automation, test-environment provisioning, and pipeline gates.

---

## DevOps Engineer

### Role Summary
The DevOps Engineer builds and operates CI/CD pipelines, automates infrastructure, and ensures reliable, repeatable delivery from code commit to production. They are the primary owner of deployment tooling and operational observability.

### Responsibilities
- Maintain and improve build, test, and deployment pipelines
- Ensure production observability, reliability, and security baselines
- Automate provisioning, configuration management, and monitoring
- Support incident response, backup, and recovery procedures
- Contribute to the [Release Readiness Checklist](octoacme-release-readiness-checklist.md) for infrastructure and pipeline gates

### Goals
- Reduce lead time from code-complete to production
- Eliminate manual, error-prone deployment steps
- Provide the team with fast, reliable feedback loops

### Typical Communication
- Deployment status updates to the Project Manager
- Incident notifications and post-mortems shared with the full team
- Pipeline and environment documentation maintained in the project repo

### Interaction
- **Developers**: Supports deployment needs, reviews infrastructure-as-code changes, and provides environment access.
- **QA Leads**: Collaborates on test environment provisioning and automated quality gates in CI/CD.
- **Project Managers**: Communicates deployment schedules, incidents, and pipeline blockers.
- **Stakeholders**: Provides availability and reliability metrics relevant to business commitments.

---

## UX Designer

### Role Summary
The UX Designer ensures that products are usable, accessible, and aligned with real user needs. They translate user research and business goals into design artifacts that guide development.

### Responsibilities
- Collaborate with Product Managers to define user journeys and experience goals
- Create wireframes, prototypes, and interaction specifications
- Plan and facilitate usability tests; synthesize and share findings
- Advocate for accessible, inclusive design decisions throughout the project lifecycle
- Iterate on designs based on user feedback and development constraints

### Goals
- Deliver experiences that users find intuitive and valuable
- Reduce rework caused by late-stage usability issues
- Maintain design consistency across features and releases

### Typical Communication
- Design reviews with Product Managers and Developers at the start of each feature
- Usability test reports shared with the full team
- Design specifications and annotated prototypes linked from feature issues or PRs

### Interaction
- **Product Managers**: Co-defines user journeys, success metrics, and acceptance criteria at the planning stage.
- **Developers**: Provides design specifications and is available for implementation questions; reviews UI against designs before QA.
- **QA Leads**: Shares usability acceptance criteria and participates in acceptance testing of UX-critical flows.
- **Stakeholders**: Presents design concepts and usability findings to align on experience goals and get approval on major design directions.

---

## Stakeholder

### Role Summary
Stakeholders provide the business context that shapes what gets built and why. They approve initiatives, review outcomes, and ensure that product development aligns with organizational objectives and customer needs.

### Responsibilities
- Define success criteria and high-level business goals for initiatives
- Provide timely feedback on deliverables, demos, and proposed trade-offs
- Participate in key decision gates (initiation approval, release sign-off)
- Sponsor projects and resolve escalated blockers that require executive or cross-department action
- Review project outcomes against defined success metrics

### Goals
- Ensure investment in the right initiatives for the right reasons
- Maintain visibility into project health without being in the day-to-day
- Achieve business outcomes that justify project investment

### Typical Communication
- Monthly or milestone-based status updates from the Project Manager
- Demo participation at sprint/milestone reviews
- Escalation notifications when business-impacting risks or blockers arise

### Interaction
- **Product Managers**: Aligns on roadmap priorities, success metrics, and trade-offs; reviews business-case assumptions.
- **Project Managers**: Receives regular status reports; is consulted on scope changes, resource needs, and escalations.
- **Developers**: Reviews demo outputs and provides business feedback on delivered features.
- **UX Designers**: Reviews proposed experience directions and approves major design decisions that affect customers or brand.

---

## Role Interaction Map

The table below summarizes the primary handoffs and decision points between roles.

| From → To | Key Handoffs & Decision Points |
|---|---|
| **Stakeholder → Product Manager** | Business goals, success metrics, initiative approval |
| **Product Manager → Developers** | Prioritized backlog, acceptance criteria, feature specs |
| **Product Manager → UX Designer** | User journey requirements, experience goals |
| **UX Designer → Developers** | Design specs, prototypes, usability acceptance criteria |
| **UX Designer → QA Lead** | UX acceptance criteria for usability testing |
| **Developers → QA Lead** | Features ready for testing; defect resolutions |
| **QA Lead → Project Manager** | Quality status, go/no-go recommendation for release |
| **QA Lead → DevOps Engineer** | Test automation requirements, pipeline gate criteria |
| **DevOps Engineer → Developers** | Environment access, deployment tooling, pipeline feedback |
| **DevOps Engineer → Project Manager** | Deployment schedule, pipeline incidents, infrastructure risks |
| **Project Manager → Stakeholder** | Status reports, risk escalations, release approvals |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

