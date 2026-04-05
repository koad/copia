---
date: 2026-04-05
author: copia
type: cost-benefit analysis
status: final
subject: Approved but unactivated subscriptions — activate vs defer vs skip
---

# Subscription Cost/Benefit Analysis — April 2026

Prepared by Copia. This report assesses four approved-but-unactivated subscriptions before koad triggers payment. Total at stake: CAD 73/month (CAD 29 + CAD 23 + CAD 6 + CAD 15). Current committed spend is CAD 140/month (Claude Max). These four would bring April recurring to CAD 213 — within budget, but only worth spending if they unblock real work.

---

## Summary Table

| Subscription         | CAD/mo | Tier          | Activate? |
|----------------------|--------|---------------|-----------|
| Figma Professional   | 29     | DEFER         | No        |
| Runway Gen-4.5       | 23     | SKIP          | No        |
| Brave Search API     | 6      | DEFER         | No        |
| Flux via fal.ai      | 15     | DEFER         | No        |

**Recommendation: Activate none of the four in April.** The team is shipping at pace without any of them. Reserve CAD 73/month for Month 2 or until a concrete blocker surfaces.

---

## 1. Figma Professional — CAD 29/month

### Current alternative
Muse is producing design work entirely in markdown. As of 2026-04-05, she has authored 27+ design briefs covering: homepage wireframes, entity cards, Alice conversation UI, blog layout, trust bond visualization, graduation certificates, MVPZone, Stream PWA, domain skins, the dark passenger extension, and the full koad.sh site redesign. These are delivered as spec documents to Vulcan. Vulcan builds from them. The workflow is functioning.

Muse's design-system directory (`~/.muse/design-system/koad-io-design-system.md`) exists as a markdown document. The entity card and homepage wireframe already shipped as working code via Vulcan (Alice Phase 2A on kingofalldata.com, commit 7d95c39).

### Who it unblocks
Nobody, currently. Muse's output reaches Vulcan as specification. Vulcan implements in code. There is no step in that pipeline that requires a Figma file. If Vulcan were receiving wireframes as Figma links and struggling to interpret them, that would be different. He isn't.

### Priority tier
**DEFER.** When Muse needs to deliver interactive prototypes for stakeholder review, or when the team brings in external collaborators who need Figma access, this becomes relevant. Neither condition is true in April.

### Month 1 ROI
Negligible. Muse can produce the same deliverables in markdown for CAD 0. The value of Figma (collaboration, handoff, prototyping) is only realized when there are external parties to collaborate with. Right now the team is internal and developer-to-developer. The markdown workflow is faster, not slower.

**Hold until:** external collaborators, or a Vulcan request for interactive prototypes over static specs.

---

## 2. Runway Gen-4.5 — CAD 23/month

### Current alternative
Rufus's video format is **terminal-capture throughout**. His production spec (`ENTITY-INTRO-SERIES.md`, `ALICE_PRODUCTION_PLAN.md`) explicitly defines the capture method as asciinema-to-mp4 via `agg`/ffmpeg, or OBS screen capture of a terminal window. The video format is pure terminal: black background, white monospace text, no graphics, no motion design, no generated imagery. The opening and closing cards are static text frames typed live or produced as static PNGs.

Five videos are scripted. None of them call for AI-generated footage.

### Who it unblocks
Nobody in the current production pipeline. Runway generates AI video — cinematic clips, transitions, visual effects. Rufus's content aesthetic is deliberately the opposite: raw, honest, terminal-native. Runway video would be aesthetically wrong for these videos, not just unnecessary.

### Priority tier
**SKIP.** This isn't a deferral — the use case doesn't exist in the current content strategy. If Rufus shifts to produced explainer videos with motion graphics, revisit. That's a Month 2+ strategic decision.

### Month 1 ROI
Zero. No entity has a production workflow that touches AI video generation. The CAD 23/month would sit unused.

**Hold until:** Rufus explicitly plans a production piece that requires generative video, which contradicts his current spec.

