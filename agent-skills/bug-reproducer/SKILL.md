---
name: bug-reproducer
description: Turn a vague defect report into a deterministic reproduction and bounded fix request. Use whenever behavior is described as intermittent, broken, or inconsistent.
---

# Bug Reproducer

## Outcome

A minimal failing sequence that another person or agent can repeat.

## Inputs

- Original report, environment, and available evidence
- Relevant version or revision

## Workflow

1. Capture the exact starting state and environment.
2. Reduce the report to the shortest action sequence that still fails.
3. Record expected and actual results plus frequency.
4. Change one condition at a time to isolate the cause boundary.
5. After the fix, rerun the original sequence and one nearby regression check.

## Evidence gate

- The failure is reproduced before editing unless explicitly impossible.
- The passing result uses the same starting state and action sequence.

## Output

Write the completed bug template with severity, reproduction, evidence, cause, fix scope, and retest result.
