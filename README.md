# SAFE-CARE-SDK

> **PUBLIC · Tier 3 — Public**  |  Apache-2.0

The public client SDK for the SAFE-CARE evaluation API — register an agent, submit transcripts, run an evaluation, and fetch results and scorecards. It ships NO internal logic.

---

## ⛔ Before your first commit

**Read [`IP-BOUNDARY.md`](IP-BOUNDARY.md).** It defines exactly what belongs in this repo,
what must never touch it, and the one leak we are never repeating. Every pull request must
pass the checklist in that file. If you use an AI coding assistant, point it at
[`AGENTS.md`](AGENTS.md) first.

## What this repo is

The public client SDK for the SAFE-CARE evaluation API — register an agent, submit transcripts, run an evaluation, and fetch results and scorecards. It ships NO internal logic.

It is one repo in the SAFE-CARE Lab system. The full picture — the one-engine / six-surfaces
model, the tiers, and the IP firewall — is in the internal *SAFE-CARE Lab — Architecture & IP Protection Strategy (Conefia/Projects/SAFE-CARE/SAFE-CARE-Lab-Strategy)*.

## ✅ What belongs here

- A thin API client (Python and TypeScript) for the PUBLIC SAFE-CARE evaluation API: register an agent, submit transcripts, run an evaluation, fetch results and scorecards, and test guardrails (pass/fail only).
- Type/model definitions for the public API request/response shapes.
- Examples that use ONLY synthetic, generic agents (e.g. "DemoCare Clinic", "Example Health Assistant").
- Documentation and a quickstart.
- Tests that run against a mocked API.

## ⛔ What must never be here

- Scoring weights, aggregation logic, guardrail rules or thresholds, or the escalation decision logic.
- Premium scenarios, the qualification library, or judge-calibration data.
- ANY client or partner name, or anything that identifies a specific deployment.
- Real transcripts, real patient data, PHI, production logs, or screenshots.
- Internal service/class/module names, database schema/table/field names, environment-variable names, or model-deployment identifiers.
- Internal or private endpoints — only the documented public API base URL (https://api.conefia.com/v1).
- Secrets, API keys, tokens, or credentials.
- Prompt libraries or the logic used to assemble production prompts.

## Status

Skeleton — first commit. Structure and code to follow. This initial push exists to carry the
guardrails (`IP-BOUNDARY.md`, `AGENTS.md`, `CONTRIBUTING.md`, `SECURITY.md`, PR template, leak-scan CI)
before any code lands.

## License

Apache-2.0 (see `LICENSE`). SAFE-CARE™ is a trademark of Yassen Eltayeb / Conefia, LLC.

## Contact

Questions, or unsure whether something is safe to commit: **dev@conefia.com** — ask first.
