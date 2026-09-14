---
name: clean-install-verifier
description: Verify installation and first launch from a clean or representative environment. Use before distributing a desktop, mobile, CLI, extension, or packaged web app.
---

# Clean Install Verifier

## Outcome

Evidence that the artifact a new user receives can be installed and opened without developer state.

## Inputs

- Final distributable artifact
- Supported operating systems, runtimes, or browsers
- Documented setup steps

## Workflow

1. Remove or isolate prior app state, caches, development credentials, and local services.
2. Follow only the user-facing installation instructions.
3. Launch the packaged artifact, not the development command.
4. Complete the first-run flow and record missing dependencies or permissions.
5. Repeat the failure path for unavailable network or denied permission when relevant.

## Evidence gate

- Artifact name, version, size, and checksum are recorded.
- First launch reaches the documented starting state without hidden developer setup.

## Output

Add a clean-install result to the release workbook with environment, steps, evidence, and blockers.
