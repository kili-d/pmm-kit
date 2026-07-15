---
name: competitor-journey-capture
description: Capture a competitor's customer journey sequentially — what a prospect actually sees and experiences, screen by screen — before any strategic positioning analysis. Second of three competitor passes (after competitor-discovery, before competitor-positioning-pricing). Fires on prompts like "capture the competitor journey for X," "take me through Y's signup and buying flow," "organize these competitor screenshots into a sequence," or when following up on competitor-discovery's prioritized list. Requires an existing product hub with prioritized competitors in 04-competitor-map.md.
---

# Competitor Journey Capture

Walk a prioritized competitor's actual journey — landing page, signup, onboarding,
pricing, whatever a real prospect would move through — in order, and record what's
there. This is observation, not analysis: save the strategic reading (what it implies,
where the whitespace is) for `competitor-positioning-pricing`.

## Before you start

Check `04-competitor-map.md` for which competitors were prioritized by
`competitor-discovery` and why. If asked to capture a journey for something not on that
list or not prioritized, do it, but note the gap — either discovery missed it or this
request is jumping ahead of the prioritization.

## Process

1. Walk the journey in the order a real prospect would encounter it — don't sample pages
   out of sequence. If you have live browsing/screenshot tools, use them; otherwise work
   from whatever screenshots, recordings, or descriptions the user provides.
2. For each step, record: entry point/page, its apparent purpose, the core message shown,
   the CTA, and any friction (confusing copy, unexpected paywalls, dead ends) — the same
   discipline `product-immersion` applies to your own product, applied to theirs.
3. Save real screenshots into `assets/competitor-screenshots/`, organized by competitor
   and date. If no real images are available (text descriptions only), don't fabricate
   placeholder images — write "no screenshots (text-described only)" in the Journey
   Capture Index's screenshot-folder cell instead of leaving it ambiguously blank.
   Source each step with provenance `external` — `external: competitor journey (live
   browsing)` when you actually browsed it yourself, or `external: competitor journey
   (text description)` when working from a description someone else gave you — the latter
   is inherently a step further from the thing itself and should read that way in
   confidence, not be written as if verified firsthand.
4. If the user wants a whiteboard-ready sequence, build it from the same step data and
   save the export/link in `assets/whiteboards/`.
5. Update the Journey Capture Index in `05-journey-teardowns.md` and log the journey as a
   source in `02-evidence-log.md` (it's evidence, with a date and a pointer to where the
   screenshots live).

## Rules

- Capture in order. A journey summarized out of sequence loses the thing that makes it
  useful — what a prospect experiences first shapes everything after.
- Keep this pass to observation. If something clearly implies a strategic conclusion,
  note it as a flag for `competitor-positioning-pricing` rather than writing the
  conclusion here.
- Organize raw screenshots by competitor and date so a later pass (or a human) can find
  the source of any specific claim.

## Output

Updates: `05-journey-teardowns.md` (Journey Capture Index, Teardown per competitor),
`assets/competitor-screenshots/`, `assets/whiteboards/` if applicable, `02-evidence-log.md`,
`00-index.md` (Freshness row, Next Best Action).

End with the single next best action — usually `competitor-positioning-pricing` on the
same competitor(s) now that their journey is captured, or which competitor to capture
next from the prioritized list. If the hub already has a more urgent unrelated open item
(check `00-index.md`'s existing Next Best Action before overwriting it), name that
instead — don't let this pass's own follow-up bump a genuinely higher-priority item just
because it's the one you just worked on.
