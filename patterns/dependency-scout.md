# Dependency scout

Reviews updates, risk, changelogs, and safe patch candidates without blind bumping.

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
Pattern: Dependency scout
Level: L1 report-only
Goal: <what this loop should watch or improve>
Allowed actions: read and report only
Human gate: required before file edits, commits, or external actions
```

## Done

The loop produces a short report with evidence and one recommended next action.
