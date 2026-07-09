# Context layer

This folder holds your personalization for PMM Kit — the facts that turn the generic
framework in `CLAUDE.md` into something specific to you and your product. It's written
once by the `context-intake` skill (and refreshed whenever your situation changes), then
read by every other skill.

Everything in here except this file is gitignored — it's expected to contain real
organization, product, and market detail that shouldn't ship with the public framework.

## Files `context-intake` writes here

- `domain.md` — the market/technical domain, in your own terms
- `organization.md` — org name, structure, relevant teams, who you work with
- `product-line.md` — the product(s) in scope and how they relate to each other
- `channels.md` — distribution channels and owned assets actually available to you
- `constraints.md` — compliance, brand, legal, or process constraints that shape claims
- `terminology.md` — internal shorthand, acronyms, naming conventions worth knowing

Not every file will exist for every setup — `context-intake` only writes what your
answers and uploaded docs actually support, and labels anything inferred rather than
stated outright.

## Getting started

Run `context-intake` (or just start working — `CLAUDE.md` will prompt you to run it if
this folder is empty). Drop any docs you want ingested — specs, wikis exports, decks,
notes — into a product's `inputs/` folder first; `context-intake` will read them.
