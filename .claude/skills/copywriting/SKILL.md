---
name: copywriting
description: Turn an approved positioning statement and messaging house into actual copy — headlines, subheads, taglines, CTAs, opening lines, punch-up edits of existing drafts — at the sentence level. Fires on prompts like "give me headline options," "write a tagline," "punch up this paragraph," "draft CTA copy," "tighten this hero section," or any ad hoc copywriting request. Unlike `campaign-starter`, this is not gated behind full campaign readiness — it can run any time `08-messaging-house.md` (or at minimum `07-positioning.md`) has real content, and it's meant to be invoked repeatedly, not once. Requires an existing product hub; if positioning/messaging house are still empty, it says so and offers clearly-labeled draft copy anyway rather than refusing outright.
---

# Copywriting

The craft layer, not the strategy layer. `messaging-house` decides what gets said and to
whom; this skill gives it voice — rhythm, concision, specificity, punch. It doesn't
invent claims, jobs, or positioning, and it isn't gated the way `campaign-starter` is: use
it any time for a quick headline pass, a tagline option, or tightening a paragraph someone
already drafted.

## Before you start

Read `08-messaging-house.md` for the narrative, pillars, and audience angles this copy
should carry. If it's thin, fall back to `07-positioning.md`. If both are still
template-empty, say so plainly, ask which claim, pillar, or audience this copy is meant
to express — or proceed with an explicit `Hypothesis`-labeled placeholder if the user
wants a draft anyway. Either way, don't manufacture a value proposition that doesn't
exist anywhere in the hub.

## Process

1. **Name the pillar/angle and audience** this request is for, explicitly, before
   writing anything. If the request doesn't map to anything in the messaging house, say
   so — that's a gap for `messaging-house` or `value-framing` to close, not something to
   paper over with a plausible-sounding line.
2. **Generate options, not one answer.** Copywriting is iterative by nature — offer
   several distinct directions (different angles, lengths, or registers: e.g. five
   headline directions, not one "best" headline) rather than a single take presented as
   final.
3. **Trace every option to a real claim.** If the punchiest version of a line depends on
   a claim that isn't substantiated in `02-evidence-log.md`, either mark it inline as
   `Needs-proof` or offer an alternative that doesn't depend on it — don't quietly launder
   an unproven claim into confident prose.
4. **Cut generic marketing language.** If a line could sit on any competitor's homepage
   unchanged, sharpen it until it's specific to what this hub actually established, or
   cut it.
5. **For punch-up requests** (editing existing copy): preserve the underlying claim and
   its confidence label. Tighten language, cut filler, sharpen verbs — don't use an
   editing pass as cover to quietly upgrade a claim's strength.
6. **Save what's reusable.** Append notable options — not every discarded draft — to
   `13-copy-library.md`, tagged with the pillar/audience/asset they're for, so later
   requests (including `campaign-starter`) can draw on them instead of regenerating from
   scratch.

## Rules

- Craft, not strategy — if a request reveals a genuine gap (no pillar covers this angle,
  no audience angle exists for this segment), name the gap and point to `messaging-house`
  or `value-framing` rather than inventing one to fill it.
- Confidence labels stay in the paper trail (`13-copy-library.md`) even when the
  final external-facing copy itself won't carry them.
- Never write copy to a shared system (CMS, ESP, ad platform, deck tool) without
  explicit, specific approval for that exact write, per `CLAUDE.md`'s read/write
  governance — draft locally first, always.
- This skill does not replace `campaign-starter` — it doesn't assemble full assets
  (landing pages, email sequences, one-pagers) or check campaign-level launch
  readiness. It writes the lines; `campaign-starter` assembles them into gated,
  launch-ready packages.

## Output

Returns the requested copy directly in the response. Appends reusable lines to
`13-copy-library.md` with pillar/audience/asset tags. Updates `00-index.md`'s Freshness
row for `13-copy-library.md` only if it changed meaningfully — a one-off request that
produced nothing worth keeping doesn't need a freshness update.

End with the single next best action — usually none needed for a one-off request, or a
pointer to `campaign-starter` if the request was clearly in service of an upcoming
launch.
