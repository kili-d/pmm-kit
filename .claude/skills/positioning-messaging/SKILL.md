---
name: positioning-messaging
description: Draft positioning (Dunford spine) and the messaging house — narrative, message hierarchy, audience angles — only once product, customer, and competitor evidence actually supports it. Fires on prompts like "build a messaging house," "draft positioning from this context hub," "create audience-specific messaging," "what's our positioning," or as the natural next step once value-framing and enough competitor passes exist. Requires an existing product hub — this is a late-stage skill and will refuse to produce polished messaging if the hub isn't ready yet, telling you what's missing instead.
---

# Positioning & Messaging

Draft the product's positioning and messaging house — but only from real evidence. This
is the skill CLAUDE.md means when it says "don't jump to campaign work": if the hub can't
back a claim, this skill's job is to say so and produce a gap list, not to paper over it
with confident-sounding copy.

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
2. **Draft `08-messaging-house.md`** from the positioning: narrative, core value
   proposition, message hierarchy (pillars), audience-specific angles. Every message
   traces to a Strongest claim in `09-value-prop-matrix.md` — don't introduce a new claim
   here that wasn't already substantiated upstream.
3. **Run the claims-substantiation check**: for every differentiated claim in the
   messaging house, confirm it points to a row in `02-evidence-log.md`. No source = cut
   the claim or label it `Needs-customer-proof`. Comparative claims ("faster than X,"
   "the only tool that...") and anything in a regulated market get flagged for human
   legal/PM review explicitly — don't self-clear them.
4. Prefer the simplest credible story the evidence actually supports over a cleverer one
   it doesn't.

## Rules

- Never let messaging quality outrun evidence quality — a well-written unsubstantiated
  claim is more dangerous than an unwritten one.
- Keep technical claims accurate to what `01-product-truth.md` and `02-evidence-log.md`
  actually establish — don't round a capability up to sound more impressive.
- The market category in step 5 of the Dunford spine is a decision, not a default —
  don't inherit whatever category the product happened to launch under without asking
  whether it's still the right one.

## Output

Updates: `07-positioning.md`, `08-messaging-house.md` (both only if the gate passes),
`00-index.md` (Freshness rows, Next Best Action, and — if the gate didn't pass — the gap
list and validation agenda go here too, since that's the hub's shared "what's missing"
surface).

End with the single next best action — either the specific gap most worth closing next
(if gated), or `distribution-planner`/`stakeholder-alignment` once positioning is drafted.
