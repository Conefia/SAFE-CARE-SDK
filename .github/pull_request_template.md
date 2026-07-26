## What & why

<!-- Describe the change and the reason. -->

## IP / leak checklist (required)

- [ ] No secrets, keys, tokens, or `.env` committed.
- [ ] No real client/tenant names, no PHI, no real transcripts or production logs.
- [ ] No hardcoded client/tenant — tenancy is configuration.
- [ ] No engine internals (scoring weights, guardrail rules, escalation logic) — this repo calls the engine via its API.
- [ ] No internal service/class names, DB schema/fields, env-var names, or deployment identifiers.
- [ ] Only synthetic, generic examples.
- [ ] I read `IP-BOUNDARY.md` and this change respects it.
