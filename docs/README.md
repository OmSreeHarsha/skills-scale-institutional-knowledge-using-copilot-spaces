# OctoAcme Project Management Documentation

Welcome to the OctoAcme Project Management Docs! This collection provides standardized guidance for running successful projects.

## Overview

OctoAcme uses a lightweight, iterative project management approach focused on delivering customer value through small, testable increments. Projects are anchored by concise artifacts — a Project One‑pager (charter), prioritized backlog, release plan, risk register, and retrospectives with action items — and follow a simple lifecycle: Initiation → Planning → Execution → Release → Close/Retrospective. Decision gates ensure readiness to progress, requiring clear success metrics, stakeholder alignment, and team availability.

Our team rhythm includes daily standups, weekly delivery syncs, sprint demos/reviews, and regular PM–PdM alignment meetings. Work is tracked on a project board (Backlog, Ready, In Progress, In Review, QA, Done). Pull Request practices emphasize small changes, linked issues and acceptance criteria, automated CI checks, and at least one reviewer approval before merging.

## Key Processes

- Initiation: Validate business need, create a project one‑pager, identify stakeholders, and capture initial risks.
- Planning: Prioritize backlog items, estimate scope, define the Definition of Done, and create release milestones.
- Execution & Tracking: Implement features, run unit/integration tests, perform reviews, and monitor progress via velocity and dashboards.
- Release & Deployment: Follow pre‑release checks, run staging smoke tests, deploy via automated pipelines, and execute post‑deploy verifications with rollback plans.
- Retrospective & Continuous Improvement: Run timeboxed retrospectives, record action items with owners and due dates, and incorporate improvements into the backlog.

## Personas & Roles

- Product Manager (PdM): Owns outcomes, prioritization, and success metrics.
- Project Manager (PM): Coordinates delivery, manages risks and communication, and facilitates ceremonies.
- Developers: Implement features, write tests and documentation, and participate in reviews.
- QA/Testing: Validate acceptance criteria and ensure quality through test suites and manual checks when needed.
- Stakeholders: Provide inputs and approvals.

## Quality & Testing

Quality is built into the workflow with requirements for unit tests, integration tests where applicable, end‑to‑end smoke tests for critical flows, and security scanning in CI. Manual QA is used as needed for feature acceptance. Releases require passing CI, drafted release notes, and a rollback/mitigation plan.

## Navigation

- Project Management Overview: octoacme-project-management-overview.md
- Project Initiation Guide: octoacme-project-initiation.md
- Project Planning: octoacme-project-planning.md
- Execution & Tracking: octoacme-execution-and-tracking.md
- Risk Management & Communication: octoacme-risks-and-communication.md
- Release & Deployment Guide: octoacme-release-and-deployment.md
- Retrospective & Continuous Improvement: octoacme-retrospective-and-continuous-improvement.md
- OctoAcme Personas: octoacme-roles-and-personas.md

## Quick Reference by Phase

- Starting a project → Project Initiation Guide
- Planning work → Project Planning
- Active development → Execution & Tracking
- Shipping → Release & Deployment Guide
- Reviewing learnings → Retrospective & Continuous Improvement

