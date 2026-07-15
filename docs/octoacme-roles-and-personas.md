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

### Interactions with Other Roles
- **Product Managers**: Align on acceptance criteria and feature priorities
- **Project Managers**: Report progress and blockers; participate in planning
- **QA/Testing Lead**: Collaborate on test design; fix identified defects
- **Technical Lead**: Receive technical guidance and architecture feedback
- **DevOps/Release Engineer**: Coordinate on deployment requirements and CI/CD configuration

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

### Interactions with Other Roles
- **Project Managers**: Collaborate on timelines and milestone planning
- **Developers**: Discuss feasibility and technical trade-offs
- **Sponsor**: Align on strategic objectives and business priorities
- **Technical Lead**: Evaluate technical feasibility of features

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

### Interactions with Other Roles
- **Sponsor**: Escalate critical issues and seek go/no-go decisions
- **Product Managers**: Coordinate on priorities and timeline alignment
- **Developers**: Track progress and manage blockers
- **QA/Testing Lead**: Coordinate testing phases and quality gates
- **Scrum Master/Delivery Lead**: Collaborate on ceremony facilitation and process

---

## QA/Testing Lead

### Role Summary
QA/Testing Leads define and execute quality strategies, manage test planning, and ensure features meet acceptance criteria and quality standards before release.

### Responsibilities
- Define test plans and QA approaches during planning phase
- Create and maintain test cases aligned with acceptance criteria
- Execute manual and automated testing throughout delivery
- Identify quality risks and blockers
- Report quality metrics and test coverage to the team
- Approve features as meeting acceptance criteria before moving to Done
- Participate in release readiness reviews and smoke testing
- Mentor team on testing best practices and standards

### Goals
- Deliver high-quality, reliable features to production
- Catch defects early and reduce post-release issues
- Maintain clear visibility into quality status
- Build quality into the development process, not as an afterthought

### Typical Communication
- Sprint planning and backlog refinement
- Daily standups (blockers and test progress)
- QA sign-off in PR reviews and acceptance ceremonies
- Quality metrics in weekly status reports
- Post-release verification and incident triage

### Interactions with Other Roles
- **Developers**: Collaborate on test design; accept quality feedback; fix identified defects
- **Product Managers**: Align on acceptance criteria and quality expectations
- **Project Managers**: Report blockers and schedule time for testing phases
- **Sponsor**: Escalate critical quality issues affecting release readiness
- **DevOps/Release Engineer**: Execute smoke tests before/after deployment

---

## Technical Lead / Architect

### Role Summary
Technical Leads provide architectural guidance, make technical design decisions, and identify technical risks that could impact project success.

### Responsibilities
- Review and approve technical designs and architecture
- Identify technical risks and propose mitigations
- Make trade-off decisions on technology choices
- Mentor developers on technical best practices
- Ensure scalability, security, and maintainability of solutions
- Participate in code reviews for complex or risky changes
- Support capacity planning and technical estimating
- Champion technical excellence and reduce technical debt

### Goals
- Deliver scalable, maintainable, and secure technical solutions
- Reduce technical debt and architectural risks
- Enable team to deliver with high quality
- Foster a culture of technical excellence

### Typical Communication
- Technical design reviews and architecture discussions
- Sprint planning and estimation
- Code review feedback on complex changes
- Technical risk updates in project syncs
- One-on-ones with developers for mentoring

### Interactions with Other Roles
- **Developers**: Provide technical guidance and code review feedback
- **Project Managers**: Highlight technical risks and effort implications
- **Product Managers**: Discuss technical feasibility and trade-offs
- **DevOps/Release Engineer**: Coordinate on deployment and infrastructure needs
- **Security Lead**: Align on security architecture and design

---

## DevOps / Release Engineer

### Role Summary
DevOps and Release Engineers manage deployment pipelines, infrastructure, and ensure smooth, safe releases to production.

### Responsibilities
- Design and maintain CI/CD pipelines
- Manage deployment environments (staging, production)
- Execute deployments and verify production health
- Create and test rollback procedures
- Monitor post-deployment metrics and alerts
- Coordinate release schedules and communication
- Document deployment runbooks and incident playbooks
- Support incident response and hotfixes
- Ensure observability and logging throughout systems

### Goals
- Enable safe, frequent, and reliable releases
- Minimize deployment risk and time-to-recovery
- Maintain high availability and observability
- Automate repetitive deployment tasks

