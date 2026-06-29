# Loop design

A Vibe Ship loop has six parts.

## 1. Trigger

What starts the loop?

- manual prompt
- GitHub issue label
- PR event
- daily schedule
- failed CI

## 2. Scope

What is the loop allowed to touch?

Good scope:

```text
Only inspect README, docs, examples, and open issues.
Do not edit source code, secrets, auth, deploy config, or billing files.
```

Bad scope:

```text
Improve the whole repo.
```

## 3. State

Where does the loop remember context?

Use one or more of:

- `STATE.md`
- issue comments
- PR comments
- changelog notes
- a task board

State should be short. If it becomes a diary, the agent will stop reading it.

## 4. Worker

The worker is the agent that does the task. Keep it boxed in with a brief:

```text
Role: docs fixer
Goal: make install instructions accurate
Allowed: README, docs/QUICKSTART.md
Not allowed: package config, source code, release tags
```

## 5. Verifier

Every loop needs proof.

Examples:

- `npm test`
- `npx skills add owner/repo --list`
- screenshot check
- curl endpoint check
- markdown link validation
- second-agent review

## 6. Human gate

Decide what always stops for approval.

Recommended hard gates:

- deploys
- deletes
- billing
- secrets
- auth
- database migrations
- dependency major upgrades
- auto-merge

Good loops do not remove your judgment. They protect it from busywork.
