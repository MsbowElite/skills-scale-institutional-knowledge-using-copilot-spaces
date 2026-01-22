# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (validated by DevOps and Security Lead)
- QA sign-off: all test plans executed and critical bugs resolved
- Release notes drafted (with input from Product, Support, and relevant stakeholders)
- Rollback / mitigation plan documented
- Smoke tests prepared
- Support team notified and prepared for release

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] QA approval received
- [ ] Security scan passed
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred, coordinated by DevOps)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders, support, and customers
- [ ] Monitor key metrics and dashboards (with Data Analyst support if applicable)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (DevOps, Security Lead as needed)
  - Rollback to last known-good release if necessary (coordinated by DevOps)
  - Notify Support/Customer Success of customer impact
  - Triage root cause and capture action items
  - Schedule post-incident review with relevant stakeholders

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
