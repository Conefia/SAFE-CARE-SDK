# Instructions for AI coding assistants

Before generating, editing, or suggesting any code in this repository, **read
[`IP-BOUNDARY.md`](IP-BOUNDARY.md) and obey it without exception.**

## Context
- Repository: **SAFE-CARE-SDK**
- Visibility: **PUBLIC** (Tier 3 — Public)
- This repository is PUBLIC. Assume everything you write here becomes world-readable immediately and stays in git history forever.

## Hard rules for this repo
- Scoring weights, aggregation logic, guardrail rules or thresholds, or the escalation decision logic.
- Premium scenarios, the qualification library, or judge-calibration data.
- ANY client or partner name, or anything that identifies a specific deployment.
- Real transcripts, real patient data, PHI, production logs, or screenshots.
- Internal service/class/module names, database schema/table/field names, environment-variable names, or model-deployment identifiers.
- Internal or private endpoints — only the documented public API base URL (https://api.conefia.com/v1).
- Secrets, API keys, tokens, or credentials.
- Prompt libraries or the logic used to assemble production prompts.

## Behaviour
- Never invent, paste, or hardcode client names, real data, secrets, or engine internals.
- Use only synthetic, generic placeholders in examples (e.g. "DemoCare Clinic", "Example Health Assistant").
- If a request would require exposing anything on the "never here" list, **refuse and cite `IP-BOUNDARY.md`** instead of complying.
- If you are unsure whether something is safe to write here, say so and stop — do not guess.

This file is guidance for humans and tools alike. It does not override `IP-BOUNDARY.md`; it enforces it.
