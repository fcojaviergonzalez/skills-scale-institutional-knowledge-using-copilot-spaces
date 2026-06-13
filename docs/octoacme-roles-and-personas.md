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

## Additional Personas

The following roles address gaps in cross-team coordination, release reliability, observability, security, and user experience that are not fully covered by the core personas above. Adding these personas improves onboarding clarity, reduces handoff ambiguity, and surfaces clear ownership across the full project lifecycle.

---

### Technical Program Manager (TPM)

#### Role Summary
The Technical Program Manager coordinates cross-team technical dependencies, owns program-level timelines, and acts as the escalation path for technical blockers that span more than one team.

#### Responsibilities
- Track and communicate cross-team dependencies and integration milestones
- Facilitate alignment sessions between engineering leads and product leadership
- Own the program-level risk register and escalation log
- Maintain a shared roadmap across multiple workstreams

#### Goals
- Ensure inter-team dependencies are resolved before they block delivery
- Provide leadership with a clear, consolidated view of program status
- Reduce re-work caused by misaligned timelines or duplicate efforts

#### Typical Communication & Interactions
- Weekly syncs with Project Manager (PM), Tech Leads, and Release Engineer
- Program-level status reports to engineering and product leadership
- Dependency and integration reviews during planning cycles

---

### Tech Lead / Architect

#### Role Summary
The Tech Lead or Architect defines the high-level technical approach, drives architecture decisions, and mentors developers to maintain consistency and quality across the codebase.

#### Responsibilities
- Define and document architecture decisions (ADRs)
- Review high-impact designs for feasibility, scalability, and security
- Mentor developers and lead technical discussion in planning
- Partner with QA to identify testability risks early
- Evaluate trade-offs between speed, quality, and technical debt

#### Goals
- Maintain a coherent, sustainable architecture
- Reduce critical defects caused by design gaps
- Enable developers to work faster through clear technical standards

#### Typical Communication & Interactions
- Design review sessions with Developers and QA
- Feasibility trade-off discussions with Product Manager (PdM) and PM
- Dependency reviews with TPM
- Architecture decision records (ADRs) in the project repository

---

### Delivery Lead / Scrum Master

#### Role Summary
The Delivery Lead or Scrum Master facilitates team ceremonies, removes process impediments, and continuously improves team flow and delivery health.

#### Responsibilities
- Facilitate daily standups, sprint planning, reviews, and retrospectives
- Identify and remove blockers that slow the team
- Keep the backlog refined and prioritized in partnership with PM and PdM
- Track team velocity and flag risks to delivery commitments

#### Goals
- Maintain a predictable, sustainable team delivery cadence
- Create space for continuous improvement and psychological safety
- Reduce unplanned interruptions and context switching

#### Typical Communication & Interactions
- Daily standups with Developers
- Backlog grooming sessions with PM and PdM
- Retrospective facilitation with the full delivery team
- Escalation of systemic blockers to TPM or PM

---

### UX Researcher / Designer

#### Role Summary
The UX Researcher or Designer owns user research, interaction design, and accessibility validation. They ensure solutions are usable, accessible, and aligned with user needs before and after release.

#### Responsibilities
- Conduct user research, usability tests, and synthesis sessions
- Create wireframes, prototypes, and final design specifications
- Review acceptance criteria for usability and accessibility compliance
- Partner with Developers during implementation to validate fidelity

#### Goals
- Ensure features meet real user needs and accessibility standards
- Reduce post-release redesign by validating designs early
- Improve user satisfaction and adoption metrics

#### Typical Communication & Interactions
- Research and design reviews with PdM and Developers
- Accessibility review sessions with QA before release
- Usability findings shared via design docs and research summaries
- Prototype walkthroughs with stakeholders during planning

---

### Site Reliability Engineer (SRE) / On-call Owner

#### Role Summary
The SRE or On-call Owner defines reliability targets, owns runbooks, and coordinates post-deploy verification and incident response. They bridge development and production operations.

