# Contributing to VisionVend

This file lives in the VisionVend `.github` repo, so it is the default
contributing guide for every VisionVend org repo that does not define its
own. A repo's own `CONTRIBUTING.md` always takes precedence over this one.

## Ground rules

- **VisionVend repos are private.** Do not publish, mirror, or share repo
  contents outside the org without 's explicit approval.
- **No commits, pushes, deploys, or external messages ship on silence.**
  Every change of that kind needs 's explicit word first.
- **Never permanently delete files on his machines** — move to Trash only;
   empties the Trash himself. Never delete a repo, and never delete a
  repo name that might be a transfer redirect (deleting the old name can
  delete the repo itself — see the `vv-capture` / `vv-capture-fork-legacy`
  and `visionvend-cam` redirect cases).
- **Verify before asserting.** Show actual command output, not a claim, for
  anything  will act on. Check the standing notes before asking him
  to do something by hand.
- **No secrets in code, docs, or commit messages.** Credentials go through
  the Secure Vault only. If you find a secret in history, report it and
  rotate it — archiving or deleting does not remediate a committed secret.
- **Backups before status changes.** Before archiving, unarchiving, or
  renaming a repo, confirm at least two local copies plus GitHub exist.

## Workflow

1. Work on a branch, never direct to `main` for anything non-trivial.
2. Keep the diff scoped to what the commit message describes — a message
   must describe only what its diff actually does.
3. Update the affected README/docs in the same change, not as a follow-up.
4. If a repo is archived, do not edit it in place: an archived-repo fix
   needs an approved unarchive → edit → re-archive cycle.
5. When a repo is created or archived, update the repo table in
   `profile/README.md` in this repo in the same batch — the table rotted
   in six days in October 2026 because that step was skipped.

## Reporting problems

Open an issue in the affected repo using its issue template (or this
repo's default templates if it has none). Security problems go through
`SECURITY.md`, not a public issue.
