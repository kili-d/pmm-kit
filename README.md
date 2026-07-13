# PMM Kit

A technical product marketing skill set for tools like Claude Code and Codex.
It takes you from raw product evidence to defensible positioning and launch-ready assets
— with every material claim carrying a confidence label and a checkable source, never a
guess dressed up as fact.

PMM Kit ships with **zero domain knowledge**. It doesn't know your company, your product,
or your market until you tell it. That's deliberate: the framework is generic and safe to
share; your product's reality lives in a separate layer that never leaves your machine
unless you decide otherwise.

## What's actually in here

- **`CLAUDE.md`** — the orchestrator. Loaded every session. Defines the two-axis claim
  discipline (`[Confidence | src: pointer]`), the evidence-hub structure, the positioning
  framework (April Dunford's spine + Jobs-to-be-Done), and which skill runs when.
- **`.claude/skills/`** — ten skills that do the actual work, run roughly in this order:

  | Skill | What it does |
  |---|---|
  | `context-intake` | Runs first. Personalizes the kit and seeds a product hub. |
  | `product-immersion` | Naive, hands-on first read of the product, before PM framing. |
  | `evidence-synthesizer` | Turns tickets, chat, support, sales notes, docs into labeled evidence. |
  | `competitor-discovery` | Finds direct, indirect, substitute, and "do nothing" alternatives. |
  | `competitor-journey-capture` | Records a competitor's actual signup/buying flow, screen by screen. |
  | `competitor-positioning-pricing` | Analyzes competitor messaging, pricing, packaging, ICP signals. |
  | `value-framing` | Turns features into JTBD chains and a graded value-proposition matrix. |
  | `positioning-messaging` | Drafts positioning (Dunford spine) and the messaging house — only once the evidence supports it. |
  | `distribution-planner` | Maps every channel, including owned assets, before messaging is final. |
  | `stakeholder-alignment` | Who can approve, block, dilute, or accelerate — and what they need to believe. |
  | `campaign-starter` | Least powerful skill by design. Assembles launch assets from an approved hub — or refuses and tells you what's missing. |

That's the whole kit. It's meant to stay this small — new skills get added only when a
real, recurring gap shows up, not by default.

## The split that makes this shareable

Two things never leave your machine unless you explicitly commit them:

- **`context/`** — your organization, product line, channels, constraints, terminology.
  Written once by `context-intake`, read by everything else.
- **Product hubs** (`/<product-name>/`) — the evidence log, competitor research,
  positioning drafts, everything specific to one product you're working on.

The repo's `.gitignore` enforces this with an allow-list: everything is ignored by
default except `CLAUDE.md`, `README.md`, `.claude/skills/`, and `context/README.md`. A
new product hub folder needs nothing added to `.gitignore` — it's private the moment it's
created. Only the framework — this file, `CLAUDE.md`, and the skills — is meant to be
shared or published.

## Getting started

1. **Clone this repo** (or copy `CLAUDE.md` + `.claude/skills/` into your own project —
   PMM Kit doesn't need to own the whole repo).
2. **Open it in Claude Code.** `CLAUDE.md` loads automatically.
3. **Run `context-intake`** — either just start talking about your product (`CLAUDE.md`
   will prompt you to run it if `context/` is empty), or ask for it directly: *"set up
   PMM Kit for [product]."* It'll ask a short questionnaire and read anything you drop
   into a hub's `inputs/` folder first, so it only asks what a document hasn't already
   answered.
4. **Drop source material into `inputs/`** as you go — specs, tickets exports, sales
   notes, support threads, competitor pricing pages, anything raw. `evidence-synthesizer`
   and `competitor-*` skills read from there when there's no live tool connection.
5. **Follow the workflow.** `CLAUDE.md` orchestrates the order; you don't need to
   memorize the sequence — just say what you want ("find competitors," "build a value
   prop matrix," "draft positioning") and the right skill fires.
6. **Optional: a personal `CLAUDE.local.md`.** If you have preferences or shorthand
   that are yours alone (not shared product context), Claude Code will pick up a
   `CLAUDE.local.md` in the repo root automatically. It's covered by the same
   `.gitignore` allow-list, so it never gets committed.

## Why some skills say no

Two skills — `positioning-messaging` and `campaign-starter` — run a gate check before
producing anything, every time, even under time pressure. If the hub doesn't have a real
value claim, an unresolved contradiction bears on the message, or positioning hasn't been
substantiated, they'll refuse and tell you exactly what's missing instead of generating
fluent copy on a shaky foundation. That's not a bug — it's the point. A credible "not
ready yet, here's what's blocking it" is worth more than a polished claim nobody can
defend in a room with Sales, Legal, or a customer.