#### Responsibilities
- Define and track Service Level Objectives (SLOs) and error budgets
- Write and maintain operational runbooks and incident response playbooks
- Participate in release planning to assess production impact
- Lead incident response and post-incident reviews (post-mortems)
- Validate observability (logging, metrics, alerts) before deployment

#### Goals
- Maintain system reliability and meet SLO targets
- Reduce mean time to detection (MTTD) and mean time to recovery (MTTR)
- Improve deployment confidence through pre-release verification

#### Typical Communication & Interactions
- Release readiness reviews with Release Engineer and Developers
- Incident channels and escalation paths with on-call responders
- SLO review sessions with PdM and engineering leadership
- Runbook updates after each incident or significant deployment

---

### Release Engineer / DevOps

#### Role Summary
The Release Engineer or DevOps engineer owns CI/CD pipelines, release automation, rollback plans, and deployment validations. They are the primary coordinator of the technical release process.

#### Responsibilities
- Build and maintain CI/CD pipelines and deployment automation
- Own the deployment checklist and gate criteria for each release type
- Coordinate deployment windows with PM, SRE, and Developers
- Document and test rollback procedures before each release
- Track pipeline health and address flaky tests or build failures

#### Goals
- Achieve consistent, low-risk deployments through automation
- Enable developer self-service for routine deployments
- Maintain full rollback readiness for every release

#### Typical Communication & Interactions
- Deployment coordination with PM and SRE during release windows
- Pipeline status updates shared with Developers and Tech Lead
- Post-release verification sign-off with SRE
- Incident collaboration with SRE when deployments cause production issues

---

### Data Analyst / Measurement Owner

#### Role Summary
The Data Analyst or Measurement Owner defines required metrics, builds and maintains dashboards, and validates that success metrics are measurable and tracked after release.

#### Responsibilities
- Partner with PdM to define feature success metrics before development starts
- Instrument tracking requirements and review implementation with Developers
- Build and maintain dashboards for release and post-release monitoring
- Conduct post-release analysis and share findings with the team

#### Goals
- Ensure every feature ships with measurable outcomes
- Reduce time to insight after release through automated dashboards
- Support data-driven prioritization and retrospective discussions

#### Typical Communication & Interactions
- Metric definition sessions with PdM during planning
- Instrumentation reviews with Developers
- Post-release dashboards and reports shared with PM and stakeholders
- Retrospective data summaries to inform team decisions

---

### Security & Compliance Liaison

#### Role Summary
The Security & Compliance Liaison reviews changes for security and compliance impact, coordinates security scans, and records required approvals. They ensure the team ships securely without introducing unnecessary process friction.

#### Responsibilities
- Review significant design and architecture changes for security risk
- Coordinate automated and manual security scanning in CI/CD
- Maintain a log of compliance approvals and security review decisions
- Advise the team on secure coding practices and data-handling requirements
- Participate in incident response when security issues are discovered

#### Goals
- Prevent security vulnerabilities from reaching production
- Meet compliance requirements without blocking delivery
- Build security awareness across the development team

#### Typical Communication & Interactions
- Design reviews with Tech Lead and Developers for high-risk changes
- Pre-release security sign-off with Release Engineer and SRE
- Compliance approval records shared with PM and stakeholders
- Incident response coordination with SRE when security incidents occur

---

## Why these additional personas matter

Explicitly defining these roles improves OctoAcme project outcomes in the following ways:

- **Onboarding clarity**: New team members can see who owns what, who to contact for specific concerns, and what each role contributes across the lifecycle.
- **Reduced handoff ambiguity**: Clear role boundaries and interaction descriptions reduce repeated clarifying questions and missed handoffs between planning, delivery, and release.
- **Release reliability**: Naming the SRE and Release Engineer responsibilities for runbooks, deployment gates, and post-deploy verification reduces the risk of undocumented production changes.
- **Cross-team coordination**: The TPM role provides a single coordination point for multi-team dependencies, reducing the risk of schedule conflicts and integration failures.
- **Accountability for outcomes**: The Data Analyst / Measurement Owner role ensures success metrics are defined and tracked, not left as an afterthought.
- **Security by design**: The Security & Compliance Liaison keeps security reviews embedded in the delivery process rather than bolted on at release.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

