---
name: ui-polish-pass
description: "Apply tasteful product polish without random redesign: hierarchy, spacing, empty states, and mobile sanity."
author: Mustafa / @mustafaiscoding
license: MIT
tags: [vibe-coding, ai-agents, claude-code, cursor, codex, builders]
---

# UI Polish Pass

## What this skill does

Apply tasteful product polish without random redesign: hierarchy, spacing, empty states, and mobile sanity.

Use it when you want AI speed without the usual vibe-coding tax: vague scope, broken demos, missing tests, or code that looks done but cannot ship.

## Operating mode

1. **Name the outcome** — one sentence, user-visible, demoable.
2. **List constraints** — stack, files to avoid, style, deadline, and non-goals.
3. **Create a tiny proof loop** — test, script, screenshot, curl command, or manual checklist.
4. **Build one vertical slice** — no speculative framework work.
5. **Verify out loud** — report the exact command or evidence that proves the slice works.

## Prompt template

```text
Use the UI Polish Pass skill.
Goal: <what I want built or improved>
Context: <repo/app/user/problem>
Constraints: <stack, files, time, style>
Done means: <observable proof>
Do not: <scope traps or risky changes>
```

## Anti-patterns this skill blocks

- Starting with a folder explosion instead of a working slice.
- Accepting generated code without a verification loop.
- Rewriting the app to fix one small issue.
- Shipping a README claim that no command has proven.
- Letting the agent hide uncertainty behind confident prose.

## Done checklist

- [ ] The request has a one-line success condition.
- [ ] The agent knows what not to change.
- [ ] There is at least one concrete verification step.
- [ ] The final answer includes evidence, not vibes.

---

Part of **Vibe Coder Skills** by Mustafa — Instagram: [@mustafaiscoding](https://instagram.com/mustafaiscoding), X/Twitter: [@_mustafa30_](https://twitter.com/_mustafa30_).
