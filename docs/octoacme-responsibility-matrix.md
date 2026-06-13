# OctoAcme Responsibility Matrix (RACI)

## Purpose
Map key lifecycle activities to the roles and personas defined in [`octoacme-roles-and-personas.md`](./octoacme-roles-and-personas.md). Use this matrix to quickly identify who is **Responsible**, **Accountable**, **Consulted**, or **Informed** for each activity.

**Legend**
| Code | Meaning |
|------|---------|
| **R** | Responsible — does the work |
| **A** | Accountable — owns the outcome and signs off |
| **C** | Consulted — provides input; two-way communication |
| **I** | Informed — receives updates; one-way communication |

---

## Matrix

| Activity | PM | PdM | Dev | QA | Delivery Lead | Tech Lead | TPM | UX | SRE | Release Eng | Data Analyst | Security Liaison |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Initiation** |  |  |  |  |  |  |  |  |  |  |  |  |
| Draft project charter | R/A | C | I | I | I | C | C | I | I | I | I | I |
| Define success metrics | C | R/A | I | I | I | C | I | C | I | I | C | I |
| Stakeholder identification | R | C | I | I | I | I | C | I | I | I | I | I |
| Go/no-go decision | A | C | I | I | I | C | C | I | I | I | I | C |
| **Planning** |  |  |  |  |  |  |  |  |  |  |  |  |
| Backlog refinement and estimation | C | R | R | C | R | C | I | C | I | I | I | I |
| Architecture and design review | I | C | C | C | I | R/A | C | I | C | I | I | C |
| UX research and prototyping | I | C | C | I | I | C | I | R/A | I | I | I | I |
| Risk register creation | R/A | C | C | C | C | C | C | I | C | C | I | C |
| Dependency mapping | C | C | C | I | C | I | R/A | I | C | C | I | I |
| Instrumentation planning | I | C | C | I | I | C | I | I | C | I | R/A | I |
| Security review of design | I | I | C | I | I | C | I | I | C | I | I | R/A |
| **Execution & Tracking** |  |  |  |  |  |  |  |  |  |  |  |  |
| Daily delivery (feature work) | I | I | R/A | C | C | C | I | C | I | I | I | I |
| Sprint facilitation | C | C | I | I | R/A | I | I | I | I | I | I | I |
| Blocker removal | C | C | C | I | R | C | C | I | I | I | I | I |
| Code and design review | I | I | R | R | I | R/A | I | C | I | I | I | I |
| Status reporting | R/A | C | I | I | C | I | C | I | I | I | I | I |
| Cross-team dependency coordination | C | C | I | I | I | C | R/A | I | I | I | I | I |
| **Release & Deployment** |  |  |  |  |  |  |  |  |  |  |  |  |
| Release readiness sign-off | A | C | C | C | I | C | I | I | C | R | I | C |
| CI/CD pipeline management | I | I | C | I | I | C | I | I | C | R/A | I | C |
| Deployment execution | I | I | C | I | I | I | I | I | C | R/A | I | I |
| Post-deploy verification | I | I | C | C | I | C | I | I | R/A | C | I | I |
| Rollback decision | A | I | C | I | I | C | I | I | R | C | I | I |
| Release notes | R | C | C | I | I | I | I | I | I | C | I | I |
| Security scan approval | I | I | I | I | I | I | I | I | C | C | I | R/A |
| **Incidents** |  |  |  |  |  |  |  |  |  |  |  |  |
| Incident response lead | I | I | C | I | I | C | I | I | R/A | C | I | C |
| Root cause analysis | C | I | C | C | I | C | I | I | R | C | I | C |
| Incident communication | R | I | I | I | I | I | C | I | C | I | I | I |
| Action item tracking | R/A | I | C | I | C | C | C | I | C | C | I | C |
| **Retrospective** |  |  |  |  |  |  |  |  |  |  |  |  |
| Retrospective facilitation | C | C | C | C | R/A | I | I | I | I | I | I | I |
| Metrics review and trend analysis | C | C | I | I | I | I | I | I | C | I | R/A | I |
| Action item ownership | A | C | C | C | C | C | C | I | C | C | C | C |
| Documentation update | R/A | C | C | I | C | C | C | I | I | I | I | I |

---

## Notes
- A single cell may show **R/A** when the same role is both responsible and accountable (common for specialist-owned tasks).
- When a role is not involved in an activity, the cell is left blank.
- This matrix is a guide, not a rigid rule. Teams should adapt ownership based on project context and team size.
- For small teams, roles may be combined; for larger programs, dedicated individuals fill each role.

## Related docs
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [Role Handoff Checklist](./octoacme-role-handoff-checklist.md)
- [Project Management Overview](./octoacme-project-management-overview.md)
