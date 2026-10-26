# Security Policy

This file lives in the VisionVend `.github` repo, so it is the default
security policy for every VisionVend org repo that does not define its
own. A repo's own `SECURITY.md` always takes precedence over this one.

## Reporting a vulnerability

Do **not** open a public issue for a security problem. Report it privately
to the org owner via the business contact in `profile/README.md`
(email info@vision-vend.com). Include the repo, the affected version or
commit, and steps to reproduce if you have them.

## Scope notes for this org

- VisionVend repos are currently private, which limits exposure but does
  not make a repo secret-free: a secret committed to history stays
  committed. If a secret is found in history, rotate it; archiving or
  deleting a repo does not remediate it.
- Several VisionVend services run on LAN/Tailscale networks with
  unauthenticated endpoints by default (hub dashboards, camera bridges,
  training consoles). Reports about authentication on those surfaces are
  in scope and welcome, even when the service is "LAN-only" by design.
- Device hardening counts too: if a flashed board or deployed kit still
  runs a default or placeholder credential, report it as a device issue,
  not just a repo issue.
- Supported versions: there is no published release-support window for
  these repos. Report against the current `main` branch unless the issue
  is specific to a deployed kit or tagged release — say which.
