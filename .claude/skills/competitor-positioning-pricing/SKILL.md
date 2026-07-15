---
name: competitor-positioning-pricing
description: Analyze a competitor's positioning, messaging, pricing, packaging, claims, proof points, and implied ICP — the third and final competitor pass, after competitor-discovery and competitor-journey-capture. Fires on prompts like "analyze competitor positioning," "compare pricing and packaging for these competitors," "extract messaging patterns from competitor pages," or as the natural follow-up once a competitor's journey has been captured. Requires an existing product hub with a captured journey in 05-journey-teardowns.md for the competitor(s) in question.
---

# Competitor Positioning & Pricing

Analyze what a competitor's own pricing, packaging, and messaging reveal — category
language, implied ICP, proof points they lean on, claims they make. This is the
strategic read that `competitor-journey-capture` deliberately withheld; that pass
recorded what's there, this one interprets what it means.

## Before you start

Read `05-journey-teardowns.md` for the competitor's captured journey and any flags left
for this pass. If no journey exists yet for the competitor you're asked to analyze, run
(or ask for) `competitor-journey-capture` first rather than analyzing from pricing pages
alone — packaging without the surrounding journey context is easy to misread.

## Process

1. **Pricing and packaging**: record plans, price points, what's bundled at each tier,
   and what's gated — with the capture date, since competitor pricing changes. Write to
   `06-pricing-packaging.md`'s **Competitor Pricing** section (the **Product Packaging**
   section in that same file is `evidence-synthesizer`'s territory — our own pricing, not
   theirs; don't touch it here).
2. **Messaging and claims**: pull the actual language a competitor uses — category
   words, headline claims, proof points (customer logos, stats, certifications) they
   lead with. Quote it, don't paraphrase into something more generic.
3. **Category language and implied ICP**: what market category is the competitor
   positioning into, and who does their language suggest they're chasing (company size,
   technical sophistication, budget)? This is inference from evidence — label it as such.
4. **Whitespace**: only call out a gap or opportunity when the evidence actually supports
   it — a missing feature or an unaddressed audience segment you can point to, not a
   vibe. An unsupported whitespace claim is exactly the kind of thing `CLAUDE.md`'s
   claims-substantiation check is meant to catch downstream — don't let it originate here.
5. Log every source (pricing page URL + date, marketing page, etc.) with provenance
   `external` in `02-evidence-log.md`.

## Rules

- Keep this pass separate from journey capture — you're interpreting what the journey
  and pricing pages mean, not re-recording what's on them.
- Every pricing fact needs a capture date; competitor pricing is a moving target and an
  undated price is close to useless six months from now.
- This analysis feeds `positioning-messaging` and `messaging-house` later — it doesn't
  draft our own positioning or messaging house itself. Write findings as competitor
  facts and implications, not as "so here's what we should say."

## Output

Updates: `04-competitor-map.md` (a short pointer added to the competitor's existing row,
with the substantive positioning/ICP/whitespace writeup in a dedicated subsection below
the table — the table's cells are too narrow for real analysis, don't try to cram it in),
`06-pricing-packaging.md` (Competitor Pricing section; its neighboring Packaging
Questions section is shared across skills — add to it, don't treat it as owned by one
pass), `02-evidence-log.md`, `00-index.md` (Freshness rows, Next Best Action).

End with the single next best action — usually the next prioritized competitor still
needing this pass, or `value-framing`/`positioning-messaging` once enough competitors
have been through all three passes to support real positioning work.
