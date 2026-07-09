---
name: evidence-synthesizer
description: Turn messy source material — issue-tracker tickets, team chat/discussion, support tickets, sales notes, product analytics, specs, docs, product vision — into structured, labeled PMM evidence. Fires on prompts like "synthesize these docs into the context hub," "read these tickets and pull out the product marketing implications," "turn these sales and support notes into customer evidence," "what does our analytics/chat/support data actually tell us," or whenever a product hub has a pile of unprocessed material in inputs/ or connected tools. Requires an existing product hub — run context-intake first if none exists. This does not cover competitor material — that's competitor-discovery and its sequence.
---

# Evidence Synthesizer

Turn raw material from the non-competitor evidence lanes in `CLAUDE.md` (product, team
discussion, customer evidence, market/demand) into hub entries with a confidence and a
source pointer on every claim. This is where "someone said X in a ticket" becomes a
claim other skills can actually build on — or gets explicitly flagged as too weak to.

## Before you start

Confirm a product hub exists. Check `00-index.md`'s Freshness table and the hub's
`inputs/` folder for anything new since the last sync — if key sources have changed,
surface the diff and confirm before treating old entries as still current.

## Sources to pull from

Per `CLAUDE.md`'s evidence lanes — read live via connected tools where available,
otherwise from files the user has placed in `inputs/`:

- **Product**: issue tracker, specs, design docs, vision docs — tickets, epics, roadmap intent
- **Team discussion**: team chat/messaging — decisions, disagreements, open threads
- **Customer evidence**: support desk, sales notes, product analytics — churn reasons, usage, friction
- **Market/demand**: search/SEO tools, social listening — demand signals, category language, sentiment

If a connector isn't available, say so plainly rather than silently skipping the lane —
an unchecked lane is a gap worth naming, not an assumption to make quietly.

## Process

1. **Log every source first.** Before extracting anything, add a row per source to
   `02-evidence-log.md`'s Sources table: source, type, date, pointer, brief note. A claim
   with no corresponding source row isn't traceable — don't extract past this step.
2. **Extract claims, not summaries.** For each source, pull out discrete, checkable
   claims — not a paraphrase of the whole document. Use the format
   `Claim text. [Confidence | src: pointer]`.
3. **Preserve contradictions.** If two sources disagree, log both claims with both
   sources and mark the conflict explicitly — don't average them into one smoothed
   claim, and don't silently prefer the more recent or more senior source without saying
   you did.
4. **Extract the "why," not just the "what," when the source supports it** — e.g. a
   ticket that says a feature shipped is a `Confirmed` fact; a ticket thread's discussion
   of *why* it shipped that way is a separate, usually lower-confidence claim about
   intent. Keep them as separate entries.
5. **Route claims to the right file**, not just the evidence log:
   - Product facts and capabilities → `01-product-truth.md` Validated Truth
   - Our own pricing/packaging facts (plan names, prices, what's included) →
     `06-pricing-packaging.md`'s **Product Packaging** section — this is internal
     evidence, distinct from that file's **Competitor Pricing** section, which is
     `competitor-positioning-pricing`'s to fill
   - Anything about users, buyers, jobs, pains, objections → `03-customer-and-jobs.md`
   - Anything revealing a stakeholder's stance, constraint, or veto power → `11-stakeholders.md`
   - Market/demand signals with no clear home yet → note in `00-index.md` Open Questions
     rather than forcing them into a file where they don't fit
6. **Flag what's still missing.** After synthesis, list what none of the available
   sources answered — these are real gaps, not just unasked questions.

## Rules

- Preserve technical accuracy. Don't simplify a claim in a way an engineer would dispute.
- Never collapse a contradiction into a single confident claim — contradictions are
  signal, not noise to clean up.
- Every claim you write gets both axes: confidence and a checkable source pointer. If you
  can't point to where it came from, it's `Hypothesis`, full stop.
- Distinguish "someone asserted X" from "X is true." A sales call transcript quoting an
  AE's price confirms the AE *said* that price — it doesn't confirm the price is correct.
  Label these as e.g. `Confirmed (as a statement made) | src: ...` so a contradiction
  between a verified fact and a reported utterance doesn't read as two equally solid
  facts.
- If a source has no date, say so explicitly ("date not stated in source") rather than
  inventing one or substituting file metadata.
- Don't re-synthesize a source that's already logged and unchanged since its last pull —
  check the evidence log first.

## Output

Updates: `02-evidence-log.md` (Sources, Extracted Claims), `01-product-truth.md`
(Validated Truth), `06-pricing-packaging.md` (Product Packaging section only),
`03-customer-and-jobs.md`, `11-stakeholders.md` where relevant, `00-index.md` (Open
Questions, Next Best Action, and Freshness rows for every file you touched — last-synced
= today, reflects-source-as-of = the source's own date, or "not stated in source").

End with the single next best action — usually `value-framing` once enough customer
evidence exists, or naming the single highest-value evidence gap to close first if not.
