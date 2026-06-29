# Daily hygiene loop

Runs on a schedule, summarizes repo health, and recommends the smallest useful next action.

## Inputs

- repo state
- recent commits or issues
- allowed files
- explicit non-goals

## Default level

Start at **L1 report-only**. Move to L2 only when the reports are consistently useful.

## Prompt

```text
Use the Vibe Ship loop style.
Pattern: Daily hygiene loop
Level: L1 report-only
Goal: <what this loop should watch or improve>
Allowed actions: read and report only
Human gate: required before file edits, commits, or external actions
```

## Done

The loop produces a short report with evidence and one recommended next action.
