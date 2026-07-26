# ⛔ IP BOUNDARY — READ BEFORE YOUR FIRST COMMIT

**SAFE-CARE-SDK · PUBLIC · Tier 3 — Public**

> **This repo is PUBLIC.** Everything here is world-readable the moment it is pushed, and it stays in git history forever — deleting a file does not un-leak it. Assume every commit is a press release.

This file is the contract for what may and may not live in this repository. It exists because
Conefia's advantage is its intellectual property, and one careless commit can give it away
permanently. Read it fully before you write code here, and re-read the checklist before every push.

## 1. What this repo is
The public client SDK for the SAFE-CARE evaluation API — register an agent, submit transcripts, run an evaluation, and fetch results and scorecards. It ships NO internal logic.

## 2. ✅ Belongs here
- A thin API client (Python and TypeScript) for the PUBLIC SAFE-CARE evaluation API: register an agent, submit transcripts, run an evaluation, fetch results and scorecards, and test guardrails (pass/fail only).
- Type/model definitions for the public API request/response shapes.
- Examples that use ONLY synthetic, generic agents (e.g. "DemoCare Clinic", "Example Health Assistant").
- Documentation and a quickstart.
- Tests that run against a mocked API.

## 3. ⛔ NEVER here — the danger zone
- Scoring weights, aggregation logic, guardrail rules or thresholds, or the escalation decision logic.
- Premium scenarios, the qualification library, or judge-calibration data.
- ANY client or partner name, or anything that identifies a specific deployment.
- Real transcripts, real patient data, PHI, production logs, or screenshots.
- Internal service/class/module names, database schema/table/field names, environment-variable names, or model-deployment identifiers.
- Internal or private endpoints — only the documented public API base URL (https://api.conefia.com/v1).
- Secrets, API keys, tokens, or credentials.
- Prompt libraries or the logic used to assemble production prompts.

## 4. Why this boundary exists
Everything that lands in this repo is world-readable, forever, and remains in git history even after deletion. Treat every file as a press release. A prior public research repository accidentally shipped a client's production architecture — internal service and class names, environment variables, database schema fields, and prompt-assembly logic — alongside written records of unfixed defects. It had to be pulled offline and made private, but the exposure could not be undone because the repository had already been cloned and cached elsewhere. That must never happen again. When in doubt, leave it out and ask.

## 5. What happened last time (learn from it)
A previous public repository in this program accidentally exposed a client's production internals —
internal service and class names, environment variables, database schema fields, and the logic used
to assemble production prompts — together with written notes about unfixed defects. The repository
had to be taken offline and made private. Because it had already been cloned and cached, the exposure
was permanent and could not be reversed. The damage was not the code itself — it was that it named
a real client's system and revealed how it worked. Do not let convenience recreate that mistake.

## 6. Before EVERY push — checklist
- [ ] No secrets, API keys, tokens, passwords, or `.env` files.
- [ ] No real client or tenant names; no PHI; no real transcripts or production logs.
- [ ] No hardcoded client/tenant — tenancy is configuration, not code.
- [ ] No engine internals (scoring weights, guardrail rules, escalation logic) — this repo calls the engine via its API.
- [ ] No internal service/class names, DB schema/fields, env-var names, or deployment identifiers.
- [ ] Only synthetic, generic examples (e.g. "DemoCare Clinic").
- [ ] I read this file and my change respects it.

## 7. If you are not 100% sure
Stop. Do not push. Ask **dev@conefia.com** first. "When in doubt, leave it out" is always the
right call — it is far cheaper to ask than to un-leak.

## 8. Where the full rules live
- Internal: *SAFE-CARE Lab — Architecture & IP Protection Strategy (Conefia/Projects/SAFE-CARE/SAFE-CARE-Lab-Strategy)* and the **SAFE-CARE Lab — Engineering Build Guide**.
- Conefia **Intellectual Property Policy**: https://conefia.com/ip-policy
- Master Services Agreement IP terms (§2.2 Conefia Background IP incl. SAFE-CARE™; §7).

© 2026 Conefia, LLC. SAFE-CARE™ is a trademark of Yassen Eltayeb / Conefia, LLC.
