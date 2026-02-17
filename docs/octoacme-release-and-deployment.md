# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (validated by Automation Specialist)
- Quality Assurance Lead sign-off on test completion and quality metrics
- Release notes drafted
- Change Manager approval for all changes in release
- Rollback / mitigation plan documented
- Smoke tests prepared and executed by Quality Assurance Lead

## Deployment Checklist
- [ ] Quality Assurance Lead confirms all tests passed and quality gates met
- [ ] Change Manager confirms all changes documented and approved
- [ ] Deployment window scheduled (if needed) and communicated by Stakeholder Liaison
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (coordinated by QA Lead)
- [ ] Deploy to production (automated pipeline managed by Automation Specialist)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support (led by Stakeholder Liaison)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
