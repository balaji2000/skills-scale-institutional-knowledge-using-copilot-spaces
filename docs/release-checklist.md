# Release Checklist

Purpose: A concise release checklist to be referenced by the Release Manager and teams prior to deployment.

Pre-release (owner: Release Manager / PM)
- [ ] Confirm all PRs merged and acceptance criteria met
- [ ] CI checks passed (unit, integration, linting, security scans)
- [ ] Release notes drafted and communications prepared
- [ ] Stakeholders notified of release window
- [ ] Rollback and mitigation plan documented

Staging (owner: Release Manager / QA)
- [ ] Deploy to staging
- [ ] Run smoke tests and critical path checks
- [ ] Confirm telemetry and dashboards are reporting expected signals

Production (owner: Platform/SRE / Release Manager)
- [ ] Schedule deployment (automated pipeline preferred)
- [ ] Execute production deploy
- [ ] Run post-deploy verifications (smoke, metrics sanity checks)
- [ ] Notify stakeholders and support teams of completion

Post-release (owner: PM / PdM)
- [ ] Monitor success metrics for defined observation window
- [ ] Triage any regressions and assign follow-up items
- [ ] Capture release retrospective notes and actions

Rollback decision criteria
- Clearly call out which errors, thresholds, or customer-impact situations trigger rollback. Owner: Release Manager + Platform/SRE.

Link with the incident communication template (see docs/incident-communication-template.md) for escalation messaging.
