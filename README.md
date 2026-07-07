# Brotherhood Blitz FFL Feedback

Public feedback intake for Brotherhood Blitz FFL.

This repository is for league members to report bugs, missing data, confusing pages, speed issues, visual issues, and feature ideas. It does not contain the private Brotherhood Blitz site code.

Project board:

[Brotherhood Blitz League Feedback](https://github.com/users/pmanaseri/projects/3)

## File A Report

Use the issue form that best matches the problem:

- Bug Report
- Feature Request
- Scoring / Stats Issue
- Roster / Owner / Team Issue
- Visual / UI Issue
- Speed / Performance Issue
- General / Missing

If none of the forms fit, use General / Missing.

## What To Include

- The page or area where the issue happened.
- What you expected to happen.
- What actually happened.
- Screenshots or screen recordings when visuals matter.
- Browser, device, or app details when the problem is device-specific.
- Season, week, team, owner, player, or matchup details when the report is about league data.

Do not post passwords, tokens, private account details, payment info, or anything that should stay off a public issue tracker.

## How Reports Are Organized

Issues use a small set of structured labels:

- `type:*` describes the kind of report.
- `component:*` describes the site area or backend/data owner.
- `impact:*` describes the user-facing symptom.
- `priority:*` describes urgency.
- `status:*` describes triage state.

The full taxonomy is documented in [docs/feedback-taxonomy.md](docs/feedback-taxonomy.md).

When a new site module, section, or backend area is added, update the feedback intake using [docs/adding-new-area.md](docs/adding-new-area.md).

## Maintainer Notes

Keep this repo clean and league-facing:

- Use plain language in issue forms.
- Keep developer-only backlog in the private repo.
- Add new components only when the site area actually exists.
- Keep General / Missing as the catch-all instead of adding speculative labels.
- Close duplicates and stale reports with a clear reason.
