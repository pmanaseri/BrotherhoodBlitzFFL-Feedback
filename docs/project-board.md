# Project Board Shape

Recommended board name:

[Brotherhood Blitz League Feedback](https://github.com/users/pmanaseri/projects/3)

## Status Field

Use these statuses:

- New
- Needs Info
- Accepted
- In Progress
- Ready for Review
- Done
- Duplicate
- Not Planned

## Recommended Views

- Incoming Triage: `status: new`
- League Blockers: `priority: league-blocker`
- Data / Stats: `impact: Data/Stats`
- UI / Visual / Mobile: `impact: UI`, `impact: Visual`, or `impact: Mobile`
- Speed: `impact: Speed`
- By Component: grouped by component label or Project component field
- Done / Closed: completed work and closed decisions

## Board Rules

- Every issue starts in New.
- Needs Info means the report cannot move forward without details from the reporter.
- Accepted means the report is valid and should be handled.
- In Progress means someone is actively working it.
- Ready for Review means the reporter or maintainer should verify the result.
- Done means the work is completed.
- Duplicate and Not Planned should be closed with a clear comment.

## Auto-Add Rule

Issue forms include `projects: ["pmanaseri/3"]` so maintainer-created issues land on this board.

For public league reporters who may not have project write access, also enable the built-in Project workflow:

- Workflow: Auto-add to project
- Repository: `pmanaseri/BrotherhoodBlitzFFL-Feedback`
- Filter: `is:issue`

GitHub's issue-form `projects` key requires project write access from the issue opener, so the built-in auto-add workflow is the reliable league-facing path.

## Repo Relationship

This feedback repo is public. The private development repo remains the implementation workspace.

When a league report turns into private implementation work:

1. Keep the public issue focused on the visible problem and expected outcome.
2. Create or link private work privately when needed.
3. Do not copy private stack details, API keys, logs, server paths, or sensitive internals into public issues.
