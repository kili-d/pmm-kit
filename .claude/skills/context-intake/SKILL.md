---
name: context-intake
description: Personalize PMM Kit and/or start a new product's context hub — this is the load-bearing, run-first skill that turns the generic PMM Kit framework into something specific to a real organization and product. Use whenever the context/ folder is empty or missing key files, when starting work on a product that has no hub yet, when the user says things like "set up PMM Kit for my product," "personalize this," "let's start a new product," "onboard this product," or drops docs into an inputs/ folder wanting them turned into usable context, or whenever CLAUDE.md's own instruction to run context-intake first applies. Always run this before product-immersion, evidence-synthesizer, or any other PMM Kit skill on a product that hasn't been through intake yet.
---

# Context Intake

PMM Kit ships with zero domain knowledge on purpose — no company, market, or product is
hardcoded anywhere else in the kit. This skill is what fills that in. It writes the
**context layer** (`context/*.md`, organization-wide, read by every other skill) and
**seeds a product hub** (`/<product-name>/`, one per product). Nothing downstream should
guess at domain, org, or product facts — it should point back here.

## When to run

- `context/` is empty, missing files, or the user says their situation changed
  (reorg, new market, new constraint) — re-run intake rather than letting other skills
  quietly assume stale facts.
- A product has no hub folder yet.
- The user has dropped new documents into a hub's `inputs/` folder and wants them folded
  into context or the hub.

If `context/` already has content, don't re-ask everything — show what's there and ask
only about what's missing, changed, or contradicted by newly uploaded docs.

## Process

### 1. Check current state

Read `context/README.md` and any existing `context/*.md` files. List what exists, what's
missing, and anything that looks stale or contradicted by new inputs. Show this to the
user before asking anything — don't make them repeat what's already on file.

### 2. Ingest uploaded documents first

Before asking questions, check for a hub's `inputs/` folder (or ask where dropped docs
live if none is obvious yet) and read anything there — specs, wiki exports, decks, notes,
PDFs. Extract facts relevant to the context layer and note the source pointer (file name)
for each. This reduces what you need to ask the human directly — don't ask something a
document already answered, just confirm your read of it.

### 3. Run the questionnaire for whatever's still missing

Ask in batched, related groups — not one question at a time. Skip any group fully
answered by ingested documents.

**Organization & product**
- What's the product (and org, if relevant) called, in one sentence — what does it do?
- What domain or market is it in, in your own words? (Don't accept a category label
  without asking what it actually means in practice — categories are a choice made later
  in `positioning-messaging`, not a starting assumption.)
- Is there an existing product line or portfolio this sits in?

**Audience (if known — it's fine if it isn't yet)**
- Any early read on who the user vs. buyer is? Capture it as a labeled `Assumption` if
  it's a deliberate early bet, or mark it open if genuinely unknown — don't guess a persona
  and present it as fact. This goes in the hub's
  `01-product-truth.md` ("who it appears to be for") or `00-index.md` open questions if
  the hub is only just being seeded — audience is product-specific, not organization-wide,
  so it never goes in `context/`.

**Distribution & owned assets**
- What distribution channels or owned assets exist today — sales motion, existing
  customer base, brand portfolio, partners, marketplace presence, SEO footprint,
  community? (This feeds `10-distribution.md` later; get it recorded now while it's easy
  to ask.)

**Constraints**
- Any compliance, legal, brand, or process constraints on what claims can be made?

**Terminology**
- Any internal shorthand, acronyms, or naming conventions worth knowing so later output
  doesn't sound like it came from outside the org?

**Product hub**
- What should this product's hub folder be named? (Check if a hub with that name
  already exists — offer to refresh it instead of starting over. The hub folder name is
  whatever the user wants — it does not need to match the product's actual name.)
- Who should be listed as the hub's owner? Ask directly rather than filling this in from
  session metadata or guessing.

### 4. Write the context layer

Write only the files supported by real answers or ingested documents, to `context/`:
`domain.md`, `organization.md`, `product-line.md`, `channels.md`, `constraints.md`,
`terminology.md`. Every material fact uses the two-axis format from `CLAUDE.md`:
`Claim. [Confidence | prov: <type>: pointer]` — provenance is usually `internal` (the
document name), or `user-interview` for something stated directly in this conversation.
Don't pass off an inference as fact; if something is genuinely unknown, write "Open — not
yet known", or capture a deliberate early read as a labeled `Assumption` traced to its
input — never a bare guess.

### 5. Seed the product hub

Create the hub folder (named whatever the user chose, not necessarily the product's
literal name) at the repo root by copying every file and folder from
`assets/hub-template/` in this skill (the 00-index.md through 13-copy-library.md set,
plus `inputs/` and `assets/{competitor-screenshots,product-screenshots,whiteboards}/`).
In `00-index.md`, fill in the owner, status, product summary, and open questions from
what you just learned. Leave the freshness table exactly as the template has it — every
row blank — since no skill has synced anything yet; there is nothing to fill there at
intake time. If the hub already exists, don't overwrite files with content in them — only
fill gaps.

Don't touch `02-evidence-log.md`, or any hub file besides `00-index.md`. Logging sources
formally (with dated entries and full claim extraction) is `evidence-synthesizer`'s job.
If `inputs/` already holds documents you haven't fully mined, say so in the hand-off
(step 6) so the user knows to run `evidence-synthesizer` next rather than assuming
everything in `inputs/` has been processed just because context-intake touched it.

### 6. Report and hand off

Summarize what was written (which context files, what's still open) and what's in the
new or refreshed hub. End with the single next best action — normally
`product-immersion` (naive first-touch read) or `evidence-synthesizer` (if there's
already a pile of docs/tickets to process), not a menu of options.

## Rules

- Never write a company, market, or product fact into `CLAUDE.md` or any skill file —
  everything specific goes in `context/` or the product hub.
- Never present a guess as fact. Where the domain, primary user, buyer, category, or
  distribution motion isn't known yet, record it as open — or, if it's a deliberate early
  bet worth carrying forward, capture it as a labeled `Assumption` traced to its input.
- `context/`, `inputs/`, and product hubs are local and gitignored by default — don't
  suggest committing them, and never write their contents to a shared system.
- Keep the questionnaire tight. If you can answer a question from an uploaded doc,
  confirm your reading of it instead of asking the human to repeat it.
