# OctoAcme — Release Manager Checklist

Use this checklist for every release to ensure readiness, clear communication, and a safe deployment. Adapt as needed for patch, minor, and major releases.

---

## 1. Pre-Release Readiness

- [ ] All features and fixes in scope are merged and code-complete
- [ ] Passing CI build (tests, lint, security scans)
- [ ] All acceptance criteria verified and QA sign-off received
- [ ] Release notes drafted and reviewed
- [ ] Migration steps (if any) documented and tested in staging
- [ ] Rollback plan documented (who, how, trigger criteria)
- [ ] Deployment window confirmed with PM and engineering lead
- [ ] On-call / support team notified of upcoming release

---

## 2. Go / No-Go Decision

Complete this section before opening the deployment window.

| Criteria | Status | Owner | Notes |
|---|---|---|---|
| QA sign-off | ☐ / ✅ | QA Lead | |
| Acceptance criteria complete | ☐ / ✅ | PdM | |
| No open P0/P1 bugs | ☐ / ✅ | QA Lead | |
| Rollback plan ready | ☐ / ✅ | Release Manager | |
| Stakeholders notified | ☐ / ✅ | PM | |
| Release notes approved | ☐ / ✅ | PdM | |

**Decision:** ☐ Go &nbsp;&nbsp; ☐ No-Go

**Decision owner:** _________________________

**Decision time (UTC):** _________________________

---

## 3. Deployment Communications

- [ ] Pre-deployment notice sent to stakeholders (include: what, when, expected downtime if any)
- [ ] Support/Customer Success team briefed on new features and known issues
- [ ] Internal #release or equivalent channel notified at deployment start

**Notification template:**
```
[Release Notice] <Release Name / Version>
Deploying: <Date & Time (UTC)>
Scope: <Brief summary of changes>
Expected impact: <None / Brief maintenance window X–Y UTC>
Rollback available: Yes
Questions: <Release Manager contact>
```

---

## 4. Deployment Execution

- [ ] Deployment to staging completed and smoke tests passing
- [ ] Production deployment initiated via automated pipeline (preferred)
- [ ] Deployment logs monitored for errors during rollout
- [ ] Feature flags toggled as planned (if applicable)
- [ ] Post-deploy smoke tests executed in production

---

## 5. Post-Deployment Verification

- [ ] Core user flows verified (smoke test checklist completed)
- [ ] Error rates and latency within normal thresholds (check dashboards)
- [ ] No new P0/P1 incidents opened within first 30 minutes
- [ ] Release announcement sent to stakeholders
- [ ] Support team handed off with release summary

**Verification window:** Monitor for at least **30 minutes** post-deployment before closing the release.

---

## 6. Rollback Triggers

Initiate a rollback immediately if any of the following occur:

- Error rate exceeds acceptable threshold (e.g., >1% 5xx errors sustained for 5 min)
- Core user flow is broken in production
- Data integrity issue detected
- P0 incident opened and no immediate hotfix available

**Rollback steps:**
1. Notify on-call engineer and PM
2. Trigger rollback via pipeline or manual deployment of last known-good release
3. Verify rollback by re-running smoke tests
4. Open incident and capture timeline (see [Incident Communication Template](octoacme-incident-communication-template.md))
5. Schedule blameless retrospective

---

## 7. Release Close-Out

- [ ] Release announcement published (changelog / release notes)
- [ ] Deployment log / summary added to project documentation
- [ ] Any post-deploy issues tracked in backlog
- [ ] Release retrospective scheduled (for major releases)

---

_See also: [Release & Deployment Guide](octoacme-release-and-deployment.md) | [Stakeholder Update Template](octoacme-stakeholder-update-template.md)_
