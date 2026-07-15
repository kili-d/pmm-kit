---
name: competitor-discovery
description: Find and categorize competitors and alternatives for a product — the first of three competitor passes (discovery, then journey capture, then positioning/pricing; run in that order, don't skip ahead). Fires on prompts like "find competitors for this product," "map the competitive landscape," "who else would a customer compare us against," or when CLAUDE.md's default workflow reaches its competitor step. Requires an existing product hub — run context-intake first if none exists.
---

# Competitor Discovery

Find who a customer would actually weigh against this product — not just the obvious
direct competitors. The output prioritizes which competitors deserve a full journey
capture and positioning/pricing pass next; don't do that deeper work here, this pass is
breadth, not depth.

## Before you start

Read `01-product-truth.md` and `03-customer-and-jobs.md` for who the product is for and
what job it does — competitors only make sense relative to a job, not a product category
in isolation.

Use live web search when it's available — this pass shouldn't rely purely on training
data for who's currently in the market, what they cost, or what they offer. If search
isn't available, say so and mark entries accordingly rather than presenting recalled
knowledge as freshly verified.

## Process

1. **Cover all four categories**, not just the obvious one:
   - Direct competitors — solve a similar problem in a similar way
   - Indirect competitors — solve the same job differently
   - Substitute workflows — manual workarounds, spreadsheets, scripts, agencies, generic
     tools bent to the purpose
   - Do nothing — the status quo a customer may simply keep
2. For each entry, write **why it matters** — what job or audience segment it competes
   for, not just that it exists. A competitor list without a "why" is a name-drop, not
   analysis.
3. **Prioritize** which competitors warrant a full `competitor-journey-capture` and
   `competitor-positioning-pricing` pass — not everything found here needs deep analysis.
   Prioritize by whichever combination of reach, direct overlap with the target audience,
   or being reflexively named by prospects/customers signals the most decision impact.
   Use `Priority: High | Medium | Low`. If nothing in the hub's existing evidence shows a
   real customer or prospect naming a competitor, don't wait for that signal to
   prioritize — rank by audience overlap and reach instead, and say plainly that the
   ranking is category-reasoned rather than customer-confirmed.
4. Log where each competitor came from (a customer mentioned it, a search, a category
   listing) as a source with provenance `external` in `02-evidence-log.md` — competitor
   existence is a claim like any other.

## Rules

- Don't stop at the first few obvious direct competitors — the substitute-workflow and
  do-nothing categories are usually where the real, harder-to-message competition lives.
- Every competitor entry needs a reason it matters, not just a name and URL.
- Mark confidence honestly: a competitor confirmed by multiple customer mentions is
  different from one you found by category-browsing and are guessing is relevant.

## Output

Updates: `04-competitor-map.md` (Competitor Categories, Competitor List with Source and
Priority columns filled in), `02-evidence-log.md`, `00-index.md` (Freshness row, and
Next Best Action if this pass changes what the hub should do next).

End with the single next best action: which prioritized competitor(s) should go through
`competitor-journey-capture` first, or a note that discovery turned up too little to
prioritize yet and more evidence is needed.
