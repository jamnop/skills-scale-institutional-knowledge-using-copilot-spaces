---
title: "Release checklist (example)"
summary: "Example playbook showing the release checklist and ownership"
owners:
  - team: "platform"
  - contact: "@release-lead"
tags: ["release", "checklist", "example"]
created: 2025-12-01
review_date: 2026-06-01
status: stable
---

# Release checklist (example)

## Problem
Releases need a short, repeatable checklist so engineers and release leads can ship safely and predictably.

## Context / When to use
Use this checklist for any production release or canary deployment of OctoAcme services.

## Steps / Playbook
1. Create a release branch and open a PR with the release notes.
2. Verify CI: unit tests, integration smoke tests, and security scans pass.
3. Assign the PR to `@release-lead` and a QA reviewer.
4. Run the pre-release smoke test against staging.
5. Publish release notes and update the Project One-pager with the release version.
6. Deploy to production during the approved window and run post-deploy smoke tests.
7. Monitor for 30 minutes and follow rollback playbook if critical errors are found.

## Examples
- Pre-release checklist PR: link to a sample PR or release notes.

## Related
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)

## Change history
- 2025-12-01 — Created by Playbook seed
