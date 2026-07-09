---
name: value-framing
description: Translate product capabilities into customer jobs, pains, desired outcomes, objections, proof needs, and value propositions — completing the JTBD chain and building the value-proposition matrix. Fires on prompts like "turn these features into customer value," "build a value proposition matrix," "identify customer jobs and proof needs," or once product truth and enough customer evidence exist. Requires an existing product hub with content in 01-product-truth.md and 03-customer-and-jobs.md — run product-immersion and/or evidence-synthesizer first if those are still thin.
---

# Value Framing

A feature is not a value proposition. This skill closes the gap between "what the
product does" and "why a specific audience would actually care" — completing the JTBD
chain per audience and building the value-proposition matrix that `positioning-messaging`
will later draw on.

## Before you start

Read `01-product-truth.md` (What It Does) and `03-customer-and-jobs.md` (Candidate
Audiences, JTBD Chain so far). If both are still mostly empty templates, say so and
suggest `product-immersion` and/or `evidence-synthesizer` first — value framing on top of
naive-only or evidence-thin input just produces confident-sounding guesses.

## Process

1. **Complete the JTBD chain** in `03-customer-and-jobs.md` for each audience with real
   support behind it — evidenced at `Inferred` or better, not a naive-read `Hypothesis`
   alone. For audiences that are still pure hypothesis, note them and say why you didn't
   build a full chain rather than inventing pains nobody's actually stated. For each
   audience you do chain: job → pain/constraint → desired outcome → objection → proof
   point needed → value proposition. A chain missing a proof point is a value claim with
   nothing behind it — flag it rather than leaving the cell blank and moving on.
2. **Make the audience explicit for every value claim.** "Saves time" is not a value
   proposition; "saves a 3-person agency the 2 hours/week they currently spend manually
   checking deploy status across client sites" is closer. If you can't name who benefits
   and why they specifically care, the claim isn't ready.
3. **Separate capability from value** for each row: what the feature *does*
   (capability, from `01-product-truth.md`) vs. what outcome it produces for this
   specific audience (value) vs. what would prove it (proof). Three distinct things, three
   distinct columns in `09-value-prop-matrix.md` — don't collapse them.
4. **Grade honestly.** A claim only earns Strongest with all three: an evidenced
   audience, a confirmed (not just plausible) pain, and proof that already exists —
   "a proof point would be easy to get" doesn't count, that's a Proof Gap, not proof.
   Everything else is Weak or Unproven; say which link is missing. It's normal, maybe
   even expected, for a hub to have zero Strongest claims early on — that's real
   information, not a failed pass. A weak claim isn't a failure to hide — it's exactly
   the kind of gap this hub exists to surface before it becomes a promise
   `campaign-starter` writes down and someone has to defend.
   If a "capability" is actually broken or non-functional (visible but doesn't work,
   promises something it doesn't deliver), don't force it into a value row at all — flag
   it directly as a risk in the matrix's notes; a non-functional feature has no value
   translation, only a liability one.
5. List **Proof Gaps** explicitly — value claims that would be strong if only there were
   evidence for them. This is a direct feed for what `evidence-synthesizer` or a human
   should go find next.

## Rules

- Every value proposition needs a named audience, a real pain/job it addresses, and a
  proof point (existing or needed) — three-out-of-three, not two.
- Don't polish a weak claim into something that reads stronger than the evidence
  supports. Mark it weak and say why.
- Capability language ("supports X," "includes Y") stays out of the Value column — that's
  what the Feature/Capability column is for.

## Output

Updates: `03-customer-and-jobs.md` (JTBD Chain), `09-value-prop-matrix.md` (full matrix,
Strongest/Weak claims, Proof Gaps), `00-index.md` (Freshness rows, Next Best Action).

End with the single next best action — usually `positioning-messaging` once the matrix
has enough strong, proof-backed claims to build a narrative on, or naming the specific
proof gap most worth closing first if not.
