---
date: 2026-04-05
period: April 2026 (Day 6 elapsed / "Day 37" session marker)
author: copia
type: checkpoint
prior_report: reports/2026-04-05-day30-budget-report.md
status: provisional — Anthropic charges unconfirmed pending koad review of billing portal
---

# Day 37 Budget Checkpoint — April 2026

Prepared by Copia. Working directory: `/home/koad/.copia/`
Ledger source: `ledger/2026-04.journal`

Note on "Day 37": Session labels reflect internal workload intensity milestones, not elapsed calendar days. Operation began 2026-03-30. Actual elapsed time as of this report is 6 days. The "Day 37" marker indicates the volume of work sessions and parallel agent operations completed, not a 37-day period. All financial data covers the period 2026-03-30 through 2026-04-05.

---

## 1. Budget Status Table

| Metric                                       | Amount (CAD)   |
|----------------------------------------------|----------------|
| Claude Max 5x (flat monthly)                 | 140.00         |
| Electricity — thinker (estimated)            | ~4.00          |
| Approved unactivated subscriptions           | 73.00          |
| **Total committed if all activate**          | **~217.00**    |
| April ceiling (ratified 2026-04-04)          | 1,000.00       |
| **Reserve remaining (worst case)**           | **~783.00**    |
| **% of ceiling consumed (worst case)**       | **~21.7%**     |
| Revenue to date                              | 0.00           |
| LangSmith                                    | Not in use     |
| Per-token API charges                        | None — Max 5x flat rate |

**Status: WITHIN BUDGET. No threshold alerts triggered.**

---

## 2. The Flat-Rate Insight — Why Parallel Agent Volume Doesn't Move the Needle

This checkpoint was requested specifically in the context of the most intensive parallel agent workload to date. Days 31–37 session work includes:

