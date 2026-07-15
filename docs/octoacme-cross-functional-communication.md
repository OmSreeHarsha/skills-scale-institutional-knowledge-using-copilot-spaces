# OctoAcme Cross-Functional Communication Guide

This guide establishes communication standards, escalation paths, and best practices for coordinating across the diverse roles in OctoAcme projects.

## Communication Standards

### Meeting Cadence

| Meeting | Frequency | Duration | Attendees | Purpose |
|---------|-----------|----------|-----------|----------|
| Daily Standup | Daily | 15 min | Developers, QA, DevOps, Scrum Master | Share progress, blockers, dependencies |
| Sprint Planning | Start of Sprint | 2-4 hours | All team members | Plan sprint work, estimate, identify risks |
| Sprint Review/Demo | End of Sprint | 1-2 hours | All team + Sponsor/PdM | Demonstrate completed work, get feedback |
| Sprint Retrospective | End of Sprint | 1-1.5 hours | All team members | Reflect on process, identify improvements |
| PM + PdM Sync | Weekly | 30 min | Project Manager, Product Manager | Align on priorities, risks, schedule |
| Technical Design Review | As-needed | 1 hour | Technical Lead, Developers, relevant leads | Review architectural approach, identify risks |
| Weekly Risk Review | Weekly | 30 min | Project Manager, relevant leads | Review risk register, identify escalations |
| Stakeholder Update | Weekly/Monthly | 30-60 min | Project Manager, Product Manager, Sponsor | Status update, decisions, issues |
| Security Review Gate | Per phase | 1-2 hours | Security Lead, Developers, Technical Lead | Approve security controls and mitigations |
| Release Coordination | Release window | 2-4 hours | Project Manager, DevOps, QA, Developers | Execute release, verify production health |

### Communication Channels

| Channel | Best For | Ground Rules |
|---------|----------|---------------|
| Synchronous (Meetings) | Decisions, complex discussions, alignment | Schedule in advance; come prepared; respect time |
| Asynchronous (Slack/Email) | Updates, announcements, questions | Tag relevant people; provide context; response time expectations |
| Project Board | Task tracking, work visibility | Keep updated; use labels consistently; link related issues |
| GitHub Issues | Problem tracking, decision logging | Link to relevant docs; provide acceptance criteria; close when resolved |
| Design Docs | Technical specifications, architectural decisions | Write before building; circulate for review; update as implementation evolves |
| Status Reports | Executive visibility, milestone tracking | Weekly or bi-weekly; consistent format; highlight risks |

---

## Escalation Paths

### Level 1: Team-Level Triage

**When**: Issue impacts immediate work
**Who**: Team member identifies → Scrum Master or Project Manager
**Action**: 
- Identify root cause
- Determine if it can be resolved within team
- Propose solution
- Document in blocker log

**Example Blockers**:
- Test environment unavailable
- Dependent team delayed
- Technical uncertainty
- Disagreement on approach

---

### Level 2: Cross-Functional Resolution

**When**: Issue requires input from multiple teams/roles
**Who**: Project Manager escalates → Product Manager, Technical Lead, relevant leads
**Action**:
- Schedule sync with all stakeholders
- Present problem statement and attempted solutions
- Discuss trade-offs and implications
- Make consensus decision or define next steps
- Document decision and rationale

**Example Issues**:
- Schedule vs. quality trade-off
- Technical feasibility vs. requirements
- Resource constraints vs. scope
- Security requirements vs. performance

---

### Level 3: Sponsor-Level Decision

**When**: Issue impacts business outcomes or requires executive judgment
**Who**: Project Manager escalates → Sponsor (with context from Product Manager, Technical Lead)
**Action**:
- Prepare escalation brief with:
  - Issue description
  - Business impact
  - Options considered
  - Recommendation with pros/cons
  - Decision timeline needed
- Present to Sponsor
- Document decision and communicate to team
- Update project plan and risk register

**Example Decisions**:
- Scope change
- Timeline/deadline change
- Budget increase
- Critical quality/security trade-off
- Resource reallocation
- Go/no-go decision

---

## Escalation Documentation Template

```
### Escalation: [Title]

**Date Escalated**: [Date]
**Escalated By**: [Role/Name]
**Escalation Level**: [1/2/3]
**Decision Owner**: [Role/Name]

#### Issue Summary
[Concise description of the problem]

#### Business Impact
[How does this affect the project? What are the consequences of inaction?]

#### Root Cause (if applicable)
[Why did this happen? What conditions led to this?]

#### Options Considered
1. [Option 1]
   - Pros: ...
   - Cons: ...
   - Effort: ...
2. [Option 2]
   - Pros: ...
   - Cons: ...
   - Effort: ...

#### Recommendation
[Which option is recommended and why?]

#### Timeline
[When is a decision needed? When would solution be implemented?]

#### Decision
[Final decision made and by whom]

#### Communication Plan
[Who needs to be informed? How and when will they be notified?]
```

---

## Risk Communication

### Risk Register Format

