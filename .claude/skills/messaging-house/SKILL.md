---
name: messaging-house
description: Draft or refine the messaging house — narrative, core value proposition, message hierarchy (pillars), and audience-specific angles — built from an already-drafted positioning statement. Fires on prompts like "build a messaging house," "give me a message hierarchy," "draft audience angles for X," "what's our narrative," or as the natural next step once `positioning-messaging` has produced a real `07-positioning.md`. Also the skill to re-run when positioning changes, or when an existing messaging house needs deepening — proof integration, objection handling, sharper audience angles. Requires an existing product hub with a real (non-template) `07-positioning.md`; will say so and point back to `positioning-messaging` if that's still empty.
---

# Messaging House

Turn an approved positioning statement into a narrative people can actually repeat: the
overarching story, the core value proposition, a small set of prioritized pillars, and
distinct per-audience angles. This is strategy, not sentences — it decides *what* gets
said and to whom. Turning it into actual headlines, taglines, and CTAs is `copywriting`'s
job, not this one.

## Gate check (do this first, every time)

- `07-positioning.md` has a real positioning statement with a confidence label, not the
  blank template. If it's still empty or thin, say so and point back to
  `positioning-messaging` — don't build a narrative on a positioning statement that
  doesn't exist yet.
- `09-value-prop-matrix.md` has at least one claim beyond pure `Unproven` to build a
  pillar from. If every claim is Unproven, say so — a messaging house needs something
  real to hang a pillar on, not a hopeful one.

If either check fails, don't draft `08-messaging-house.md`. Say exactly what's missing
and point to `positioning-messaging` or `value-framing` to close it — this is expected
output, not a failure to complete the task.

## Process (once the gate passes)

1. **Draft or refresh the Narrative and Core Value Proposition** in
   `08-messaging-house.md`, derived directly from the positioning statement in
   `07-positioning.md` — don't introduce a new angle on the product here that positioning
   didn't already establish.
2. **Build the Message Hierarchy**: a small, prioritized set of pillars (not an
   exhaustive list of every feature) — each traced to a specific claim in
   `09-value-prop-matrix.md`. If a tempting pillar has no real claim behind it, leave it
   out and note it as a gap rather than writing it anyway.
3. **Build Audience-Specific Angles** for each audience in `03-customer-and-jobs.md`:
   the angle, why it lands (which job/pain/objection it speaks to), and confidence. Each
   audience's angle must be genuinely distinct — reflecting *that* audience's job and
   objection — not the same message relabeled with a different persona name.
4. For each pillar and angle, name the objection it's meant to defuse and the proof point
   behind it, pulled from `02-evidence-log.md` / `09-value-prop-matrix.md` — don't invent
   a proof point that doesn't exist yet; flag it as a proof gap instead.
5. **Run the claims-substantiation check**: every differentiated claim in the messaging
   house must point to a row in `02-evidence-log.md`. No source = cut the claim or label
   it `Needs-customer-proof`. Comparative claims ("faster than X," "the only tool
   that...") and anything in a regulated market get flagged for human legal/PM review
   explicitly — don't self-clear them.
6. **If refining an existing messaging house** rather than drafting the first one: diff
   against what's already there, call out what changed and why (usually because
   positioning or the value-prop matrix changed upstream), and keep angles that still
   hold rather than rewriting wholesale for its own sake.

## Rules

- Each audience angle must be distinct — reusing one message across audiences with only
  the label changed defeats the point of segmenting at all.
- Never let messaging quality outrun evidence quality — a fluent pillar with no proof
  behind it is a liability, not an asset.
- Market category and the core positioning decision belong to `positioning-messaging` —
  if drafting the narrative surfaces doubt about the category choice, flag it back rather
  than quietly redeciding it here.
- This skill does not write headlines, taglines, or CTAs — that's `copywriting`, and it
  needs this file's pillars and angles as its starting material.

## Output

Updates: `08-messaging-house.md` (only if the gate passes), `00-index.md` (Freshness
rows, Next Best Action, and — if the gate didn't pass — the gap list goes here too).

End with the single next best action — either the specific gap most worth closing next
(if gated), or `copywriting` for ad hoc headline/CTA work, or `distribution-planner` /
`stakeholder-alignment` to keep moving toward `campaign-starter`.