---

## 3. Brave Search API — CAD 6/month

### Current alternative
Sibyl has produced 54 research documents without a paid search API. Her research index covers competitive landscape, market signals, sponsor acquisition, inter-agent communications, enterprise adoption barriers, trust bonds technical deep-dives, and content strategy. Faber has written 27 posts pulling from Sibyl's research with no apparent research gaps.

The Exa API is available on free credits for all of April — no decision needed until May.

### Who it unblocks
Faber, marginally. Brave Search API would give Sibyl a real-time web search layer for current events and news hooks. The CAD 6/month is genuinely cheap for what it provides. However: Sibyl has shipped 54 research files, Faber has shipped 27 posts, and neither entity has flagged a blocked research task. The output quality has been sufficient.

### Priority tier
**DEFER.** At CAD 6/month this is nearly negligible, but the principle is the same: activate when there's a concrete need, not preemptively. May is the natural decision point when Exa's free credits expire and the team can evaluate both APIs together.

### Month 1 ROI
Minimal. The research pipeline is running without it. Activating now adds a tool nobody is waiting on.

**Hold until:** May 1 — reassess alongside the Exa paid tier decision (CAD 68/mo). Brave Search at CAD 6 may be the right answer over Exa at CAD 68 depending on May research needs. Evaluate together.

---

## 4. Flux via fal.ai — CAD 15/month (burst capacity)

### Current alternative
No current entity workflow requires image generation. Muse produces design specs in markdown. Faber's content is written posts. Rufus's videos are terminal captures. Mercury distributes text and links. There is no production pipeline today that hands off a prompt to an image generation API.

The CAD 15/month was approved as "burst capacity" — meaning: for occasional use when needed. That occasion hasn't arrived.

### Who it unblocks
Nobody currently. Potential future uses: social media imagery for Mercury's distribution, header images for Faber's blog posts, entity avatar generation. None of these have been requested by any entity or blocked any task.

### Priority tier
**DEFER.** When Mercury needs header images for distributed posts, or when the blog requires imagery, this becomes worth activating. CAD 15/month is low risk, but there's no reason to start the meter before there's a use.

### Month 1 ROI
Zero. No entity is asking for images. Activating now means paying for idle burst capacity.

**Hold until:** Mercury has platform credentials and is distributing content that needs visual assets, OR Faber's blog posts require imagery. Neither condition is met in April.

---

## Financial Impact

### If all four are activated (as ratified):
- April recurring: CAD 213/month
- Reserve remaining: CAD 787 of CAD 1,000 ceiling

### If none are activated (this recommendation):
- April recurring: CAD 140/month (Claude Max only)
- Reserve remaining: CAD 860 of CAD 1,000 ceiling
- Freed-up: CAD 73/month

### What to do with CAD 73 in reserve
Hold it. Month 2 is conditional on April revenue. If no sponsors by April 30, the budget drops to ~CAD 300/month — and that CAD 73 in uncommitted recurring becomes meaningful headroom. Activating subscriptions before they're needed converts reserve into locked spend. Don't do it.

---

## The Honest Assessment

The team shipped:
- 27 design briefs (Muse, markdown)
- 27 posts (Faber)
- 54 research documents (Sibyl)
- 5 video scripts (Rufus)
- Alice Phase 2A on production (Vulcan)
- Trust bond architecture, ICM synthesis, hook fix, governance notes

Total external tooling spend enabling all of this: **CAD 140/month** (Claude Max).

The four pending subscriptions solve problems the team hasn't hit yet. In a self-funding Month 1 with no revenue confirmed, that's reason enough to wait.

**Recommendation:** Revisit all four on May 1 alongside the Exa tier decision and the Month 2 budget review. By then the team will have 30 days of evidence about which tools they actually need.

---

*Report generated by Copia — koad:io CFO entity*
*Working directory: `/home/koad/.copia/`*
*Ledger: `ledger/2026-04.journal`*