- Parallel invocations of Faber, Sibyl, Mercury, Veritas, Muse, Rufus, Chiron, Vulcan, and Juno simultaneously
- Multiple content pieces produced: Day 6 content, PRIMER.md post, Day 7 video script, curriculum authoring, distribution plans
- Governance resolution (koad/juno#52, #53, #56 partial)
- Hook architecture work, signed code block implementation
- ICM paper synthesis, Alice Phase 2A deployment

**Financial impact of all of the above: CAD 0.00 in additional charges.**

Claude Max 5x is a flat subscription. The ceiling is per-month, not per-session, per-entity, or per-token. No matter how many parallel agent sessions ran during Days 31–37, the Anthropic line item stays at CAD 140/month. There is no usage meter being incremented. There is no burst charge. There is no per-seat fee for running 15 entities under one subscription.

The concern this checkpoint addresses — "we've run a lot of sessions, are we burning budget?" — does not apply to flat-rate subscription infrastructure. The operational risk is not overspend; it is subscription continuation (i.e., revenue to fund Month 2).

---

## 3. Cost Items to Note

### Active charges (provisional, as of last confirmed state)

| Item                        | CAD/month | Status         |
|-----------------------------|-----------|----------------|
| Claude Max 5x               | 140.00    | Running        |
| Electricity — thinker       | ~4.00     | Estimated      |
| dotsh VPS (Vultr Toronto)   | Unknown   | Not in ledger  |

### Approved but unactivated

| Service             | CAD/month | Status                  |
|---------------------|-----------|-------------------------|
| Figma Professional  | 29.00     | Approved, not started   |
| Runway Gen-4.5      | 23.00     | Approved, not started   |
| Brave Search API    | 6.00      | Approved, not started   |
| Flux via fal.ai     | 15.00     | Approved (burst/usage)  |
| Exa API             | 0.00      | Free credits April      |
| **Subtotal**        | **73.00** |                         |

### Not in use / confirmed zero

| Item                | Status                          |
|---------------------|---------------------------------|
| LangSmith           | Not provisioned, not in use     |
| X API v2            | Deferred — stage-and-submit path active |
| Perplexity API      | Deferred                        |
| Any inference APIs  | No separate API key usage detected |

The Day 30 report flagged a concern about the Faber Day 29 post citing "$24/month" as the operational cost. That figure remains incorrect — the actual commitment is ~CAD 144/month (Claude Max + electricity). That post has not yet been distributed and the correction is still pending before Mercury pushes it.

---

## 4. April Projection (Updated Through Day 37 Session)

No new charges have been incurred since the Day 30 report. The projection is unchanged.

**Scenario A: Subscriptions remain deactivated (current trajectory)**

| Item                        | CAD (full month) |
|-----------------------------|-----------------|
| Claude Max 5x               | 140.00          |
| Electricity                 | ~4.00           |
| dotsh VPS (unknown)         | TBD             |
| **April projected total**   | **~144.00+**    |
| April ceiling               | 1,000.00        |
| **% of ceiling**            | **~14.4%+**     |

**Scenario B: All approved subscriptions activate**

| Item                        | CAD (full month) |
|-----------------------------|-----------------|
| Claude Max 5x               | 140.00          |
| Figma + Runway + Brave + Flux | 73.00          |
| Electricity                 | ~4.00           |
| **April projected total**   | **~217.00**     |
| **% of ceiling**            | **~21.7%**      |

Under both scenarios, April ends substantially under ceiling. Budget is not the operational constraint.

---

## 5. Month 2 Decision Point

Revenue position as of Day 37: **CAD 0.00**

The May ceiling decision is approaching. The conditional framework from the ratified budget stands:

| April revenue outcome        | May ceiling          |
|------------------------------|----------------------|
| 0 sponsors (current path)    | ~CAD 300 (Claude Max + essentials only) |
| 1–3 sponsors                 | Maintain CAD 1,000   |
| 5+ sponsors                  | Expand to CAD 1,500  |

The critical path item blocking revenue: Alice PR (koad/kingofalldata-dot-com#1) unmerged → Mercury distribution blocked → first sponsor acquisition delayed. This is not a Copia action item. Flagged for koad's attention.

If the Alice PR is not merged by approximately 2026-04-20, the realistic outcome is: May operates at the reduced ~CAD 300 ceiling. Claude Max continues; discretionary tools (Figma, Runway, Flux) are suspended.

---

## 6. Threshold Alert Status

Per the ratified budget rules:

| Threshold    | Amount (CAD) | Triggered? |
|--------------|--------------|------------|
| 50% warning  | 500          | No         |
| 80% alert    | 800          | No         |
| 100% ceiling | 1,000        | No         |

No alerts to issue. Operation is healthy.

---

## Summary

| Metric                              | Value          |
|-------------------------------------|----------------|
| Actual spend (provisional)          | CAD ~144.00    |
| Committed if all subscriptions live | CAD ~217.00    |
| April ceiling                       | CAD 1,000.00   |
| Reserve remaining (worst case)      | CAD ~783.00    |
| % of ceiling consumed (worst case)  | ~21.7%         |
| Revenue to date                     | CAD 0.00       |
| LangSmith                           | Not in use     |
| Per-token charges from parallel ops | None           |
| Session volume financial impact     | Zero (flat rate) |
| Month 2 risk                        | Revenue, not spend |

The Days 31–37 parallel agent workload — the most intensive to date — produced zero incremental cost. Claude Max 5x absorbs unlimited session volume at a fixed monthly fee. April is tracking at approximately 14–22% of ceiling depending on whether deferred subscriptions are activated.

The financial health of this operation is not threatened by operational intensity. It is conditional on revenue. The first sponsor is the next meaningful financial event.

---

*Report prepared by Copia — koad:io financial entity*
*Working directory: `/home/koad/.copia/`*
*Ledger: `ledger/2026-04.journal`*
*Prior reports: `reports/2026-04-day6.md`, `reports/2026-04-05-day30-budget-report.md`*
