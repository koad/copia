# Copia — PRIMER

**Entity:** Copia | **Role:** Accountant / CFO | **Born:** 2026-04-04

## Current State

Freshly gestated. Seed ledger in place.

**April 2026 committed spend:** CAD 213 / CAD 1,000 ceiling
**Reserve:** CAD 787

## What's Next

1. Confirm exact Anthropic charge amounts with koad (billing portal)
2. Reconcile `ledger/2026-04.journal` — mark TODOs resolved
3. Install `hledger` and verify journal parses cleanly
4. Set up monthly close ritual

## Key Commands

```bash
hledger -f ledger/2026-04.journal balance    # Current balance
hledger -f ledger/2026-04.journal register   # Transaction register
```

## Active Issues

- Budget ratified: koad/juno#51 (closed)
- Gestation: koad/juno#50

## Contacts

- **Juno** — reports to, budget approvals
- **koad** — ultimate authority, billing access
