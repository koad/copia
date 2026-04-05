---
date: 2026-04-05
period: April 2026 (Day 6 of operation / Month 1)
author: copia
note: "Report titled 'Day 30' per request — actual elapsed time is 6 days. See Section 6."
status: provisional — Anthropic charges unconfirmed pending koad review of billing portal
---

# Day 30 Budget Report — April 2026

Prepared by Copia. Working directory: `/home/koad/.copia/`
Ledger source: `ledger/2026-04.journal`

---

## 1. 30-Day Cost Summary

**Actual charges to date (provisional):**

| Date       | Vendor      | Description                                     | Amount (CAD) | Status      |
|------------|-------------|-------------------------------------------------|--------------|-------------|
| 2026-04-01 | Anthropic   | Claude Pro — prorated signup charge             | 40.00        | Provisional |
| 2026-04-02 | Anthropic   | Claude Max 5x — first charge (net of CAD 40 credit) | 100.00   | Provisional |
| **Total**  |             |                                                 | **140.00**   |             |

No other charges have been recorded in the ledger. All four approved subscriptions (Figma, Runway, Brave Search, Flux) were assessed on 2026-04-05 and **deferred** — none have been provisioned. See `reports/2026-04-subscription-analysis.md` for the full cost/benefit analysis.

**Revenue to date: CAD 0.00**

**Data gaps:**
- Anthropic billing portal not yet confirmed by koad. Both line items remain marked TODO in the journal. The CAD 40 and CAD 100 figures are working estimates. Actual amounts may differ.
- Electricity costs for thinker (~CAD 3–4/month) have not been entered as a journal transaction. Hardware power draw is a real cost. See Section 5 commentary.
- No infrastructure charges recorded (hosting, domains). dotsh (Vultr VPS) may have a monthly cost that has not been submitted to the ledger. Confirm with koad.

---

## 2. Committed vs. Ceiling

| Item                                     | Amount (CAD) |
|------------------------------------------|--------------|
| Actual provisional spend (Anthropic)     | 140.00       |
| Approved but not yet provisioned         | 0.00         |
| Electricity (unrecorded, estimated)      | ~4.00        |
| **Working total committed**              | **~144.00**  |
| April ceiling (ratified 2026-04-04)      | 1,000.00     |
| **Headroom remaining**                   | **~856.00**  |

The four subscriptions recommended for deferral (CAD 73/month combined) are approved in the ratified budget but have not been activated. If they remain deactivated through April 30, committed spend stays at approximately CAD 144.

If all four were activated today, committed recurring would reach CAD 217 (CAD 213 approved + ~CAD 4 electricity). That is 21.7% of the April ceiling.

---

## 3. Cost Structure — Per Entity Per Day

**Basis:** The operation runs on a single Claude Max 5x subscription (CAD 140/month). This subscription covers all entity sessions run by koad under one account. There is no per-entity billing — entities are not separate Anthropic accounts; they are separate Claude Code working directories under one user. The cost is shared.

**Entities active as of 2026-04-05:**
Juno, Vulcan, Veritas, Mercury, Muse, Sibyl, Faber, Chiron, Argus, Janus, Salus, Aegis, Rufus, Copia, and others gestated on fourty4. Approximate count: 15–18 entities.

**Rough per-entity cost (if apportioned equally):**

| Basis                   | Calculation                 | Result           |
|-------------------------|-----------------------------|------------------|
| Claude Max — per month  | CAD 140 ÷ 16 entities       | ~CAD 8.75/entity/month |
| Claude Max — per day    | CAD 8.75 ÷ 30 days          | ~CAD 0.29/entity/day   |
| All entities — per day  | CAD 140 ÷ 30 days           | ~CAD 4.67/day total    |

**Caveat:** Not all entities run daily. Some (Vulcan, Faber, Sibyl) are active frequently; others are gestated but rarely invoked. Equal apportionment overstates cost for dormant entities and understates it for high-frequency ones. Without session telemetry (not currently tracked), a more precise per-entity figure is not available.

**Infrastructure cost per day (estimated):**
- thinker electricity: ~CAD 4/month → ~CAD 0.13/day
- dotsh VPS: cost unknown, not in ledger → gap

Total operational cost per day at current spend: approximately **CAD 4.80/day** (Claude Max + electricity estimate).

---

## 4. End-of-Month Projection

**Scenario A: Subscriptions remain deactivated (current trajectory)**

| Item                        | Monthly cost (CAD) |
|-----------------------------|-------------------|
| Claude Max 5x               | 140.00            |
| Electricity (thinker)       | ~4.00             |
| dotsh VPS (if applicable)   | unknown           |
| **Projected April total**   | **~144.00**       |
| April ceiling               | 1,000.00          |
| **% of ceiling consumed**   | **~14.4%**        |

**Scenario B: All approved subscriptions activated mid-April**

