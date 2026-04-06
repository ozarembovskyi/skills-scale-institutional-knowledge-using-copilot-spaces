# OctoAcme — Release Manager Checklist

Use this checklist for every release to ensure readiness, safe deployment, and clear communication. Adapt as needed for patch, minor, or major releases.

---

## Pre-Release Readiness

- [ ] Release scope confirmed with PM and PdM (features, fixes, exclusions documented)
- [ ] All planned PRs merged; code freeze in effect for release branch
- [ ] CI pipeline green (tests, linting, security scans passing)
- [ ] Release notes drafted and reviewed
- [ ] Rollback / mitigation plan documented and shared with the team
- [ ] Deployment window scheduled and communicated to stakeholders and Support
- [ ] On-call coverage confirmed for the deployment window
- [ ] Smoke test plan prepared and shared with QA

## Go / No-Go Decision

Convene a short go/no-go check with PM, QA Lead, and Tech Lead before deploying:

- [ ] QA has signed off (all acceptance criteria met, no open P0/P1 defects)
- [ ] Release notes and customer communications ready to send
- [ ] Rollback steps tested or validated in staging
- [ ] Deployment tooling / pipeline confirmed operational
- [ ] **Go / No-Go decision recorded:** `[ ] Go` `[ ] No-Go` — Decision owner: ___________

## Deployment Execution

- [ ] Deploy to staging and run smoke tests — passed: `[ ] Yes` `[ ] No`
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Monitor error rates, latency, and key health signals for first 15–30 minutes
- [ ] Run post-deploy smoke tests — passed: `[ ] Yes` `[ ] No`

## Post-Deploy Verification

- [ ] Core user flows verified in production
- [ ] No spike in error rates or latency outside SLO thresholds
- [ ] Monitoring and alerting confirmed active for the new release
- [ ] Release announcement sent to stakeholders and Support

## Rollback Triggers

Initiate rollback immediately if any of the following occur:

- Error rate exceeds the defined SLO threshold for more than 5 minutes
- A critical (P0) customer-facing defect is introduced
- Data integrity issue detected
- Key integrations broken and no fast-fix available

**Rollback steps:**
1. Trigger rollback pipeline or redeploy last known-good release.
2. Notify PM, on-call, and Support immediately.
3. Open an incident ticket and assign a triage owner.
4. Communicate status update to stakeholders within 30 minutes.

## Post-Release Wrap-Up

- [ ] Post-deploy retrospective scheduled (for major releases or incidents)
- [ ] Outstanding issues logged as follow-up backlog items with priority
- [ ] Release record updated (date, version, scope, outcome)
- [ ] Lessons learned captured if a rollback or incident occurred

---

*See also: [Release & Deployment Guide](octoacme-release-and-deployment.md) | [Incident Communication Template](octoacme-incident-communication-template.md)*
