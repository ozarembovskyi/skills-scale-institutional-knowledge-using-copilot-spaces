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

## QA/Testing

### Role Summary
QA/Testing engineers validate that delivered software meets acceptance criteria and quality standards before it reaches production. They are a quality gate across the entire delivery lifecycle.

### Responsibilities
- Define and execute test plans, test cases, and regression suites
- Validate acceptance criteria on features and bug fixes
- Report, track, and retest defects to closure
- Participate in sprint planning and estimation to flag testability concerns
- Maintain and improve CI test coverage and automation

### Goals
- Prevent regressions and ensure high product quality
- Reduce the cost of defects by catching issues early
- Provide clear, reproducible bug reports

### Typical Communication
- Daily standups with the delivery team
- Defect reports and test summaries in the issue tracker
- QA sign-off comments on PRs and release tickets

### Interactions with Existing Roles
- **PM:** Receives task assignments and sprint priorities; reports blocking defects.
- **PdM:** Clarifies acceptance criteria and edge cases before test execution.
- **Developers:** Collaborates on reproducing bugs, reviewing testability, and agreeing on test coverage.
- **Release Manager:** Provides go/no-go signal based on test results before each release.
- **Stakeholders:** Surfaces quality metrics and critical outstanding issues in status updates.

---

## Stakeholders

### Role Summary
Stakeholders are individuals or groups with a vested interest in project outcomes. They include business sponsors, end users, and anyone whose input or approval shapes priorities or definitions of success.

### Responsibilities
- Provide clear requirements, priorities, and feedback
- Review and approve milestones, deliverables, or release content as needed
- Escalate business risks or blockers promptly
- Attend key ceremonies (kickoff, demos, retrospectives) when invited

### Goals
- Ensure the project delivers agreed-upon business value
- Maintain visibility into progress and risks
- Provide timely decisions when trade-offs arise

### Typical Communication
- Monthly or milestone-based status updates from PM
- Ad-hoc escalation emails or meetings for significant risks or decisions
- Demo invitations at end of sprint/milestone

### Interactions with Existing Roles
- **PM:** Primary point of contact for status, risks, and decisions.
- **PdM:** Collaborates on roadmap and feature prioritization.
- **Developers:** Limited direct interaction; typically routed through PM or PdM.
- **QA/Testing:** Receives quality/defect summaries that affect acceptance decisions.
- **Support/Customer Success:** Provides field insights that inform stakeholder priorities.

---

## Release Manager

### Role Summary
The Release Manager coordinates all release activities, ensures pre-release requirements are met, and acts as the central point of contact during deployment windows. They own the release process from readiness checks through post-deploy verification.

### Responsibilities
- Own the release calendar and communicate deployment windows
- Verify pre-release checklists are completed (CI green, release notes ready, rollback plan in place)
- Coordinate deployment activities with Developers and Ops/Infrastructure
- Facilitate the go/no-go decision with PM, PdM, and QA
- Manage stakeholder and support comms for the release
- Trigger and oversee rollback procedures when needed
- Conduct or schedule post-deploy verification and retrospective

### Goals
- Ship releases safely with minimal unplanned downtime
- Ensure every release has a tested rollback path
- Keep stakeholders and support informed throughout deployment

### Typical Communication
- Pre-release go/no-go meetings with PM, QA, and Tech Lead
- Release announcement emails/posts to stakeholders and Support
- Incident and rollback notifications via established channels

### Interactions with Existing Roles
- **PM:** Confirms timeline, scope, and stakeholder sign-off before release.
- **PdM:** Validates that release content matches the agreed roadmap increment.
- **Developers:** Coordinates code freeze, hotfix merges, and deployment execution.
- **QA/Testing:** Receives the go/no-go signal; ensures smoke tests pass pre- and post-deploy.
- **Stakeholders:** Sends release announcements and post-deploy status reports.

---

## UX Lead

### Role Summary
The UX Lead champions user experience throughout the project lifecycle. They ensure design and usability considerations are embedded in planning, development, and acceptance—not added as an afterthought.

### Responsibilities
- Define UX principles, patterns, and design standards for the project
- Partner with PdM to write usability-focused acceptance criteria
- Conduct or coordinate usability testing and incorporate findings
- Review designs and prototypes with Developers before implementation
- Participate in sprint reviews and demos to surface UX issues
- Maintain design artifacts (wireframes, prototypes, design system updates)

### Goals
- Deliver experiences that are intuitive, accessible, and consistent
- Reduce UX-related rework by catching issues early
- Build a shared design language across the team

### Typical Communication
- Backlog refinement sessions with PM and PdM
- Design review sessions with Developers before implementation
- Usability test summaries after testing rounds

### Interactions with Existing Roles
- **PM:** Flags UX risks and ensures design tasks are on the project plan.
- **PdM:** Co-authors acceptance criteria that include usability requirements.
- **Developers:** Shares wireframes and design specs; reviews implementation fidelity.
- **QA/Testing:** Defines usability test cases and participates in exploratory testing.
- **Stakeholders:** Presents design rationale and usability findings at key milestones.

---

## Support / Customer Success

### Role Summary
Support/Customer Success represents the voice of the customer and serves as the frontline for issues post-release. They close the loop between users in the field and the delivery team, ensuring real-world feedback informs future work.

### Responsibilities
- Monitor incoming customer feedback, bug reports, and support tickets
- Escalate critical or high-impact issues to PM and QA with clear reproduction steps
- Contribute customer insights and trend data to retrospectives and backlog refinement
- Maintain customer-facing communication during incidents and releases
- Ensure escalated field issues are entered as actionable backlog items

### Goals
- Minimize customer impact from defects and incidents
- Provide timely, clear communication to affected customers
- Translate field feedback into prioritized product improvements

### Typical Communication
- Regular feedback summaries (weekly or per sprint) shared with PM and PdM
- Incident status updates to customers via support channels
- Retrospective contribution on recurring customer pain points

### Interactions with Existing Roles
- **PM:** Escalates high-priority customer issues; provides field context for risk assessments.
- **PdM:** Shares customer feedback and usage patterns that inform roadmap priorities.
- **Developers:** Routes bug reports with reproduction steps; validates fixes from a customer perspective.
- **QA/Testing:** Collaborates on reproducing customer-reported issues and validating fixes.
- **Stakeholders:** Provides customer satisfaction signals and escalation visibility.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

