---
name: distribution-planner
description: Map every available distribution channel — including owned assets like an existing customer base, brand portfolio, or partner network — and work out how channel realities should change messaging, assets, and launch sequencing. Fires on prompts like "build a GTM distribution plan," "map available channels for this launch," "decide which distribution paths fit this product," or once positioning exists and it's time to figure out how it actually reaches anyone. Requires an existing product hub.
---

# Distribution Planner

Distribution is strategy, not just execution — map it *before* messaging is treated as
final, because the channel changes what the message needs to do. This skill covers the
full channel set an organization actually has, with owned distribution assets treated as
first-class, not an execution footnote.

## Before you start

Read `context/channels.md` (if it exists) for what's already known about available
channels/owned assets from intake, and `11-stakeholders.md` for who owns what. Read
`07-positioning.md` / `08-messaging-house.md` if drafted, so the channel plan connects to
a real message rather than operating in a vacuum — but positioning not being drafted yet
is a normal, expected state to run this skill against, not a blocker: per `CLAUDE.md`,
distribution is meant to be mapped *before* positioning is finalized. Don't wait for it,
and don't invent a message to hang the channel plan on if it isn't there yet.

## Process

1. **Cover the full channel set**: sales, lifecycle/email, SEO, marketplace, partners,
   support, events, community, existing customer touchpoints — plus owned distribution
   assets (a portfolio of brands, a partner network, an existing customer base). Don't
   skip a channel just because it isn't the obviously exciting one — a boring existing
   channel with real reach beats an exciting one that doesn't exist yet.
2. For each channel/asset, record: how it actually works, its strength for this specific
   product (not distribution in general), constraints, and who owns it. An owner-less
   channel is a channel that won't ship anything.
3. **Tie channels to messages and assets.** For each viable channel, name what message
   variant and asset type it needs — a sales deck and a lifecycle email are not the same
   artifact even when they carry the same core positioning.
4. Form a GTM motion hypothesis: which channel(s) plausibly carry the most weight for
   this launch, and why — grounded in the channels that actually exist and have an owner,
   not the ones that would be nice to have.
5. Surface channel-driven stakeholder dependencies (who needs to approve or activate a
   given channel) into `11-stakeholders.md` — don't duplicate the full stakeholder
   analysis here, just the distribution-specific dependencies this pass surfaced.

## Rules

- Owned assets (existing customer base, brand portfolio, partners) are first-class —
  give them the same rigor as paid/earned channels, don't relegate them to a footnote.
- Every channel entry needs an owner and a constraint, not just a description of how the
  channel works in general.
- Don't write `12-campaign-brief.md` — that's `campaign-starter`'s file, generated last
  and gated on the whole hub, not assembled incrementally by earlier skills.

## Output

Updates: `10-distribution.md` (full channel map, owned assets, GTM motion hypothesis),
`11-stakeholders.md` (distribution-driven dependencies only), `00-index.md` (Freshness
rows, Next Best Action).

End with the single next best action — usually `stakeholder-alignment` to work through
the dependencies this pass surfaced, or `campaign-starter` if positioning, value, and
distribution are all in place.
