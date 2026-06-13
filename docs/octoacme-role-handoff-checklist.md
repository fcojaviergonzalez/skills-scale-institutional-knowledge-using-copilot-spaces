# OctoAcme Role Handoff & Participation Checklist

## Purpose
Clarify which roles participate in key project lifecycle moments and what each role is expected to contribute or hand off. Use this checklist alongside the [Responsibility Matrix](./octoacme-responsibility-matrix.md) to reduce coordination gaps at phase boundaries.

---

## 1. Project Initiation Handoff

**Trigger:** Project charter approved; moving from ideation to planning.

| Role | Required action |
|------|----------------|
| Project Manager | Share approved charter and initial timeline; schedule kickoff meeting |
| Product Manager | Confirm problem statement, success metrics, and backlog seed |
| Tech Lead / Architect | Provide initial feasibility assessment and flag major technical unknowns |
| Technical Program Manager | Identify cross-team dependencies; confirm availability of shared resources |
| Security & Compliance Liaison | Flag any known compliance or data-handling requirements |
| UX Researcher / Designer | Confirm whether user research is needed before design begins |
| Data Analyst / Measurement Owner | Agree on metric instrumentation requirements at kickoff |

**Handoff artifact:** Completed project charter and dependency log shared with all roles above.

---

## 2. Planning Participation Checklist

**Trigger:** Sprint/iteration planning or release planning session.

- [ ] **Project Manager** — facilitates session; confirms scope and milestones
- [ ] **Product Manager** — presents prioritized backlog; clarifies acceptance criteria
- [ ] **Delivery Lead / Scrum Master** — ensures backlog is refined before session; tracks capacity
- [ ] **Tech Lead / Architect** — reviews technical estimates; flags design risks
- [ ] **UX Researcher / Designer** — confirms design assets are ready for stories in scope
- [ ] **Data Analyst / Measurement Owner** — confirms tracking requirements are included in stories
- [ ] **Security & Compliance Liaison** — flags any stories with security implications
- [ ] **Technical Program Manager** — raises cross-team dependencies that affect the sprint

**Output:** Committed sprint/iteration plan with clear acceptance criteria and Definition of Done.

---

## 3. Pre-release Participation Checklist

**Trigger:** Feature complete; preparing for deployment.

- [ ] **Project Manager** — confirms release notes drafted and stakeholders notified
- [ ] **Product Manager** — verifies all acceptance criteria met; approves release content
- [ ] **QA / Testing** — confirms all tests passing; sign-off on acceptance criteria
- [ ] **Tech Lead / Architect** — reviews any last-minute architecture concerns
- [ ] **Release Engineer / DevOps** — confirms CI/CD pipeline passing; deployment checklist ready; rollback plan documented
- [ ] **SRE / On-call Owner** — confirms observability (logs, metrics, alerts) in place; runbook updated
- [ ] **Security & Compliance Liaison** — confirms security scans passed; compliance approvals recorded
- [ ] **Data Analyst / Measurement Owner** — confirms dashboards and tracking are ready for post-release monitoring
- [ ] **Technical Program Manager** — confirms all cross-team dependencies resolved

**Handoff artifact:** Release readiness sign-off (can be a checklist comment in the release PR or issue).

---

## 4. Post-deploy Verification Checklist

**Trigger:** Deployment to production complete.

- [ ] **Release Engineer / DevOps** — confirms deployment completed without errors
- [ ] **SRE / On-call Owner** — runs post-deploy verification; confirms error rates within SLO
- [ ] **QA / Testing** — validates smoke tests pass in production
- [ ] **Data Analyst / Measurement Owner** — confirms tracking is firing correctly in production
- [ ] **Project Manager** — sends release announcement to stakeholders
- [ ] **Product Manager** — notifies customer-facing teams and support

**Handoff artifact:** Post-deploy verification comment in the release record; monitoring link shared in team channel.

---

## 5. Incident Response Participation

**Trigger:** Production incident declared (page/alert fired).

| Phase | Roles involved | Action |
|-------|---------------|--------|
| Detection | SRE / On-call Owner | Acknowledge alert; assess severity |
| Initial response | SRE, Release Engineer | Begin triage; decide whether to rollback |
| Communication | Project Manager | Notify stakeholders and leadership per severity level |
| Technical triage | SRE, Tech Lead, Developers | Identify root cause |
| Security check | Security & Compliance Liaison | Assess whether incident has security or compliance implications |
| Resolution | Release Engineer, SRE | Deploy fix or rollback; confirm system stable |
| Post-incident review | SRE, Tech Lead, PM, PdM | Write post-mortem; assign action items |

**Handoff artifact:** Post-mortem document with timeline, root cause, and action items. Action items tracked in the project backlog.

---

## 6. Retrospective Participation

**Trigger:** End of sprint, milestone, release, or incident.

- [ ] **Delivery Lead / Scrum Master** — facilitates the session; ensures psychological safety
- [ ] **All delivery team members** — contribute to what went well, what to improve, action items
- [ ] **Project Manager** — tracks action items to completion; updates process docs if needed
- [ ] **Data Analyst / Measurement Owner** — presents metrics trend (velocity, defect rate, etc.)
- [ ] **SRE / On-call Owner** — shares reliability and incident trends for release retros
- [ ] **Product Manager** — shares customer feedback and outcome metrics

**Output:** 3–5 prioritized action items with named owners and target dates. Action items added to the project backlog.

---

## Related docs
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [Responsibility Matrix](./octoacme-responsibility-matrix.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
