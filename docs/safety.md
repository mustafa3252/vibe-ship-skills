# Safety rules

Use automation like deploy access: slowly.

## Default denylist

A Vibe Ship loop should not touch these without explicit approval:

- secrets or `.env` files
- billing or payment settings
- auth providers
- production deploy config
- database migrations
- destructive deletes
- dependency major upgrades
- branch protection
- GitHub repo settings

## Trust levels

| Level | Allowed | Not allowed |
|---|---|---|
| L1 | read, summarize, recommend | file edits, comments, commits |
| L2 | branch, small edits, tests, PR | merge, deploy, destructive changes |
| L3 | allowlisted chores | anything outside the written policy |

## Kill switch

Stop a loop if it:

- creates repeated low-signal reports
- opens PRs you do not want to review
- changes files outside scope
- fails to include verification evidence
- gets stuck retrying the same bad fix

## The rule

If you cannot explain what the loop did, you cannot trust it yet.