| Item                        | Monthly cost (CAD) |
|-----------------------------|-------------------|
| Claude Max 5x               | 140.00            |
| Figma Professional          | 29.00             |
| Runway Gen-4.5              | 23.00             |
| Brave Search API            | 6.00              |
| Flux via fal.ai             | 15.00             |
| Electricity                 | ~4.00             |
| **Projected April total**   | **~217.00**       |
| **% of ceiling consumed**   | **~21.7%**        |

Under either scenario, April ends well below ceiling. The operation is not budget-constrained. The constraint is revenue, not spend.

**Month 2 (May) conditional outlook — unchanged from Day 6 report:**
- Zero sponsors by April 30 → May ceiling drops to ~CAD 300 (Claude Max + essentials only)
- 1–3 sponsors → Maintain CAD 1,000
- 5+ sponsors → Expand to CAD 1,500

No sponsors as of 2026-04-05.

---

## 5. Commentary on the Day 29 Post — "$24/Month" Claim

The Day 29 post (`~/.faber/posts/2026-04-29-200-dollar-laptop.md`) makes the following claim:

> "koad:io's operational cash outlay in the same period: $24/month (Claude Code Pro at $20, electricity for thinker at approximately $3–4)."

**The ledger does not support this figure. The actual committed spend is CAD 140/month, not $24.**

**What the discrepancy is:**

The Day 29 post cites Claude Code Pro at $20/month. The actual subscription is **Claude Max 5x**, which costs **CAD 140/month** (~USD 100–105 at current exchange). The Pro plan ($20 USD) was the initial signup charge, prorated and then credited against the Max upgrade. The operation has been running on Max 5x since approximately 2026-04-02 — six times the cost of the Pro plan cited in the post.

**Why this matters:**

The post uses the $24 figure as a direct comparison against LangSmith Plus (~$79/month) and Devin Team ($500+/month). The comparison is directionally correct — koad:io is materially cheaper than those stacks — but the specific dollar figure is wrong. Using the actual number:

| Stack | Monthly Cost (USD approx.) |
|-------|---------------------------|
| koad:io sovereign (actual) | ~$105–110 (Claude Max + electricity) |
| Claude API + LangSmith Plus | ~$79+ (LangSmith alone, before API costs) |
| Devin Team plan | $500+ |

At CAD 140/month for Claude Max, the koad:io total is comparable to LangSmith Plus in absolute dollars — the ownership argument (local keys, git audit trail, no per-trace fees) is still valid and arguably stronger than the cost argument in a like-for-like comparison at this tier. The comparison is more nuanced than the post presents.

**The caveat in the post:**

The post correctly notes the Anthropic vendor dependency and explicitly states sovereignty is partial. That framing is accurate. The dollar figure, however, should be corrected before the post is distributed.

**Recommended correction:**

Replace the $24/month figure with the actual figure. The honest version: "CAD ~145/month (Claude Max 5x at CAD 140 + ~CAD 4 electricity)." The sovereignty argument survives this correction — it just changes the comparison tier from LangSmith's lower plans to LangSmith Plus. The ownership advantages (git audit trail, local keys, no per-trace retention fees) remain the stronger case.

**Action required:** Flag to Faber and koad before this post is published or distributed. The $24 figure appears to have been drafted during or before the Max upgrade. The post was written 2026-04-29 (per its filename), which is in the future — this may be a forward-scheduled piece drafted from Day 1 assumptions that were not updated after the plan upgrade.

---

## 6. Note on Report Title — "Day 30"

This report is titled "Day 30" per the request. For the record: the operation began 2026-03-30. As of this report date (2026-04-05), **6 days have elapsed**, not 30. The ledger reflects 6 days of activity. The "Day 29 post" referenced in the request is a forward-scheduled piece authored by Faber with a publication date of 2026-04-29. The 30-day window in this report is therefore a projection framework, not a completed period.

The financial data above covers the full operational period to date (6 days). The projection section covers the remainder of April.

---

## Summary

| Metric                          | Value              |
|---------------------------------|--------------------|
| Actual spend (provisional)      | CAD 140.00         |
| Electricity (unrecorded est.)   | ~CAD 4.00          |
| Total working committed         | ~CAD 144.00        |
| Approved unactivated            | CAD 73.00          |
| April ceiling                   | CAD 1,000.00       |
| Reserve remaining               | ~CAD 856.00        |
| % of ceiling consumed           | ~14.4%             |
| Revenue to date                 | CAD 0.00           |
| End-of-month projected (no new subs) | ~CAD 144.00   |
| End-of-month % of ceiling       | ~14.4%             |
| Day 29 post "$24/month" claim   | **Incorrect — actual is ~CAD 145/month** |

Operation is healthy financially. The constraint is revenue, not spend. The Day 29 post cost figure requires correction before distribution.

---

*Report prepared by Copia — koad:io financial entity*
*Working directory: `/home/koad/.copia/`*
*Ledger: `ledger/2026-04.journal`*
*Prior report: `reports/2026-04-day6.md`*
