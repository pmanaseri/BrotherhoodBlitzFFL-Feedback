# Adding A New Feedback Area

Use this checklist when Brotherhood Blitz adds a new site module, Team Front Office section, admin tool, backend stack, or public-facing feature area.

## 1. Confirm The Area Exists

Only add a feedback component after the area exists in the site or is intentionally exposed to league users.

Do not create labels for speculative future work.

## 2. Pick The Public Name

Use the name league members will recognize.

Good component names:

- `component: Salary Dashboard`
- `component: Draft Board`
- `component: Calendar/Scoring`

Avoid internal-only names unless they are the clearest owner for triage.

## 3. Decide The Ownership Lane

Choose one primary lane:

- Top-level module
- Team Front Office section
- Backend/data owner
- General/Missing

If the area has both a visible page and a backend owner, keep both available. Example: a standings display bug may use `component: Team Front Office`, `component: Matchups/Standings`, and `impact: Data/Stats`.

## 4. Add The Label

Add a `component:*` label with:

- Name: `component: Area Name`
- Description: short and league-readable
- Color: consistent with the component family

Also update `.github/labels.json` so labels can be recreated or audited later.

## 5. Update Issue Forms

Update the component dropdown in each issue form that should accept reports for the new area:

- `.github/ISSUE_TEMPLATE/bug-report.yml`
- `.github/ISSUE_TEMPLATE/feature-request.yml`
- `.github/ISSUE_TEMPLATE/scoring-stats-issue.yml`
- `.github/ISSUE_TEMPLATE/roster-owner-team-issue.yml`
- `.github/ISSUE_TEMPLATE/visual-ui-issue.yml`
- `.github/ISSUE_TEMPLATE/speed-performance-issue.yml`
- `.github/ISSUE_TEMPLATE/general-missing.yml`

GitHub issue forms do not share dropdown lists, so every relevant form must be updated directly.

## 6. Update The Docs

Update:

- `README.md` if the area changes how league members should report issues.
- `docs/feedback-taxonomy.md` so the component list remains the source of truth.
- `docs/project-board.md` if the new area needs a board view, saved filter, or custom triage note.

## 7. Backend Work Rule

If the new area has backend or stack ownership, keep private implementation work in the private development repo and follow the backend guides there:

`C:\Users\PatTheMerciless\Desktop\Brotherhood Website\Master Files - SoT\Backend Guides`

This public repo should track the league report and visible outcome, not private backend implementation details.

## 8. New Area Acceptance Check

Before calling the new feedback area ready, confirm:

- The label exists on GitHub.
- `.github/labels.json` includes the label.
- Relevant issue forms include the area in the dropdown.
- `docs/feedback-taxonomy.md` lists the area.
- Any Project board view or filter has been updated.
- General/Missing still exists as the catch-all.