### Typical Communication
- Release planning and deployment windows
- Daily standup blockers related to deployments
- Post-release verification and monitoring
- Incident response and root cause analysis
- Infrastructure and capacity planning discussions

### Interactions with Other Roles
- **Developers**: Collaborate on CI/CD requirements and deployment readiness
- **Project Managers**: Coordinate release schedules and stakeholder communication
- **QA/Testing**: Execute smoke tests before/after deployment
- **Technical Lead**: Align on infrastructure and deployment architecture
- **Security Lead**: Implement security controls in CI/CD and deployment

---

## Security Lead

### Role Summary
Security Leads manage security reviews, ensure compliance, and respond to security incidents and vulnerabilities.

### Responsibilities
- Conduct security reviews of designs and code
- Manage security testing and vulnerability scanning
- Ensure compliance with security policies and standards
- Triage and manage security incidents
- Coordinate security incident response and communication
- Update security policies based on lessons learned
- Provide security training and awareness to the team
- Establish secure development practices and standards

### Goals
- Protect customer data and system security
- Reduce security vulnerabilities and incidents
- Maintain compliance and customer trust
- Enable developers to build secure solutions

### Typical Communication
- Security review gates during planning
- Code review comments on security-sensitive changes
- Vulnerability and incident response coordination
- Monthly security metrics and incident reviews
- Security awareness and training sessions

### Interactions with Other Roles
- **Developers**: Review code for security issues; provide guidance
- **Project Managers**: Escalate security incidents; coordinate response
- **DevOps/Release Engineer**: Ensure security controls in CI/CD and deployment
- **Sponsor**: Escalate critical security issues requiring executive attention
- **Technical Lead**: Align on security architecture and threat modeling

---

## Sponsor / Executive Stakeholder

### Role Summary
Sponsors provide business context, strategic direction, and executive oversight. They approve go/no-go decisions and escalate business-impacting issues.

### Responsibilities
- Define business objectives and success metrics
- Approve project charter and business case
- Make go/no-go decisions at key gates (initiation, planning, release)
- Escalate and resolve critical blockers affecting business outcomes
- Provide executive visibility to leadership and customers
- Remove organizational barriers to project success
- Approve scope or timeline changes
- Champion the project across the organization

### Goals
- Ensure projects deliver business value
- Maintain executive alignment and stakeholder confidence
- Resolve cross-functional conflicts and dependencies
- Enable successful project outcomes

### Typical Communication
- Project initiation and approval gates
- Monthly stakeholder updates
- Escalation calls for critical issues
- Release announcements and post-mortems
- Executive steering committee meetings

### Interactions with Other Roles
- **Project Managers**: Receive escalations and provide go/no-go decisions
- **Product Managers**: Align on strategic objectives and trade-offs
- **Developers/Teams**: Remove organizational or resource blockers
- **QA/Testing Lead**: Receive critical quality issue escalations
- **Security Lead**: Escalate critical security issues requiring executive attention

---

## Scrum Master / Delivery Lead

### Role Summary
Scrum Masters and Delivery Leads facilitate agile ceremonies, remove blockers, and coach the team on process adherence and continuous improvement.

### Responsibilities
- Facilitate daily standups, planning, reviews, and retrospectives
- Remove impediments and blockers for the team
- Coach team on agile principles and practices
- Maintain sprint/iteration board and backlog health
- Track team velocity and capacity
- Identify process improvements and facilitate implementation
- Support team communication and collaboration
- Shield team from external distractions

### Goals
- Enable team velocity and predictable delivery
- Foster psychological safety and continuous improvement
- Maintain process discipline and transparency
- Build a high-performing, self-organizing team

### Typical Communication
- Facilitation of all agile ceremonies
- Daily standup participation
- One-on-ones with team members
- Retrospective notes and action item tracking
- Process improvement recommendations

### Interactions with Other Roles
- **Project Managers**: Coordinate on process and timeline
- **Developers**: Facilitate ceremonies; remove blockers
- **Product Managers**: Support backlog refinement and prioritization
- **QA/Testing Lead**: Ensure testing activities are planned and tracked
- **All Roles**: Foster collaboration and remove communication barriers

---

## How these personas are used in the exercise

- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Reference the interaction patterns to understand cross-functional dependencies and communication flows.
- Use these personas to identify gaps in project processes and accountability.
