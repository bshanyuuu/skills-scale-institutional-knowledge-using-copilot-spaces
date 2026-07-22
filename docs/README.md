# OctoAcme Project Management Docs

Welcome to the OctoAcme Project Management documentation hub. This repository contains comprehensive guides for managing projects from initiation through release and continuous improvement.

## Quick Start

New to OctoAcme project management? Start here:

1. Read the [Project Management Overview](./octoacme-project-management-overview.md) to understand our principles, roles, and lifecycle
2. Explore the relevant process guide based on your project phase
3. Refer to [Personas](./octoacme-roles-and-personas.md) to understand team roles and responsibilities

## OctoAcme Project Management Overview

OctoAcme follows a structured **five-phase project lifecycle**: Initiation, Planning, Execution, Release, and Close & Retrospective. During **initiation**, teams validate business needs and create a lightweight Project One-pager that captures the problem statement, success metrics, and stakeholder alignment. This decision gate ensures teams move forward only when success criteria are clear and stakeholders agree on priority. 

Once approved, the **planning phase** transforms the approved initiative into an actionable backlog, breaking work into shippable increments with prioritization, estimation, and a Definition of Done. **Execution** follows a team rhythm of daily standups (15 min), weekly delivery syncs, and sprint-based delivery using GitHub Projects with standard columns (Backlog, Ready, In Progress, In Review, QA, Done). Pull requests are kept small (≤400 lines when possible) and require at least one approval before merging, with automated tests and linting running in CI before review.

OctoAcme defines three core delivery roles: **Project Managers** coordinate schedules, risks, and communications; **Product Managers** define outcomes and prioritize the backlog; and **Developers** implement features while maintaining tests and documentation. Each project has a named PM and Product Lead for clear ownership. Communication occurs through a regular cadence including weekly syncs between PM and Product Manager, twice-weekly standups for the delivery team, and monthly stakeholder updates, with ad-hoc escalation paths (Team-level → PM → Product Lead → Sponsor) for blockers and risks. Risk management is embedded throughout the lifecycle via a Risk Register that tracks identification, assessment, mitigation, and monitoring—reviewed weekly during syncs.

Quality is enforced at multiple gates: unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for feature acceptance when needed. The **release process** is standardized across three types (Patch, Minor, Major) with pre-release requirements including passing CI, security scans, drafted release notes, and a documented rollback plan. Before production deployment, teams run smoke tests in staging and post-deploy verifications to maintain observability. After each sprint, release, or incident, teams conduct **retrospectives** (45–75 min) to capture learnings, identify 2–3 actionable improvements, and track these improvements back into the project backlog with clear owners and timelines—creating a culture of continuous iterative enhancement grounded in data and psychological safety.

## Project Lifecycle Stages

### 1. Initiation
- **Document**: [Project Initiation Guide](./octoacme-project-initiation.md)
- **When**: Starting a new project or feature proposal
- **Key Output**: Project One-pager with problem, goals, and success metrics
- **Key Activities**: Validate business need, identify stakeholders, define success criteria, decide go/no-go

### 2. Planning
- **Document**: [Project Planning](./octoacme-project-planning.md)
- **When**: After project approval, before execution begins
- **Key Output**: Prioritized backlog, release timeline, Definition of Done
- **Key Activities**: Break work into increments, estimate scope, identify dependencies, create release plan

### 3. Execution & Tracking
- **Document**: [Execution & Tracking](./octoacme-execution-and-tracking.md)
- **When**: During active development and delivery
- **Key Output**: Daily standups, weekly syncs, progress dashboards
- **Key Activities**: Build, test, review, iterate; track velocity and burndown; escalate blockers

### 4. Release & Deployment
- **Document**: [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- **When**: Preparing to move features to production
- **Key Output**: Release notes, deployment checklist, rollback plan
- **Key Activities**: Pre-release validation, smoke testing, deployment, post-deploy verification

### 5. Retrospective & Continuous Improvement
- **Document**: [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- **When**: After sprint, release, or milestone completion
- **Key Output**: Learnings, action items, process improvements
- **Key Activities**: Capture what went well and what could improve, prioritize 2-3 action items, track improvements

## Cross-cutting Topics

- **Risk Management & Communication**: [Risk Management & Communication](./octoacme-risks-and-communication.md) — Identify, assess, mitigate, and monitor risks; manage stakeholder communication and escalation
- **Roles & Personas**: [Roles & Personas](./octoacme-roles-and-personas.md) — Understand core roles (Project Manager, Product Manager, Developer, QA) and their responsibilities

## Core Principles

OctoAcme operates on these principles:

- **Customer-first**: Prioritize customer value and usability
- **Iterative delivery**: Deliver small, testable increments
- **Clear ownership**: Each project has named PM and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback and learning

## Communication Cadence

- **Daily**: Team standups (15 min) — progress, blockers, dependencies
- **Twice-weekly**: Delivery team standups (or as agreed)
- **Weekly**: PM + Product Manager sync; Risk register review
- **Monthly**: Stakeholder updates
- **Ad-hoc**: Escalations for blockers and critical issues

## Key Artifacts

Across all phases, teams maintain:
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog with acceptance criteria
- Definition of Done
- Risk Register
- Retrospective notes and action items

## How to Use These Docs

- **Start here** if you're new to OctoAcme project management
- **Keep the Project Charter updated** in your project repo
- **Add process-specific docs** to `.copilot/` if you want Copilot Spaces to use them as context
- **Update process docs** using the [Add Content to Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template
