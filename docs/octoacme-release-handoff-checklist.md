# OctoAcme — Release Handoff Checklist

Use this checklist before every release to confirm all roles have completed their pre-release responsibilities. Each owner must explicitly sign off before the Release Manager approves deployment.

---

## 1. Product Manager Sign-off

- [ ] All acceptance criteria for in-scope stories are met and verified
- [ ] Release notes drafted and reviewed for accuracy
- [ ] Any out-of-scope items or known limitations are documented and communicated
- [ ] Product stakeholders have been notified of the upcoming release date and contents

## 2. Project Manager Sign-off

- [ ] Release window is scheduled and communicated to all teams
- [ ] No open blocking risks or unresolved dependencies remain
- [ ] Project tracking board reflects the correct release state
- [ ] Post-release retro is scheduled (if applicable)

## 3. Developer Sign-off

- [ ] All feature PRs are merged to the release branch
- [ ] CI pipeline is green (build, unit tests, integration tests)
- [ ] No known critical or high-severity defects in the release scope
- [ ] Rollback scripts or procedures are prepared and documented
- [ ] Deployment runbook is up to date

## 4. QA Automation Specialist Sign-off

- [ ] Automated regression suite passes with no new failures
- [ ] Smoke test scenarios covering key user flows are ready
- [ ] Test coverage meets or exceeds the agreed threshold for this release
- [ ] Any known flaky tests have been triaged and are not masking real failures

## 5. Release Manager Sign-off

- [ ] All above sign-offs are received
- [ ] Deployment window is confirmed with infrastructure/ops (if applicable)
- [ ] Staging deployment completed and verified
- [ ] Rollback plan is documented and accessible to the on-call team
- [ ] Post-deploy verification steps are defined and assigned
- [ ] Release announcement template is prepared

---

## Post-Release Verification

After deployment, the Release Manager should confirm:

- [ ] Production smoke tests pass
- [ ] Key metrics (error rates, latency) are within normal ranges
- [ ] Stakeholders and support team have been notified of the release
- [ ] Release notes are published

---

## References

- [Roles & Personas](./octoacme-roles-and-personas.md) — see Release Manager and QA Automation Specialist
- [Release & Deployment Guide](./octoacme-release-and-deployment.md) — full deployment checklist and rollback playbook
