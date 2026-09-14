---
name: go-no-go-coordinator
description: Make an evidence-backed release decision. Use when implementation is complete and the team needs a clear ship, hold, or limited-release recommendation.
---

# Go No Go Coordinator

## Outcome

A documented decision based on required checks, blocking defects, artifact verification, and known limitations.

## Inputs

- Release workbook, bug list, and artifact manifest
- Required checks and acceptable-risk criteria

## Workflow

1. Separate required checks from optional improvements.
2. Verify every required row has current evidence for the exact release artifact.
3. List unresolved defects by user impact and recovery availability.
4. Confirm privacy, data integrity, payment, installation, and authorization blockers are absent when applicable.
5. Choose ship, limited release, or hold and state the evidence behind it.

## Evidence gate

- Missing evidence is not a pass.
- Any unresolved data loss, cross-account access, secret exposure, or false payment state forces hold.

## Output

Complete the release-decision section with version, artifact, checks, blockers, limitations, owner, date, and recommendation.