| ID | Description | Impact | Likelihood | Owner | Mitigation | Status | Next Review |
|----|-----------|----|-----------|-------|-----------|--------|-------------|
| R-001 | Dependency delayed | High | Medium | PM | Weekly check-in; identify alternatives | Active | Weekly |
| R-002 | Technical uncertainty | Medium | High | Tech Lead | Design review; spike investigation | Active | Bi-weekly |

### Risk Review Cadence
- **Weekly**: Review top risks, update status, identify escalations
- **Sprint Planning**: Add new risks identified, remove closed risks
- **Retrospective**: Analyze risks that materialized; improve risk management

### Risk Escalation Trigger
- **Probability x Impact > 8 (on scale of 1-10)**: Escalate to Level 2
- **Probability x Impact > 12**: Escalate to Level 3 (Sponsor)
- **Any security/compliance risk**: Always escalate to Security Lead and Sponsor if High impact

---

## Status Communication

### Weekly Status Template

**Project**: [Project Name]  
**Week of**: [Date]  
**Project Manager**: [Name]  

#### Progress This Week
- Completed: [List of delivered items]
- In Progress: [Current focus areas]
- Upcoming: [Next week priorities]

#### Metrics
- Velocity: [Story points or work items]
- Burn-down: [% of sprint complete]
- Quality: [Test coverage, bug count, etc.]
- Blockers: [Count and severity]

#### Key Risks & Issues
- **Risk 1**: [Description] - [Mitigation] - [Owner] - [Status]
- **Issue 1**: [Description] - [Action] - [Owner] - [Target Resolution Date]

#### Decisions Needed
- [Decision 1]: [Context] - [Options] - [Timeline]

#### Stakeholder Updates
- [What stakeholders need to know]

---

## Incident Communication

### Incident Response Notification

**Upon Detection** (within 15 min):
- Alert Sponsor, Project Manager, Product Manager
- Use escalation channel (Slack #incident or email)
- Include: "INCIDENT: [Brief Description] - [Team responding]"

**Initial Triage** (within 1 hour):
- Convene incident response team
- Assess impact and severity
- Assign incident lead and communication lead
- Determine timeline for resolution

**Regular Updates** (every 30 min or as impact changes):
- Share status on Slack
- Provide ETA for resolution
- Note: "Still investigating" or "Escalating"

**Resolution** (within hours of fix):
- Confirm fix in production
- Notify all stakeholders
- Schedule post-incident review

### Incident Severity Levels

| Level | Impact | Example | Response Time | Notify |
|-------|--------|---------|---|---|
| **Critical** | Customer-facing outage | Production down, data loss | 15 min | Sponsor, Exec |
| **High** | Significant degradation | Major feature broken | 30 min | Sponsor, Leads |
| **Medium** | Partial impact | Some users affected | 1 hour | PM, Leads |
| **Low** | Minor impact | Edge case issue | Next business day | Team |

---

## Communication Best Practices

### 1. Prepare for Meetings
- Share agenda 24 hours in advance
- Provide relevant context/docs
- Identify decision maker(s)
- Estimate time needed

### 2. Document Decisions
- Record what was decided and by whom
- Capture rationale and trade-offs
- Link to relevant issues/PRs
- Share decision with full team

### 3. Over-Communicate Status
- Assume stakeholders are busy
- Provide concise updates weekly
- Highlight changes from last week
- Always mention top risks

### 4. Use the Right Channel
- Announcements → Email + Slack
- Decisions → GitHub Issues + Email
- Urgent blockers → Direct communication
- Complex discussions → Meetings

### 5. Listen Actively
- Validate concerns before responding
- Ask clarifying questions
- Repeat back to confirm understanding
- Acknowledge different perspectives

### 6. Escalate Early
- Don't wait for problems to compound
- Escalate with solutions, not just problems
- Respect decision authority
- Document all escalations

### 7. Celebrate Wins
- Publicly acknowledge good work
- Share lessons learned
- Build team morale
- Reinforce team culture

---

## Handling Difficult Conversations

### Scope Creep
**Situation**: Stakeholder wants to add features mid-sprint
**Approach**:
1. Acknowledge the value of the request
2. Explain impact on timeline/quality
3. Offer to evaluate for next sprint
4. Document for retrospective

### Quality vs. Timeline
**Situation**: Team is behind, pressure to cut corners
**Approach**:
1. Present data on technical debt impact
2. Propose minimum acceptable quality level
3. Offer options (remove scope, extend timeline, add resources)
4. Let decision maker choose

### Disagreement Between Leads
**Situation**: Technical Lead and Product Manager disagree on approach
**Approach**:
1. Understand both perspectives fully
2. Identify core assumptions and trade-offs
3. Facilitate discussion with both parties
4. Make decision with input from Sponsor if needed
5. Commit to decision and move forward

### Missed Commitment
**Situation**: Team or dependency missed commitment
**Approach**:
1. Understand what happened (blameless)
2. Assess impact on project
3. Determine recovery plan
4. Adjust timeline/scope if needed
5. Update stakeholders
6. Capture lesson for retrospective
