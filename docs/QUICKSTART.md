# Quickstart

Install the skills:

```bash
npx skills add mustafa3252/vibe-ship-skills --all
```

## 1. Pick one loop

Do not automate everything on day one. Pick one boring loop that already wastes your time.

Good first picks:

- daily hygiene report
- PR babysitter
- launch polish checklist
- bug replay loop

## 2. Start at L1

L1 means report-only. The agent can inspect and summarize, but it cannot edit files.

```text
Use the agent-brief, prompt-to-plan, and ship-it-check skills.
Goal: Run a daily project hygiene loop.
Level: L1 report-only.
Inputs: open issues, failing CI, TODOs, recent commits.
Output: a short report with recommended next actions.
Do not change files.
```

## 3. Add state

Create a tiny `STATE.md` in your project:

```md
# STATE.md

Current focus:
Known risks:
Last loop result:
Next recommended action:
```

The point is not bureaucracy. The point is to stop re-explaining the same context every time.

## 4. Move to L2 only when the reports are useful

L2 lets the agent open a small PR. You still merge manually.

```text
Level: L2 assisted PR.
Allowed actions: create a branch, edit docs/tests, run checks, open a PR.
Human gate: required before merge.
```

## 5. Keep the loop small

If the loop produces noisy work, reduce the scope. A useful loop should make your next decision easier, not create another thing to babysit.
