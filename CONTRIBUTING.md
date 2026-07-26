# Contributing to SAFE-CARE-SDK

## Read first
1. [`IP-BOUNDARY.md`](IP-BOUNDARY.md) — non-negotiable. What may and may not live here.
2. [`AGENTS.md`](AGENTS.md) — if you use an AI coding assistant.
3. [`SECURITY.md`](SECURITY.md) — reporting and secret handling.

## Workflow
- Branch from `main`; open a pull request. Direct pushes to `main` are disabled.
- Every PR uses the pull-request template and must tick the IP / leak checklist.
- At least one review from a code owner (see `.github/CODEOWNERS`) is required to merge.
- CI runs a secret + forbidden-term scan on every push and PR. A failing scan blocks the merge.

## Casing convention
- Repository names follow the brand: **SAFE-CARE-Engine**, **SAFE-CARE-Studio**, **SAFE-CARE-SDK**.
- Package and image identifiers are lowercase: `safe-care-studio` (npm/PyPI), `safe-care-engine` (Docker) — those registries require it.

## Never commit
Secrets, `.env`, real client/tenant names, PHI, real transcripts, or anything else on the
"never here" list in `IP-BOUNDARY.md`. When in doubt, ask **dev@conefia.com** before pushing.
