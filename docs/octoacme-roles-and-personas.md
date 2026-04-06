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

---

## QA / Testing

### Role Summary
QA/Testing engineers validate that features meet acceptance criteria and quality standards before release. They design test plans, execute manual and automated tests, and serve as the last quality gate before deployment.

### Responsibilities
- Design and maintain test plans and test cases
- Execute manual, automated, integration, and regression tests
- Raise and track defects with clear reproduction steps
- Verify bug fixes and validate acceptance criteria
- Participate in sprint planning to surface testability concerns early

### Goals
- Prevent regressions and maintain production stability
- Provide fast, clear feedback to developers on quality issues
- Continuously improve test coverage and automation

### Typical Communication
- Daily standups and sprint planning
- Bug reports and test summary reports
- Pre-release sign-off confirmations

### Interactions
- **PM**: Receives sprint scope and timelines; flags risks that could affect test readiness.
- **PdM**: Clarifies acceptance criteria and edge cases for user-facing features.
- **Developers**: Works closely to reproduce issues, verify fixes, and align on test automation strategy.
- **Release Manager**: Provides go/no-go input based on test results before deployment.
- **Stakeholders**: Communicates quality status and known issues via PM at milestone reviews.

---

## Stakeholders

### Role Summary
Stakeholders are individuals or groups with a vested interest in project outcomes. They provide requirements and context, approve key decisions, and are kept informed throughout the project lifecycle.

### Responsibilities
- Provide business context, requirements, and success criteria
- Review and approve key milestones, scope changes, and release decisions
- Escalate blockers or priority shifts that affect delivery
- Participate in demos and milestone reviews

### Goals
- Ensure the project delivers business value and meets their needs
- Maintain visibility into project status and risks
- Minimize surprises at delivery

### Typical Communication
- Monthly or milestone-based status updates from PM
- Participation in major demos and reviews
- Ad-hoc escalation responses when decisions are needed

### Interactions
- **PM**: Primary communication channel for status, risks, and decision requests.
- **PdM**: Collaborates on prioritization, feature trade-offs, and success metrics.
- **Developers**: Occasional direct exposure during demos and sprint reviews.
- **QA/Testing**: Informed of quality status and known issues at release time.
- **Release Manager**: Notified of release schedules and go/no-go outcomes.

---

## Release Manager

### Role Summary
The Release Manager coordinates all release activities, ensures pre-release requirements are met, and is the central point of contact during deployment windows. They manage release schedules, communication, and post-deployment validation.

### Responsibilities
- Coordinate and schedule release windows with all stakeholders
- Verify pre-release checklists and go/no-go criteria are met
- Manage deployment communication and notify relevant parties
- Oversee post-deployment verification and monitor for issues
- Coordinate rollback decisions if critical issues arise
- Maintain release notes and post-deployment summaries

### Goals
- Enable smooth, low-risk releases
- Minimize downtime and production incidents during deployments
- Ensure clear communication before, during, and after each release

### Typical Communication
- Pre-release notifications and go/no-go announcements
- Deployment status updates during release windows
- Post-deployment verification summaries

### Interactions
- **PM**: Aligns on release timing, scope, and communications plan.
- **PdM**: Confirms feature readiness and acceptance criteria completion.
- **Developers**: Coordinates deployment steps, hotfix preparation, and rollback readiness.
- **QA/Testing**: Relies on QA sign-off for go/no-go decisions; coordinates smoke tests.
- **Stakeholders**: Sends release announcements and notifies of any delays or issues.

> See also: [Release Manager Checklist](octoacme-release-manager-checklist.md)

---

## UX Lead

### Role Summary
The UX Lead maintains focus on user experience throughout the project lifecycle. They champion usability, partner with Product and QA on acceptance criteria, and surface UX issues early to reduce rework.

### Responsibilities
- Define and maintain UX standards, design guidelines, and patterns
- Participate in backlog refinement to surface UX requirements and acceptance criteria
- Conduct or coordinate usability testing and user research
- Review designs and prototypes with PdM and Developers
- Participate in sprint demos to identify UX issues before release

### Goals
- Ensure the product is intuitive, accessible, and consistent
- Reduce costly UX-related rework by involving UX early in the delivery cycle
- Build a shared UX vocabulary and design library across the team

### Typical Communication
- Design reviews and backlog refinement sessions
- Usability test results and design feedback
- UX sign-off as part of feature acceptance

### Interactions
- **PM**: Surfaces UX risks or capacity constraints that may affect sprint timelines.
- **PdM**: Collaborates on feature definition, acceptance criteria, and user research priorities.
- **Developers**: Provides design guidance, reviews implementations, and aligns on feasibility.
- **QA/Testing**: Partners on usability test planning and shares UX-related acceptance criteria.
- **Stakeholders**: Presents user research findings and design rationale at milestone reviews.

---

## Support / Customer Success

### Role Summary
Support/Customer Success acts as the voice of the customer and the frontline for post-release issues. They monitor user feedback, collaborate on incident response, and ensure field issues are captured and prioritized for resolution.

### Responsibilities
- Monitor incoming support requests and surface patterns to the delivery team
- Document field issues with clear reproduction steps for backlog entry
- Collaborate with PM and QA during incident triage and response
- Provide customer impact summaries at retrospectives
- Communicate resolution timelines and workarounds to affected customers

### Goals
- Minimize customer impact from bugs and incidents
- Close the feedback loop between customers and the delivery team
- Reduce time-to-resolution for customer-facing issues

### Typical Communication
- Incident escalation notifications and status updates
- Weekly feedback summaries to PM and PdM
- Post-incident customer communications

### Interactions
- **PM**: Escalates high-priority customer issues and provides field feedback for prioritization.
- **PdM**: Shares aggregated customer feedback to inform roadmap and backlog decisions.
- **Developers**: Coordinates on issue reproduction, patches, and workaround guidance.
- **QA/Testing**: Collaborates during incident triage to reproduce and verify fixes.
- **Stakeholders**: Communicates customer impact and resolution status during incidents.

> See also: [Incident Communication Template](octoacme-incident-communication-template.md)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

