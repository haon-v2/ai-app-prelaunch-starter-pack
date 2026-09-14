# Try this first: prove a clean install

The fastest way to judge this pack is to use one complete skill on an app you already have.

Copy the prompt below into Codex, Claude Code, Cursor, Windsurf, ChatGPT, or another coding agent that can inspect your project.

```text
Read agent-skills/clean-install-verifier/SKILL.md and follow it for the exact app build I would give a new user.

Before changing anything:
1. identify the artifact or command a new user would receive;
2. list any developer-only state that could make the app appear to work;
3. state the clean starting environment and the evidence you will collect.

Run the clean-install workflow. Do not call it successful because the app opens. Prove that a new user can reach the documented starting state without cached data, hidden services, local credentials, or setup steps that are missing from the instructions.

If the check fails, stop after producing exact reproduction steps and a bounded fix recommendation. Do not silently repair the app during the verification pass.
```

## What a useful answer contains

- The exact artifact, version, size, and checksum tested.
- The clean environment and starting state.
- Installation and first-launch steps a buyer could repeat.
- Evidence for the expected starting screen.
- Any hidden setup or missing instruction.
- A clear pass, fail, or blocked result.

If this check finds a real gap, use `bug-reproducer` next. When the important checks pass, use `go-no-go-coordinator` for the release decision.

## Continue through the full launch

Builder Edition v1.4 adds 21 more skills for scoping, acceptance criteria, failure recovery, privacy, auth, payments, migrations, packaging, store review, support, and the final release decision.

Get all 24 skills for $29.25 with the launch offer applied:

https://haonv2.gumroad.com/l/vibe-coding-app-launch-kit?offer_code=LAUNCH25&wanted=true&utm_source=free_pack&utm_medium=download&utm_campaign=v14_launch
