---
name: strategic-narrative
description: Craft the movement-level story (Andy Raskin's strategic narrative) — name the old-game→new-game shift, the stakes (winners and losers), the object of the new game (Promised Land), the obstacles, capabilities as "magic gifts," and evidence the story comes true. Fires on prompts like "build a strategic narrative," "what's our why-now story," "name the shift," "old game new game," "promised land," "Raskin framework," "our pitch starts with the product and falls flat," "prospects keep asking how we're different from X," "rebuild the sales deck opener," "we need a movement, not a feature list," or "what's the campaign narrative." Also the natural next step after `positioning-messaging` when the product sells to enterprise or group buyers and needs a story bigger than a category claim. Requires an existing product hub with a chosen positioning POV in `07-positioning.md` (an `Assumption`-labeled POV counts); will say so and point back to `positioning-messaging` if that's still empty.
---

# Strategic Narrative

Turn a chosen positioning into a movement people want to join. Where positioning is the
*decision* (Dunford spine, `07-positioning.md`) and the messaging house is the *hierarchy*
(`08-messaging-house.md`), the strategic narrative is the *drama*: a single old-game →
new-game story that opens sales decks, structures the homepage, generates campaign
themes, and doubles as a roadmap filter. Based on Andy Raskin's five-element framework
(Zuora / "Greatest Sales Deck," Gong, Drift, 360 Learning), adapted to this kit's
evidence discipline — because the shift itself is a claim, and most narratives skip
checking whether it's true.

The anti-pattern this replaces is the **Arrogant Doctor**: "you have a problem, I have a
solution, here's why mine beats the others." That structure invites feature comparison
and puts prospects on the defensive. The narrative structure instead makes the buyer the
protagonist of a change already underway in their world — with or without you — and
positions the product as the gift that helps them win the new game.

## Gate check (do this first, every time)

- `07-positioning.md` has a chosen point of view with a confidence label, not the blank
  template. An `Assumption`-labeled POV counts. If it's empty, say so and point back to
  `positioning-messaging` — a narrative dramatizes a chosen position; it must not invent
  one.
- There is *some* external context to name a credible shift from — at least one reasoned
  entry in `04-competitor-map.md` or one external row in `02-evidence-log.md` (market
  signal, customer language, analyst framing). A shift named from pure introspection is a
  hypothesis wearing a story costume; say so and point to `evidence-synthesizer` or
  `competitor-discovery`.
- **Fit check, stated honestly:** this framework earns its keep for considered,
  multi-stakeholder purchases (enterprise/B2B tech, group buying committees) where one
  story must unite many heads. For spec-comparison or impulse purchases it adds little —
  if `03-customer-and-jobs.md` describes that kind of buyer, say so and recommend
  stopping at `messaging-house` instead. Proceeding anyway is allowed, but flag it.

If a gate fails, don't draft `14-strategic-narrative.md`. Say exactly what's missing and
which skill closes it — expected output, not a failure.

## Process (once the gate passes)

Work the five elements in order — each depends on the one before it. Draft into
`14-strategic-narrative.md`.

1. **Diagnose the current pitch.** Read the current deck/homepage/one-pager if present in
   `inputs/` or `13-copy-library.md`. Mark where it commits Arrogant Doctor moves:
   opening with product, HQ, investors, logos, or a "your approach is flawed" problem
   slide. This before-state sharpens the rewrite and gives stakeholders a contrast to
   react to.

2. **Name the shift (old game → new game).** The undeniable change in the *buyer's*
   world that creates big stakes and urgency — happening with or without us.
   - **Name both games concisely.** Software → cloud. Transactions → subscriptions.
     Opinions → reality. Top-down learning → upskill from within. Naming trades
     completeness for memorability; that's the deal, not a flaw. Generate 3–5 candidate
     namings, recommend one, keep the others in the file.
   - **Borrowing beats coining.** A shift name already gaining market traction (Uberflip
     borrowed "engagement economy" from Marketo) is legitimate and faster than weeks of
     wordsmithing. Check `02-evidence-log.md` and `04-competitor-map.md` for language the
     market already uses.
   - **It's a mindset shift, not competitor-bashing.** Alternatives (including "do
     nothing," from `04-competitor-map.md`) get positioned as rooted in the old game —
     not as inferior products. "Want to play the old game? Be my guest."
   - **The shift is a claim.** Log it: `The market is moving from <old> to <new>.
     [Confidence | prov: ...]` in `02-evidence-log.md`, and add what would validate or
     falsify it to the Validation Backlog in `00-index.md`. An `Assumption`-labeled shift
     ships — labeled; an untraceable one does not.

3. **Name the stakes (winners and losers).** Buyers suffer loss aversion; the status quo
   wins unless the future stops looking "sort of OK." Split it: a very negative outcome
   for those who don't adapt, a very positive one for those who do — figuratively, kill
   the aunt and uncle.
   - Name **winners already playing the new game** — real companies, each with an
     evidence-log pointer. Named losers (the Blockbuster slot) work too, with the same
     discipline.
   - Quantify the cost of not adapting where evidence allows; where it doesn't, label the
     stake as `Assumption` rather than inventing a scary stat.

4. **Name the object of the new game** (Raskin's earlier term: the Promised Land). The
   rallying cry — what winning the new game means for the buyer. "Turn customers into
   subscribers." "Own the journey." Seven words is a good ceiling.
   - **It's a future state, not our product.** Test: if it mentions our technology or
     could caption a feature screenshot, rewrite. It's what life is like *thanks to*
     having the product.
   - **Desirable and hard to reach without help** — otherwise the product has no reason
     to exist. Both halves get checked against `03-customer-and-jobs.md`.
   - **Phrase a question form** — "What would it take to turn every customer into a
     subscriber?" — which recruits the buyer as co-author of the story. Note both the
     statement and question forms in the file.
   - Sanity-check against the org's actual mission in `context/`: for the buyer, this
     line *is* the company mission. If they'd conflict, flag it to the human.

5. **Name the obstacles — then introduce capabilities as gifts.** Obstacles are why
   reaching the object of the game is hard *without us* — the old "problems we solve,"
   repackaged inside the new game so they carry emotional weight. If the buyer could just
   destroy the Death Star, there's no movie.
   - Each obstacle pairs with the capability ("magic gift" — the lightsaber, the
     wizardry) that overcomes it, traced to a row in `09-value-prop-matrix.md`. A gift
     with no obstacle is a feature list sneaking back in; an obstacle with no gift is a
     gap — log it, don't paper over it.
   - Capabilities appear here for the first time. If product shows up earlier than this
     point in the narrative, the structure is broken.

6. **Offer evidence the story comes true.** A well-designed object of the game makes
   buyers rightly skeptical. The strongest evidence: **stories of customers like them who
   already reached it** — pulled from `02-evidence-log.md`, each with provenance. Logo
   walls and investor slides are weak substitutes; demos count as evidence only when
   framed as the path to the object of the game. Missing customer stories are a named
   proof gap with a validation item, not a license to invent.

7. **Assemble and hand off.**
   - Write the **narrative in one breath** — a spoken paragraph a rep, founder, or brand
     marketer can deliver without slides.
   - Write the **deck skeleton**: discovery questions first (the narrative is a
     conversation, not a monologue), then shift → stakes → object of the game (question
     form) → obstacles → gifts → customer stories → demo. Every slide title is a
     takeaway, not a label ("Winners are already playing the new game," not "Market
     trends").
   - Record the **roadmap filter**: the one-line test the narrative gives product
     decisions ("does this help buyers <object of the game>?"). Gong cut feature requests
     about *opinions*; 360 Learning prioritizes by *upskill from within*. Note it for
     `11-stakeholders.md` — this is what makes the narrative strategy, not copy.
   - Run the **claims-substantiation check** on the whole file: every named winner,
     stake, and gift traces to `02-evidence-log.md`. Comparative claims and
     regulated-market claims get flagged for human legal/PM review — don't self-clear.

## Field test (the narrative isn't done until it survives contact)

Roll out lean: a handful of live calls or stakeholder conversations, not the whole org.
The test of the shift is whether it *sticks* — prospects nod and volunteer "let me tell
you how that's playing out for us." Train the teller to ask: **"Am I crazy, or are you
seeing this too?"** Log results in the file's Field Test Log with dates. Blank stares or
"how are you different from X?" reappearing = the shift or the object of the game needs
rework — iterate before full rollout. Expect the first team review to hurt: a clean draft
means most of the workshop's ideas got cut. A draft that provokes reactions beats boards
of ideas; plan the revision round rather than defending version one.

## Rules

- Never open with the product — in the narrative, the deck, or the homepage hero.
  Capabilities enter at element 5, as gifts, or the structure has failed.
- The buyer is Luke; we are Obi-Wan. Any draft where the company is the hero gets
  rewritten before it leaves the file.
- Don't clone someone else's narrative with our logo on it (the Zuora-deck failure mode).
  Principles, not template — slide count and phrasing come from our evidence, not theirs.
- The category name is shorthand for the movement, not the movement itself — don't spend
  the session wordsmithing three magic words ("strawberry intelligence" would have
  worked for Gong; the story mattered). If drafting surfaces doubt about the category
  *decision*, flag it back to `positioning-messaging` rather than quietly redeciding here.
- The narrative is orthogonal to category and outlives it (HubSpot's *inbound* survived
  its category moving from marketing automation to CRM) — pivots in `07-positioning.md`
  step 5 don't automatically invalidate this file, but trigger a review.
- Narrative-market fit is owned at the top. This skill drafts and pressure-tests; per
  `11-stakeholders.md`, the most senior owner (CEO for a company story, product/BU lead
  for a product story) must front it, with a narrative team of ≤4. If no owner exists,
  that's a stakeholder gap — name it.
- Never let story quality outrun label honesty: a stirring shift resting on a labeled
  `Assumption` is fine; the same shift passed off as validated market fact is a
  liability.

## Output

Updates: `14-strategic-narrative.md` (only if the gate passes), `02-evidence-log.md` (the
shift claim + winner/loser pointers), `00-index.md` (Freshness row, Validation Backlog
items for the shift and stakes, Next Best Action — or the gap list if gated).

Feeds: `messaging-house` derives `08-messaging-house.md`'s Narrative from this file when
it exists; `copywriting` pulls shift/object-of-the-game language into `13-copy-library.md`;
`campaign-starter` uses the shift as campaign-theme fodder (in a narrative-led company,
most content is about the shift, not the product); `stakeholder-alignment` records the
narrative owner and roadmap filter.

End with the single next best action — normally the field test (who tells it to which
prospect this week), `messaging-house` to cascade it into pillars and angles, or the
single most load-bearing assumption behind the shift to validate first.
