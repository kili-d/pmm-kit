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

- `07-positioning.md` has a chosen point of view with a confidence label, not the blank
  template. An `Assumption`-labeled POV counts — a positioning built on labeled assumptions
  is a valid basis to build from. If it's still empty (no POV chosen at all), say so and
  point back to `positioning-messaging` — don't invent a narrative on a positioning that
  doesn't exist yet.
- `09-value-prop-matrix.md` has at least one claim beyond pure `Unproven` to build a
  pillar from (an `Assumption`-labeled claim counts). If there's genuinely nothing to hang
  a pillar on, say so.

If either check fails, don't draft `08-messaging-house.md`. Say exactly what's missing
and point to `positioning-messaging` or `value-framing` to close it — this is expected
output, not a failure to complete the task.

## Process (once the gate passes)

1. **Draft or refresh the Narrative and Core Value Proposition** in
   `08-messaging-house.md`, derived directly from the positioning statement in
   `07-positioning.md` — don't introduce a new angle on the product here that positioning
   didn't already establish. If `14-strategic-narrative.md` exists with a chosen shift,
   derive the Narrative directly from it — compress the movement story rather than
   inventing a parallel one; if the two would diverge, flag it back to
   `strategic-narrative` instead of silently forking the story.
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
   house must point to a row in `02-evidence-log.md` with its provenance. No provenance =
   cut the claim. A claim resting on an `assumption` ships labeled as such with a
   validation item logged — not cut for lacking customer proof. Comparative claims
   ("faster than X," "the only tool that...") and anything in a regulated market get
   flagged for human legal/PM review explicitly — don't self-clear them.
6. **If refining an existing messaging house** rather than drafting the first one: diff
   against what's already there, call out what changed and why (usually because
   positioning or the value-prop matrix changed upstream), and keep angles that still
   hold rather than rewriting wholesale for its own sake.

## Rules

- Each audience angle must be distinct — reusing one message across audiences with only
  the label changed defeats the point of segmenting at all.
- Never let messaging quality outrun label honesty — a fluent pillar resting on a labeled
  `Assumption` is fine; the same pillar passed off as validated fact is a liability.
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
