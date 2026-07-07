# Feedback Taxonomy

This document is the source of truth for the league-facing feedback structure.

The private development repo can have deeper engineering labels. This public feedback repo should stay organized around what league members can see, report, and understand.

## Label Families

### Type

Apply exactly one type label after triage.

- `type: bug`: broken or incorrect behavior.
- `type: feature`: new request or improvement idea.
- `type: question`: clarification, confusion, or support-style report.

### Status

Use status labels to keep the intake lane readable.

- `status: new`: submitted and not fully triaged.
- `status: needs info`: blocked on reporter details.
- `status: accepted`: valid and accepted into the work queue.
- `status: in progress`: being actively worked.
- `status: ready for review`: fix or decision is ready to verify.
- `status: blocked`: accepted but blocked by another dependency.
- `status: done`: completed.
- `status: duplicate`: same issue already exists.
- `status: not planned`: valid report, but not planned.

### Priority

Priority is optional and should be used sparingly.

- `priority: league-blocker`: blocks league usage, data trust, access, or core workflows.
- `priority: important`: should be handled soon, but the league can keep operating.
- `priority: polish`: quality, clarity, or presentation improvement.

### Impact

Impact labels describe the symptom from the user's view.

- `impact: UI`: controls, layout, navigation, or interaction problem.
- `impact: Visual`: styling, spacing, alignment, color, images, or presentation problem.
- `impact: Speed`: slow page, timeout, delayed load, or stuck state.
- `impact: Mobile`: phone or small-screen issue.
- `impact: Data/Stats`: wrong, missing, stale, or confusing league data.
- `impact: Access/Login`: login, permission, visibility, or role access issue.
- `impact: Copy/Content`: wording, page text, labels, or instructions.

### Components

Component labels describe ownership. Apply at least one component label after triage.

Active top-level modules:

- `component: Banner`
- `component: Owners Directory`
- `component: Salary Dashboard`
- `component: League Analytics`
- `component: Team Front Office`
- `component: General/Missing`

Team Front Office sections:

- `component: Press Box`
- `component: Salary Report`
- `component: Trade Block`
- `component: Roster`
- `component: Transactions`
- `component: Draft Board`
- `component: Alerts`

Backend and data ownership:

- `component: Backend/Data`
- `component: Identity/Owners`
- `component: Rosters`
- `component: Salary Manager`
- `component: League Data`
- `component: Matchups/Standings`
- `component: Drafts/Picks`
- `component: Calendar/Scoring`

## Triage Rules

- Keep reports in this repo league-facing.
- Keep internal implementation tasks in the private development repo.
- Use `component: General/Missing` when a report does not clearly map to an existing area.
- Do not add labels for planned future areas until the area exists.
- Do not preserve old pre-production labels unless the current site still exposes that area.
- If a report crosses frontend and backend ownership, use both the visible component and the backend/data component.
- If the issue affects trust in score, roster, standings, salary, or matchup data, add `impact: Data/Stats`.
- If the issue blocks a weekly league workflow, add `priority: league-blocker`.

## Current Site Areas Behind This Taxonomy

The active public/admin module set is:

- Banner
- Owners Directory
- Salary Dashboard
- League Analytics
- Team Front Office

Team Front Office currently exposes:

- Press Box
- Salary Report
- Trade Block
- Roster
- Transactions
- Draft Board
- Alerts

Known backend/data ownership includes:

- Salary Manager
- Team Front Office stack
- League Analytics stack
- Site Identity / Users / Avatars
- Rosters
- Matchups
- Standings
- Transactions
- Draft picks and traded picks
- League drafts and projected draft board
- NFL calendar and scoring state

