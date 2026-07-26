# Security Policy — SAFE-CARE-SDK

## Reporting
Report any suspected exposure of secrets, client data, or Conefia intellectual property — or any
security vulnerability — privately to **dev@conefia.com**. Do not open a public issue for a
suspected leak or vulnerability.

## If something sensitive was committed
1. Do **not** just delete the file in a new commit — the data remains in git history.
2. Notify **dev@conefia.com** immediately.
3. Rotate any exposed secret at once (revoke keys/tokens).
4. History must be purged (e.g. `git filter-repo`) and, for a public repo, assume the value is
   already compromised and rotate regardless.

## Secret handling
- No secrets in source. Use environment variables loaded from a secret manager; keep a committed
  `.env.example` with placeholder keys only.
- GitHub secret scanning and push protection should be **on** for this repository.

See [`IP-BOUNDARY.md`](IP-BOUNDARY.md) for what counts as sensitive here.
