# Public-Release Boundary and Ownership

SAFE-CARE-SDK is a thin, public client for the SAFE-CARE evaluation API. It deliberately does not
contain the implementation of the evaluation engine or the operational configuration of any
deployed system.

## Ownership
All methodology, evaluation design, scoring logic, guardrail and escalation logic, and the
implementation behind the API are the intellectual property of Conefia, LLC (d/b/a Conefia
Technologies), and are NOT published here. See the Conefia Intellectual Property Policy at
https://conefia.com/ip-policy. Publication of this SDK is an exercise of that ownership, not a
waiver of it.

## What this repository contains
- A thin API client and type definitions for the public SAFE-CARE evaluation API.
- Documentation and synthetic, generic examples.

## What this repository does not contain, by design
- Scoring weights, aggregation logic, guardrail rules or thresholds, or escalation decision logic.
- Premium scenarios, the qualification library, or judge-calibration data.
- Any client or partner name, or any identification of a specific deployment.
- Internal service/class names, database schemas, environment-variable names, or deployment identifiers.
- Real user data, production telemetry, screenshots, or credentials.

## Synthetic data only
Every example is synthetic. No real patient data, production logs, or protected health information
appears anywhere in this repository or its history.

## Reporting
If you believe any file here discloses information that should not be public, contact
dev@conefia.com before opening a public issue.

(C) 2026 Conefia, LLC. SAFE-CARE(TM) is a trademark of Yassen Eltayeb / Conefia, LLC.
