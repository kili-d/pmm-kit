---
name: campaign-starter
description: Generate campaign and launch starter assets — campaign brief, landing page outline, email copy, sales one-pager, FAQ, social copy — from a hub that's actually ready for it. Fires on prompts like "create a campaign brief," "generate starter launch assets," "draft a sales one-pager and FAQ," or "let's put together launch copy." Deliberately the least powerful and most gated skill in PMM Kit — runs last, and refuses to produce polished launch assets on a hub that isn't ready, telling you what's missing instead. Requires an existing product hub.
---

# Campaign Starter

Generate launch-ready starter assets — but only from a hub that has actually earned it.
This is deliberately the least powerful skill here: it doesn't do strategic work itself,
it assembles assets from positioning and messaging that other skills already
substantiated. If that groundwork isn't real yet, this skill's job is to say so, not to
paper over the gap with fluent-sounding launch copy.

## Gate check (do this first, every time — do not skip even if asked to hurry)

Refuse to draft `12-campaign-brief.md` or any launch asset unless all of these hold:

- `07-positioning.md` has real content, not the empty template — a positioning
  statement with a confidence label, not blanks.
- `08-messaging-house.md` has a narrative and message hierarchy with claims that passed
  the claims-substantiation check (each traces to `02-evidence-log.md`, none left
  unlabeled as `Needs-customer-proof` without you seeing it).
- No unresolved `Contradicted` claim in `02-evidence-log.md` touches the campaign's core
  message (e.g., don't build a price-forward campaign on a disputed price).
- `10-distribution.md` names at least one channel with a real owner — a campaign with no
  channel to run in isn't ready, it's a hypothesis.

If any of these fail, **do not draft launch assets.** Say exactly which gate failed and
what closing it requires, same as `positioning-messaging`'s gate — this is expected,
sober output, not a refusal to help. Point back to whichever skill would close the gap
(`positioning-messaging`, `evidence-synthesizer`, `stakeholder-alignment`,
`distribution-planner`).

## Process (once the gate passes)

1. Draft `12-campaign-brief.md`: objective, audience, core message, supporting messages,
   offer/CTA, distribution plan — each pulled from the hub, not invented fresh. Cite
   which hub file backs each section.
2. From the brief, draft whichever starter assets were actually requested (landing page
   outline, email copy, sales one-pager, FAQ, social copy) as separate files or sections —
   practical drafts a real team can adapt, not generic launch-copy filler.
3. **Preserve uncertainty labels in the output itself.** If a supporting message is
   marked `Needs-customer-proof` upstream, don't launder it into confident copy here —
   either leave it out of customer-facing drafts or mark it inline as needing sign-off
   before use.
4. List open risks/approvals needed at the end of `12-campaign-brief.md` — anything a
   stakeholder still needs to clear per `11-stakeholders.md`.

## Rules

- The hub is the source of truth. Don't introduce a new claim, feature framing, or value
  proposition here that didn't already exist upstream — this skill assembles, it doesn't
  invent.
- Never write these assets to a shared system (wiki, CMS, ESP, deck tool) without
  explicit, specific approval for that exact write — draft locally first, always, per
  `CLAUDE.md`'s read/write governance.
- Avoid generic launch copy — if a sentence could describe any product's launch, cut it
  or make it specific to what this hub actually established.

## Output

If the gate passes: creates/updates `12-campaign-brief.md`, plus any specifically
requested starter assets (as new files alongside the brief, or noted inline if short).

If the gate fails: leave `12-campaign-brief.md` untouched (still its empty template) —
don't stamp a partial or "gated" note into it. Record the gate check and what's missing
in `00-index.md` instead, same pattern `positioning-messaging` uses.

Either way, update `00-index.md` (Freshness row, Next Best Action).

End with the single next best action — the specific gap to close if gated, or what
approval/review the drafted assets need before anything goes out.
