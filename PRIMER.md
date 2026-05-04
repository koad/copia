# Copia — PRIMER

**Entity:** Copia | **Role:** Accountant / CFO | **Born:** 2026-04-04

> Visitor context. This file is read by visitors, not Copia. Public-safe.

## Current State (as of 2026-05-01)

Books operational. April subscription total confirmed at CAD 353.55 (billing portal 2026-04-29). April remains open pending two session-compute entries for 2026-04-21 and 2026-04-24/25 — koad must pull billing portal figures before those entries can be recorded. May 2026 journal is live. The session-cost emission hook went live 2026-04-30 (commit 81f50e2): all future Juno dispatch sessions auto-emit cost via `hooks/emit-session-cost.py`.

**ADAS two-track framing (effective 2026-05-01):** Claude Max sessions are flat-subscription — no metered Anthropic charges are generated regardless of token volume. The hook now emits to `expenses:ai:adas:shadow` (informational; no alert) to represent the metered-equivalent leverage value. Real billed ADAS spend (Grok API, direct API calls outside Max) records to `expenses:ai:adas:actual` where the CAD 40/month ceiling and alerts remain. The April 168% alert was a false positive against a shadow-track figure before this framing existed — it is rescinded.

**April 2026 subscription total:** CAD 353.55 confirmed (Pro CAD 31.64 + Max 5x CAD 132.01 + Max 20x upgrade CAD 221.54)
**April AI:Anthropic ceiling:** CAD 320 — BREACHED 110.5% (CAD 33.55 over ceiling); 100% alert active
**April ADAS actual outflow:** CAD 0.00 (no metered API charges; Max covers all session compute)
**April ADAS shadow (leverage figure):** ~CAD 67.23 informational (first auto-emission; not a breach)
**Revenue:** CAD 0. Zero sponsors by April 30 gate triggered Month 2 lean+essential envelope.

**May 2026 ratified ceiling: CAD 467** (CAD 357 recurring + CAD 40–110 one-time domains)
- Claude Max 20x: ~CAD 280
- Hetzner VPS (zero.koad.sh): ~CAD 25
- Vultr VPS (Toronto): ~CAD 30
- X Premium+: ~CAD 22
- Vanity domains (2–3 TLDs, Porkbun): CAD 40–110 one-time
- ADAS actual (Grok API metered): tracked under expenses:ai:adas:actual; CAD 40/month ceiling
- **Suspended:** Figma, Runway, Flux Pro, Brave (zero cost; option to resume)

**No metered API outflow to date:** Claude Max plan has no metered API charges — the monthly subscription is the entire cash cost for session compute. ADAS actual = CAD 0.00.

## What's In Flight

1. Two April session-compute gaps open (2026-04-21, 2026-04-24/25) — koad portal pull required before April close
2. May recurring charges pending (not yet billed as of 2026-05-01)
3. ADAS reframe complete (2026-05-01) — April 168% breach rescinded; shadow/actual two-track live
4. Domain purchases (2–3 TLDs, Porkbun) — one-time, budget approved; TLDs TBD
5. Tips pool reconciliation against Stripe — dance-hall not yet live; no action needed

## Commands

```bash
copia balance          # current month burn vs ceiling
copia burn             # balance with line-item detail
copia report monthly   # P&L for current / prior month
copia ceilings         # list ceilings + headroom
copia price <op> <qty> # pre-spend price estimate
```

## Key hledger queries

```bash
hledger -f /home/koad/.copia/ledger/2026-04.journal balance
hledger -f /home/koad/.copia/ledger/2026-05.journal balance
hledger -f /home/koad/.copia/ledger/2026-04.journal register expenses:ai
```

## Communication

- Internal coordination: briefs in `~/.copia/briefs/` or via MCP
- GitHub issues: public user/sponsor channel only (not internal)
- Canonical git host: `keybase://team/kingofalldata.entities.copia/self`

## Contacts

- **Juno** — orchestrator, spend authority, report recipient
- **koad** — ultimate authority, billing access, ceiling ratifications
