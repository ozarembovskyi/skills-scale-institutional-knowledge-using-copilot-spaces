# OctoAcme — Incident Communication Template

Use this template to structure clear, timely communication during and after an incident. Adapt for severity and audience.

---

## Incident: [Short Title] | [Date & Time]

**Severity:** P0 — Critical / P1 — High / P2 — Medium
**Incident Commander:** [Name]
**Status:** 🔴 Active / 🟡 Monitoring / 🟢 Resolved

---

## Triage Summary

**What happened:**
> [1–2 sentence description of the issue and its customer/business impact.]

**Affected systems / services:**
> [List impacted services, features, or user groups.]

**Detection time:** [Time incident was first detected]
**Declaration time:** [Time incident was formally declared]
**Estimated customer impact:** [Number of users affected or % of traffic impacted, if known]

---

## Actions Being Taken

| # | Action | Owner | Status | ETA |
|---|--------|-------|--------|-----|
| 1 | [Immediate mitigation step] | [Name] | In Progress | [Time] |
| 2 | [Investigation step] | [Name] | Pending | [Time] |
| 3 | [Rollback if triggered] | [Name] | — | [Time] |

---

## Communication Cadence

| Audience | Channel | Frequency |
|----------|---------|-----------|
| Internal team | Incident channel / War room | Continuous |
| PM & Leadership | Direct message / Email | Every 30 min while active |
| Stakeholders | Email / Status page | On declaration, on resolution |
| Customers (if applicable) | Status page / In-app banner | On declaration, on resolution |

**Next update due:** [Time]

---

## Resolution

**Time resolved:** [Time]
**Root cause (preliminary):** [Brief description]
**Fix applied:** [What was done — rollback, hotfix, config change, etc.]
**Monitoring:** [What is being watched to confirm stability]

---

## Post-Incident Retrospective

**Retrospective scheduled:** [Date/Time]
**Facilitator:** [Name]

Retro agenda:
1. Timeline walkthrough — what happened and when
2. Root cause analysis (5 Whys or equivalent)
3. What went well
4. What can be improved
5. Action items with owners and due dates

| Action Item | Owner | Due Date | Status |
|-------------|-------|----------|--------|
| [Follow-up action] | [Name] | [Date] | Open |

---

*See also: [Risk Management & Communication](octoacme-risks-and-communication.md) | [Release Manager Checklist](octoacme-release-manager-checklist.md)*
