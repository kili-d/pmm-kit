---
name: product-immersion
description: Use for a hands-on, first-time-user read of a product, demo, prototype, screenshots, or docs — captured before Product Management framing shapes the story. Fires on prompts like "walk through this product like a customer," "give me product immersion notes from these screenshots," "turn this demo into product truth observations," "what would a new user notice or get confused by," or when following CLAUDE.md's default workflow to step 2 (naive read) for a product hub that hasn't had one yet. Requires an existing product hub — run context-intake first if none exists for this product.
---

# Product Immersion

Act as a naive first-time user working through whatever material you're given — live
product, demo, prototype, screenshots, or docs — not as someone who already knows the
roadmap or intended positioning. The point is to capture confusion, friction, and unclear
value *before* anyone smooths it into a tidy narrative. This pass is deliberately naive;
resist the urge to reconcile what you see with what you already know the product is
"supposed" to be.

## Before you start

Confirm a product hub exists (look for `00-index.md`). If there isn't one, stop and point
to `context-intake` instead of guessing at a domain or product to immerse in.

Read only enough of the hub to know where to look — don't front-load so much context that
you lose the naive vantage point on purpose. Going in without an internalized "official"
answer for what the product is for is the goal, not a gap to fill first.

## Process

1. Walk the actual material in the order a user would encounter it — entry point first,
   then whatever follows. Note what's presented, and what you're asked to do or
   understand, in sequence.
2. As you go, capture:
   - What you assumed the product does at each step, before being told
   - Where you got confused, stuck, or had to guess
   - Where value became clear on its own — or didn't
   - Anything that reads as a capability with no obvious "so what" attached to it
3. If actual screenshot images are available, save them into `assets/product-screenshots/`,
   named descriptively and in the order encountered. If you only have a text description
   of screens (no real image files), skip this — don't fabricate placeholder images.
4. Write the pass into `01-product-truth.md`'s **Naive Read** section as a running,
   first-person account in the order experienced. Mark each notable moment
   `[observation]` (what you actually saw/did) or `[hypothesis]` (what you inferred from
   it) — see CLAUDE.md's two-axis claim rule for the confidence vocabulary this feeds
   into once labeled.
5. Fill in what you can now defend in the **What It Does** and **Who It Appears To Be
   For** tables, each row sourced `product-observation` with an honest confidence label —
   most rows from a single naive pass should land as `Inferred` or `Hypothesis`, not
   `Confirmed`. If a row would otherwise conflate a directly-observed fact (e.g. "the CLI
   asks for a framework choice") with an inferred implication (e.g. "...because it wants
   to optimize the build per framework"), split them into two rows rather than forcing
   one confidence label onto both — the raw observation can be `Confirmed` even when its
   implication is only `Hypothesis`.
6. Add anything only Product, Support, or a real customer could resolve to
   `00-index.md`'s Open Questions — don't quietly resolve it yourself by picking the
   plausible-sounding answer.

## Rules

- Confusion and friction are evidence, not criticism — record them plainly. Don't soften
  or omit a rough edge to be polite about the product; a smoothed-over immersion note is
  worse than no note.
- Don't assume the target customer, buyer, or market category this early. If the material
  seems aimed at someone, write "this reads as if it's for X" and label it `Hypothesis`,
  not fact — that call belongs to evidence and, later, `positioning-messaging`.
- Keep capability separate from value: describe what a feature does, then separately
  whether its value was obvious to you unaided or had to be explained/inferred. A feature
  is not a value proposition.
- This produces raw material for `evidence-synthesizer` and `value-framing` — don't
  polish it into finished messaging or a clean narrative.

## Output

Updates: `01-product-truth.md` (Naive Read, What It Does, Who It Appears To Be For),
`00-index.md` (Open Questions, Next Best Action, and your row in the Freshness table —
last-synced = today, reflects-source-as-of = the date/version of the material you worked
from), plus `assets/product-screenshots/` if real images were provided.

End with the single next best action — usually `evidence-synthesizer`, whether that means
a real pile of docs/tickets or just a handful of known-but-unpulled artifacts this pass
surfaced (a pricing page, a docs section) — or straight to `value-framing` if this pass
plus existing evidence already cover the customer lane well enough.
