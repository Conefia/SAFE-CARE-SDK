# Repo settings to apply in GitHub — SAFE-CARE-SDK

Paste these into **Settings** after the first commit. (These are not applied by files; set them in the GitHub UI.)

## Description
Public client SDK for the SAFE-CARE evaluation API: register agents, submit transcripts, run evaluations, and fetch scorecards. Thin client only — no scoring logic, no guardrail rules. Apache-2.0.

## Topics
`conefia safe-care ai-evaluation llm-evaluation sdk healthcare-ai apache-2-0 python typescript`

## Settings
- Visibility: PUBLIC
- Branch protection on `main`: require PR, require 1 review, require the IP & secret scan status check, no force-push.
- Enable: Secret scanning + Push protection, Dependabot alerts, private vulnerability reporting.
- Add the `.github/workflows/ip-scan.yml` status check as a required check.

## CODEOWNERS
Edit `.github/CODEOWNERS` and replace the placeholder handle(s) with real GitHub usernames.
