# OctoAcme — Incident Communication Template

Use this template when a production incident is declared. Fill in each section as information becomes available. Update stakeholders at the cadence defined below until the incident is resolved.

Aligns with the escalation paths in [Risk Management & Communication](octoacme-risks-and-communication.md).

---

## Incident Declaration

**Incident ID / Name:** INC-_________  (_short description_)
**Severity:** P0 — Critical / P1 — High / P2 — Medium
**Declared by:** _________________________
**Declared at (UTC):** _________________________
**Incident Commander:** _________________________
**Communication lead:** _________________________  (PM or Release Manager)

---

## Triage Summary

_Complete within 15 minutes of declaration. Update as information evolves._

**What is happening?**
_Brief description of the observed impact — what is broken, who is affected._

**Customer / business impact:**
_Estimated number of users affected, key workflows broken, revenue/SLA impact._

**Current status:**
☐ Investigating &nbsp; ☐ Identified &nbsp; ☐ Mitigating &nbsp; ☐ Monitoring &nbsp; ☐ Resolved

**Timeline so far:**

| Time (UTC) | Event |
|---|---|
| | Incident declared |
| | |
| | |

---

## Actions Being Taken

_List active investigation and mitigation steps with owners._

| Action | Owner | Status | ETA |
|---|---|---|---|
| | | | |
| | | | |

---

## Estimated Timeline to Resolution

**Current ETA (UTC):** _________________________
**Basis for estimate:** _________________________
**Confidence:** Low / Medium / High

_Update this section at every communication cycle._

---

## Communications Cadence

| Audience | Channel | Frequency | Owner |
|---|---|---|---|
| Engineering / On-call | Incident channel (Slack/Teams) | Continuous | Incident Commander |
| PM / PdM | Direct message or war room | Every 30 min | Incident Commander |
| Stakeholders | Email / status page | Every 60 min or at major change | PM / Comm Lead |
| Customers (if external) | Status page / email | At declaration, update, resolution | PM / Support |

**Standard stakeholder update message:**

```
[Incident Update] INC-<ID> — <Short description>
Time (UTC): <current time>
Status: <Investigating / Mitigating / Resolved>
Impact: <Who is affected and how>
Actions: <What the team is doing>
ETA: <Expected resolution time>
Next update: <Time of next update>
Contact: <Incident Commander or PM>
```

---

## Resolution & All-Clear

**Resolved at (UTC):** _________________________
**Root cause (preliminary):** _________________________
**Fix applied:** _________________________

**All-clear communication sent:** ☐ Yes &nbsp; Date/Time: _________________________

**All-clear message template:**
```
[Resolved] INC-<ID> — <Short description>
Resolved at: <UTC time>
Duration: <X hours Y minutes>
Impact summary: <Brief description of affected users/services>
Root cause: <Preliminary root cause>
Follow-up actions: <Link to post-incident retro or ticket>
```

---

## Post-Incident Retrospective

Schedule within **5 business days** of resolution. This is a blameless retrospective focused on learning and improvement.

**Retro date/time:** _________________________
**Facilitator:** _________________________
**Required attendees:** Incident Commander, PM, affected engineers, QA, Support

### Retro Agenda

1. **Timeline review** — walk through the incident timeline together (30 min)
2. **What went well** — things that helped detect or resolve the incident faster
3. **What went wrong** — contributing factors and gaps
4. **Action items** — concrete improvements with owners and due dates

### Action Items

| # | Description | Owner | Due Date | Status |
|---|---|---|---|---|
| | | | | |
| | | | | |

---

_See also: [Risk Management & Communication](octoacme-risks-and-communication.md) | [Release Manager Checklist](octoacme-release-manager-checklist.md) | [Stakeholder Update Template](octoacme-stakeholder-update-template.md)_
