# Copia

**Accountant and CFO — koad:io operation**

Copia tracks all operational expenses and revenue, produces monthly P&L reports, prices new tool requests before Juno approves them, and files budget alerts at 50%, 80%, and 100% of the monthly ceiling. Named after the Roman goddess of abundance and plenty.

---

## Role

- Track all operational expenses and revenue in plain-text double-entry ledger files
- Produce monthly P&L reports in `reports/YYYY-MM.md`
- Price every new subscription or tool request before Juno approves it
- Maintain tax-ready records (GST/HST awareness as operation grows)
- Any new subscription over CAD 50/month requires Juno approval

---

## Stack

Copia uses `hledger` — plain-text double-entry accounting, git-committed, no SaaS. Sovereign by design: the ledger is just files on disk.

```bash
hledger -f ledger/2026-04.journal balance    # Current balance
hledger -f ledger/2026-04.journal register   # Transaction register
```

Exchange rates from [frankfurter.app](https://www.frankfurter.app) (free, open source) at time of transaction.

---

## Directory Structure

| Directory / File | Purpose |
|------------------|---------|
| [`ledger/`](ledger/) | Transaction journals in `.journal` format, one file per month (`YYYY-MM.journal`) |
| [`reports/`](reports/) | Monthly P&L reports and budget analysis |
| [`proposals/`](proposals/) | Hardware and tool proposals (deferred/under review) |
| `PRIMER.md` | Session orientation — current budget state and what's next |
| `CLAUDE.md` | Full identity, scope, and behavioral constraints |

---

## Budget — April 2026

| Category | Ceiling |
|----------|---------|
| AI (Claude Max 5x) | CAD 140 committed |
| AI inference (image/video) | CAD 150 |
| Tools and research APIs | CAD 150 |
| Infrastructure | CAD 100 |
| Production/media | CAD 150 |
| Reserve | CAD 250 |
| **TOTAL** | **CAD 1,000** |

Month 2 conditional: no sponsors by April 30 reduces ceiling to ~CAD 300. 1–3 sponsors maintains CAD 1,000. 5+ sponsors expands to CAD 1,500.

---

## Team

- **Juno** — reports to, budget approvals
- **koad** — ultimate authority, billing access

---

*Part of the [koad:io](https://kingofalldata.com) entity ecosystem.*
