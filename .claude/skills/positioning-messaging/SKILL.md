---
name: positioning-messaging
description: Draft positioning (Dunford spine) — competitive alternatives, unique attributes, the value they enable, who cares most, and the market category as an explicit decision — from product vision, internal conversations, and external observations. Fires on prompts like "draft positioning from this context hub," "what's our positioning," "help me pick a market category," or as the natural next step once value-framing and competitor passes exist. Requires an existing product hub. Vision-first — it still drafts a point of view when customer evidence is thin, flagging what's an assumption rather than refusing; it stops only when there's genuinely nothing to form a point of view from. Once positioning is drafted, run `messaging-house` next to build the narrative and message hierarchy from it — this skill does not draft the messaging house itself.
---

# Positioning

Draft the product's positioning as a **decision** — a chosen point of view fused from
product vision, internal conversations (vision docs, PRDs, transcripts, decks, Slack,
email), and external observations (competitor plus customer/market research). Positioning
is a bet made with the bravado to pick a unique position, not a report waiting on proof.
Where hard customer/analytics evidence exists, prefer it; where it's absent, form the view
anyway on labeled assumptions and record what would validate them. This skill owns
`07-positioning.md` only; the messaging house (narrative, hierarchy, audience angles) is
`messaging-house`'s job, run right after this one.

## Readiness check (do this first, every time)

The bar is a *chosen point of view*, not accumulated proof. Before drafting, check:

- Is there enough to take a position — a product read (`01-product-truth.md` or a vision
  doc), at least a candidate audience and value (`09-value-prop-matrix.md` /
  `03-customer-and-jobs.md`), and some competitive context (`04-competitor-map.md`, even a
  single reasoned entry)? Thin external evidence is not a blocker — it's a cue to label
  assumptions, not to refuse.
- Do any unresolved `Contradicted` claims bear directly on the positioning decision (e.g.,
  pricing, a core capability)? Note them as validation items so the draft doesn't quietly
  rest on a disputed fact — don't stall on them.

The only reason *not* to draft is that there's genuinely nothing to form a view from — no
vision, no product read, no audience, no competitive context at all. Then say what minimal
input is needed (usually `context-intake` or `product-immersion`) and stop. Lacking
customer proof is **not** such a reason.

## Process (once there's something to position from)

1. **Draft `07-positioning.md`** using the Dunford spine, in order — competitive
   alternatives, unique attributes, the value they enable, who cares most, and the market
   category as an explicit decision (name the assumed category and say why you're choosing
   differently, if you are). Each step cites the hub file it draws from. Where a step rests
   on a bet rather than validated evidence, write the claim and label it `Assumption` with
   its provenance (`assumption -> <internal|external pointer>`) — don't omit it, and don't
   round it up to `Confirmed`.
2. **Attach the assumption set and validation backlog.** List every `Assumption` the
   positioning rests on and, for each, what would validate or falsify it — into
   `00-index.md`'s Validation Backlog. This is what makes shipping-on-assumptions honest:
   the view goes out now, the backlog gets it pressure-tested later.
3. **Check the positioning statement's own claims.** The "unique attributes" and "value"
   steps make differentiated claims — confirm each points to a row in `02-evidence-log.md`
   with its provenance. A claim resting on an assumption ships labeled; an untraceable
   assertion does not ship. Comparative claims ("faster than X," "the only tool that...")
   and anything in a regulated market get flagged for human legal/PM review explicitly —
   don't self-clear them.
4. Prefer the simplest credible story the inputs actually support over a cleverer one they
   don't.

## Rules

- Do hold a view. Refusing to position for lack of customer proof is the old posture and is
  no longer correct — form the best-supported point of view and label what's still a bet.
- Never present an `Assumption` as a `Confirmed`/`Validated` fact — that labeling is the
  whole discipline. A claim passed off as proven is more dangerous than one honestly marked
  a bet.
- Keep technical claims accurate to what `01-product-truth.md` and `02-evidence-log.md`
  actually establish — don't round a capability up to sound more impressive.
- The market category in step 5 of the Dunford spine is a decision, not a default — don't
  inherit whatever category the product happened to launch under without asking whether
  it's still the right one.
- Don't draft `08-messaging-house.md` here, even partially — that's `messaging-house`'s
  job, and it needs a drafted `07-positioning.md` to build from.

## Output

Updates: `07-positioning.md`, `00-index.md` (Freshness rows, the Validation Backlog for the
assumptions the positioning rests on, and Next Best Action).

End with the single next best action — normally `messaging-house` to build the narrative
from the positioning, or the single most load-bearing assumption to validate first if one
is worth pressure-testing before messaging.
