# OctoAcme Project Management Docs

Welcome! This README serves as the primary entry point for all OctoAcme project management process documentation. Use the links in the index below to navigate to guidelines, workflows, and templates covering how we run projects at OctoAcme.

## Overview

OctoAcme runs projects using a lightweight, lifecycle-based approach that moves from **Initiation → Planning → Execution → Release → Close/Retrospective**. During initiation, teams validate the business need and intended outcome, identify stakeholders and champions, define success criteria and metrics, and produce a minimal set of artifacts — a Project One-pager (problem, objective, success metrics), an initial timeline with milestones, and a starter risk list. Work proceeds into planning only after a clear decision gate: success metrics are defined, stakeholders align on priority, and team availability is confirmed.

In planning, OctoAcme turns an approved initiative into an actionable backlog and delivery plan. The team holds a kickoff, breaks work into shippable increments, documents acceptance criteria and a Definition of Done, and estimates scope using T-shirt sizing or story points. Dependencies and integration points are identified early and tracked explicitly, with risks captured in a simple risk register (impact, likelihood, owner, mitigation, status). Planning outputs include a prioritized backlog, a milestone/release map, and a draft QA approach. During execution and tracking, the team relies on a consistent operating rhythm: a GitHub Projects board manages flow through **Backlog → Ready → In Progress → In Review → QA → Done**, supported by daily standups for blockers and dependencies, weekly delivery syncs for progress and risk review, and demos at the end of each sprint or milestone. Core personas are clearly separated — **Project Manager** coordinates delivery, schedules, risk, and communications; **Product Manager** defines outcomes and priorities; **Developers** implement, test, and collaborate on design; **QA/Testing** validates acceptance criteria; and **Stakeholders** provide inputs and approvals. Blockers escalate from team triage to PM-led cross-team escalation, and up to sponsor level when business impact is significant.

Quality assurance is built into both development and release practices. The team keeps pull requests small, links issues and acceptance criteria in PRs, and runs automated tests, linting, and security scanning in CI before review — requiring at least one approval to merge. Testing expectations scale with risk: unit tests for all new logic, integration tests where needed, and end-to-end smoke tests for critical flows before release, with manual QA used for feature acceptance when appropriate. Releases follow a standardized deployment checklist: acceptance criteria met, CI/security checks passing, release notes prepared, rollback and mitigation plans documented, staged deployment plus smoke tests, post-deploy verification, and stakeholder announcements. Each release is followed by a retrospective that converts learnings into owned, time-bound actions tracked on the project backlog.

## Process Documentation Index

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level overview of OctoAcme's project management philosophy and lifecycle |
| [Project Initiation Guide](octoacme-project-initiation.md) | Validating business need, defining success metrics, and producing initiation artifacts |
| [Project Planning Guide](octoacme-project-planning.md) | Backlog creation, milestone mapping, estimation, and risk register setup |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Board workflow, standups, syncs, demos, and escalation paths |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register maintenance, communication cadence, and stakeholder updates |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Deployment checklist, staged rollout, rollback plans, and release announcements |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retro format, action tracking, and continuous improvement practices |
| [Roles and Personas](octoacme-roles-and-personas.md) | Definitions and responsibilities for each role on an OctoAcme project team |

## How to Use These Docs

These documents are the **single source of truth** for OctoAcme project management practices. When starting a new project, begin with the [Project Management Overview](octoacme-project-management-overview.md) and then follow the lifecycle guides in order. Keep all project artifacts (one-pagers, risk registers, backlog items, release notes, and retro action items) updated as work progresses so the team always has an accurate picture of project status. If a process needs to change, update the relevant document and communicate the change to the team so that everyone is working from the same playbook.
