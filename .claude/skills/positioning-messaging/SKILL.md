---
name: positioning-messaging
description: Draft positioning (Dunford spine) — competitive alternatives, unique attributes, the value they enable, who cares most, and the market category as an explicit decision — only once product, customer, and competitor evidence actually supports it. Fires on prompts like "draft positioning from this context hub," "what's our positioning," "help me pick a market category," or as the natural next step once value-framing and enough competitor passes exist. Requires an existing product hub — this is a late-stage skill and will refuse to produce a positioning statement if the hub isn't ready yet, telling you what's missing instead. Once positioning is drafted, run `messaging-house` next to build the narrative and message hierarchy from it — this skill does not draft the messaging house itself.
---

# Positioning

Draft the product's positioning — but only from real evidence. This is the skill
CLAUDE.md means when it says "don't jump to campaign work": if the hub can't back a
claim, this skill's job is to say so and produce a gap list, not to paper over it with
confident-sounding copy. It owns `07-positioning.md` only; the messaging house
(narrative, hierarchy, audience angles) is `messaging-house`'s job, run right after this
one.

## Gate check (do this first, every time)

Before drafting anything, check whether the hub actually supports it:

- `09-value-prop-matrix.md` — is there at least one Strongest value claim (evidenced
  audience + confirmed pain + existing proof)? If every claim is Weak/Unproven, say so.
- `04-competitor-map.md` / `06-pricing-packaging.md` / `05-journey-teardowns.md` — has at
  least one High-priority competitor been through all three competitor passes? (One is
  the bar for a first positioning draft, not all of them — if several tie at High
  priority, one fully worked is enough to pass this check, though say so explicitly
  rather than silently treating thin coverage as complete.)
- `02-evidence-log.md` — are there unresolved `Contradicted` claims that bear directly on
  a positioning decision (e.g., pricing, a core capability)?

If the answer to any of these is "no" or "not really," **don't draft the positioning
statement or messaging house.** Instead, produce a clear gap list and validation agenda:
what's missing, why it blocks positioning, and what would resolve it. This is a legitimate
and expected output of this skill, not a failure to complete the task — a simple honest
"not ready yet, here's what's blocking it" beats a fluent positioning statement built on
sand.

If the hub genuinely does support it, proceed.

## Process (once the gate passes)

1. **Draft `07-positioning.md`** using the Dunford spine, in order — competitive
   alternatives, unique attributes, the value they enable, who cares most, and the market
   category as an explicit decision (name the assumed category and say why you're
   choosing differently, if you are). Each step should cite the hub file it draws from.
2. **Check the positioning statement's own claims**: the "unique attributes" and "value"
   steps make differentiated claims — confirm each points to a row in
   `02-evidence-log.md`. No source = cut the claim or label it `Needs-customer-proof`.
   Comparative claims ("faster than X," "the only tool that...") and anything in a
   regulated market get flagged for human legal/PM review explicitly — don't self-clear
   them.
3. Prefer the simplest credible story the evidence actually supports over a cleverer one
   it doesn't.

## Rules

- Never let the positioning statement outrun evidence quality — a well-written
  unsubstantiated claim is more dangerous than an unwritten one.
- Keep technical claims accurate to what `01-product-truth.md` and `02-evidence-log.md`
  actually establish — don't round a capability up to sound more impressive.
- The market category in step 5 of the Dunford spine is a decision, not a default —
  don't inherit whatever category the product happened to launch under without asking
  whether it's still the right one.
- Don't draft `08-messaging-house.md` here, even partially — that's `messaging-house`'s
  job, and it needs a finished, gate-passed `07-positioning.md` to build from.

## Output

Updates: `07-positioning.md` (only if the gate passes), `00-index.md` (Freshness rows,
Next Best Action, and — if the gate didn't pass — the gap list and validation agenda go
here too, since that's the hub's shared "what's missing" surface).

End with the single next best action — either the specific gap most worth closing next
(if gated), or `messaging-house` once positioning is drafted.
