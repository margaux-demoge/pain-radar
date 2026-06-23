# Crumb — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

VERDICT: CROWDED_SPACE

**Problem benchmarked**
Solo home sourdough bakers cannot read their own crumb and have no fast, trusted way to get a diagnosis before their next bake.

**Direct competitors**
1. Sourdo — Sourdough Crumb Reads, AI analyzes a crumb photo for openness, evenness, fermentation quality, plus community share, active, https://apps.apple.com/us/app/sourdo-sourdough-crumb-reads/id6745407871
2. Crumb Coach, photo-based AI loaf/starter feedback plus community for sharing bakes and questions, active (launched 2025-2026), https://apps.apple.com/us/app/crumb-coach/id6752313432
3. Sourdough AI, snap a photo, instant expert-level AI feedback on crumb, crust, starter, active, https://apps.apple.com/us/app/sourdough-ai/id6751040790
4. Loaflo, AI photo analysis on crumb and starter, plus "Mr. Crumb" assistant and starter tracker, active, https://loaflo.app/
5. Sourdough Baker AI (MWM), photo-in / feedback-out on texture, rise, crust, iOS and Android, active, https://mwm.ai/apps/sourdough-baker-ai/6503015809
6. DoughPilot, "logic-first" non-AI diagnosis app for planning, tracking, and diagnosing bakes, active, https://www.dough-pilot.com/
7. The Sourdough Club Loaf Analysis, expert-led paid feedback session on uploaded loaves, active, https://thesourdoughclub.com/loaf-analysis/

**Failed attempts**
None surfaced. The category exploded in 2025-2026 on the back of cheap multimodal vision, so there is not yet a visible graveyard. The absence of dead bodies is itself a yellow flag: every entrant is still in the "is anyone retaining?" phase.

**Adjacent players**
1. r/Sourdough, free-form peer feedback on crumb photos at massive volume, relevant: the de-facto status quo Crumb is replacing, slow, noisy, no reputation, https://reddit.com/r/Sourdough
2. The Fresh Loaf, text-heavy forum with crumb diagnosis threads, relevant: long-tail incumbent for the exact problem, https://www.thefreshloaf.com/node/74131/crumb-diagnosis
3. Homebaker, visual timeline tracking of each bake session with recipe sharing, relevant: covers the "stack my loaves over time" layer Crumb also wants, https://www.homebaker.app/
4. Breadwinner, hardware sensor for starter peak tracking, relevant: owns the starter-data side of the same baker, https://breadwinner.life/
5. Sourdough Unchained, paid coaching community with daily expert answers on photos and videos, relevant: human-diagnosis competitor, just packaged as a subscription community, https://www.culinaryexploration.eu/sourdough-unchained

**Failure pattern**
Not enough failed attempts to identify a pattern. The bigger signal is the opposite: a 2025-2026 gold rush of nearly identical AI-crumb-analysis apps means the differentiator (AI vision) is already commoditized and the real war will be on retention and community quality.

**Verdict line**
The category is freshly crowded: at least six live apps already promise crumb diagnosis, three of them (Sourdo, Crumb Coach, Loaflo) bundle AI analysis with a community layer, which is exactly Crumb's pitch minus the structured-tag plus reader-reputation mechanic. The wedge Crumb is betting on, peer diagnosis as tagged clusters with reader reputation rather than AI or free-form comments, is genuinely under-served, but it has to outrun a market where users will reach for an instant AI verdict before waiting an hour for three humans. The wedge has to be sharp. What does the team have that the top 3 competitors do not?

Sources:
- https://apps.apple.com/us/app/sourdo-sourdough-crumb-reads/id6745407871
- https://apps.apple.com/us/app/crumb-coach/id6752313432
- https://apps.apple.com/us/app/sourdough-ai/id6751040790
- https://loaflo.app/
- https://mwm.ai/apps/sourdough-baker-ai/6503015809
- https://www.dough-pilot.com/
- https://thesourdoughclub.com/loaf-analysis/
- https://www.homebaker.app/
- https://breadwinner.life/
- https://www.culinaryexploration.eu/sourdough-unchained
- https://www.thefreshloaf.com/node/74131/crumb-diagnosis
- https://www.sourdoughforge.com/en/best-sourdough-apps

**Top competitors:**
- Sourdo — Sourdough Crumb Reads
- Crumb Coach
- Sourdough AI
- Loaflo
- Sourdough Baker AI (MWM)
- DoughPilot
- The Sourdough Club Loaf Analysis
- r/Sourdough (status quo)
- Sourdough Unchained

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Help a home baker understand what went wrong (or right) with the loaf they just cut, fast enough to apply the lesson to the next bake.
Classification: naturally recurring (the target user bakes at least every two weeks, often weekly, and each bake produces a fresh diagnostic moment)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong. The personal timeline with pinned variables, plus the explicit "stop guessing after ten loaves" arc, is built around visible mastery. Readers also accumulate an accuracy score, so both posters and readers feel progression.
- Autonomie (sentiment d'être en contrôle): Weak. The baker chooses variables and decides what to apply, but the experience itself is fairly constrained (structured form, tag set, no free-form). Control sits more with the system than with the user.
- Lien social (sentiment d'être connecté à d'autres): Strong. The whole product is a peer diagnosis loop. Bakers see other humans reading their loaf within minutes, and readers feel useful by diagnosing. Reputation compounds across people.

**Boucle d'habitude**
- Déclencheur: cutting into a fresh loaf in the kitchen and seeing a crumb the baker cannot read alone. INTERNAL (the slice itself is the cue, it happens in the physical world independent of the app).
- Routine: snap the crumb, tap through preset variables in under a minute, post to Fresh queue. Quick enough to fit the cue window.
- Récompense: first structured diagnosis within 15 minutes, cluster signal within the hour, while still in the kitchen. Immediate Y (target is sub-hour, designed for the same baking session).
- Push reliance: not the primary mechanism. The cue is the loaf itself. Push may help readers on the diagnosis side, but poster retention does not depend on it.

**Verdict line**
Two of three angles pass clearly. The job recurs naturally on every bake, which for the target user is at least biweekly and often weekly. The habit loop has a strong internal cue (the cut slice) and an immediate reward (cluster within the hour). Psychological needs are mixed: competence and social connection are strong by design, autonomy is the weak leg because the experience is deliberately constrained. That is a known tradeoff for a structured-diagnosis product, not a fatal flaw. The real risk lives in product_log open question #2: reader retention once high-rep readers stop learning themselves, which is a separate retention surface the spec does not yet address.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

VERDICT: WEAK_ON_ASSUMPTIONS

**Simulated user**
Marcus, 34, Portland OR. Software PM, bakes every weekend, ~22 loaves under his belt. Active lurker on r/Sourdough, posted two crumb shots there last month, got 14 comments mostly saying "looks great!" with one contradictory "underproofed" buried below. Keeps a Notes app log of hydration and bulk times. Uses Instagram for inspiration, follows Maurizio and a few French bakers. Mildly skeptical, time-poor on Saturday mornings when the loaf comes out, and already burned by a niche cooking app that died after six weeks.

**Interview**

Q1, "I already post on r/Sourdough and get answers in an hour. Why do I download a second app instead of just posting there?"
> PARTIAL
The spec contrasts r/Sourdough as "high noise, slow turnaround" but does not address the switching cost or why Marcus, already getting answers, would re-enter his variables in a new place.

Q2, "When I post my crumb at 9am Saturday, who exactly is on the other end at 9:15am to diagnose it? Where do those people come from on day one?"
> UNANSWERED
The spec assumes a live reader pool ("Fresh queue, scrolling in real time") but has no cold-start mechanic. Product log flags this as an open question.

Q3, "I bake every two weeks. I'm not opening your app between bakes. Why would I diagnose other people's loaves when I'm not baking?"
> UNANSWERED
The spec needs readers active between their own bakes for the 60-min target to work. No motivation loop for reader-mode is described beyond a "quiet reputation."

Q4, "The form has hydration, flour, bulk time, retard, shape, oven. My bake also depends on ambient temp, starter ratio, and how I shaped. If the form misses my variable, do I just not get diagnosed correctly?"
> PARTIAL
The spec commits to "presets, not essays" but the variable list is fixed and may miss what actually drives the crumb. Product log flags this. No fallback described.

Q5, "Four people say overproofed, one says weak starter, two say looks fine. That's the same noise I get on Reddit. Why is the cluster more trustworthy here?"
> PARTIAL
Reader-score weighting is mentioned but not explained operationally. The user can't see how disagreement gets resolved or how confident a "cluster" really is.

Q6, "How do you know a diagnosis was 'later confirmed by the original baker'? I'm the one with the bias, my next loaf is a different loaf. What does confirmation even mean?"
> UNANSWERED
Reputation system rests on confirmation but confirmation mechanic is not defined. This is load-bearing for the entire reader-quality story.

Q7, "I cut my loaf at 9pm after dinner. By the time I post and wait an hour, it's 10pm and I'm not baking tomorrow, I'm baking next Saturday. Where does your '60 minute, still in the kitchen' promise leave me?"
> UNANSWERED
The use case assumes same-day or next-day rebake. Bi-weekly bakers (the stated target) break this loop. The spec sells urgency the target user does not have.

Q8, "I've been at this a year. Beginners on r/Sourdough confidently call my loaf 'underproofed' when it isn't. Why would beginner reads stacking, even weighted lighter, not pollute my cluster?"
> PARTIAL
"Weighted lighter" is asserted but the weighting threshold and visibility rules aren't defined. A flood of low-weight reads can still drown a signal.

Q9, "Why would the best readers, the ones whose accuracy compounds, keep diagnosing strangers' loaves once they've leveled up and have nothing to learn from doing it?"
> UNANSWERED
Product log explicitly lists this. Spec says "no karma chase, no rank to grind," which actively removes the extrinsic hook without replacing it.

Q10, "If I post my loaf and the cluster says 'overproofed' but it's actually my flour, I'll change bulk time next week, fail again, and blame the app. What stops a confidently-wrong cluster from making me worse, not better?"
> UNANSWERED
The spec has no calibration layer, no "the cluster might be wrong" UX, no expert override. H3's success metric (40% apply feedback) assumes feedback is right; spec has no mechanism to detect when it isn't.

**Score:** 0/10 answered, 4/10 partial, 6/10 unanswered

**Top 3 dangerous assumptions**

1. A live reader pool will be on Crumb at 9:15am Saturday to diagnose Marcus's loaf within 60 minutes (H2 = 60%). Why dangerous: cold-start and reader-retention together break the entire core promise; if no one is there in the first hour, every other metric collapses. Cheap test: post 20 seeded loaves at staggered times in a Discord/Slack of recruited bakers, measure time-to-3-diagnoses without any product, see if humans show up unprompted twice.
2. "Diagnostic accuracy" can be measured because bakers will confirm what the cluster said. Why dangerous: the entire reputation system, which is the spec's defense against Reddit-level noise, depends on a confirmation loop that is not defined and may not be reliable (baker bias, no ground truth, next loaf is a different loaf). Cheap test: run a paper prototype with 10 bakers, ask them to "confirm" diagnoses on past loaves a week later, see if confirmations are consistent enough to power a score.
3. The fixed structured tag set + variable preset list covers enough of the real diagnosis space that bakers don't revert to free-form. Why dangerous: if bakers feel constrained, they leave or comment in the "one short note" field, regressing the product to Reddit. Cheap test: take 30 real r/Sourdough crumb threads, try to encode each top comment into the tag set, measure coverage and forced-fit rate.

**Verdict line**
The positioning is sharp and the persona is real, but six of the ten hardest questions a target baker would ask have no answer in the spec, and two of the three dangerous assumptions (live reader pool, confirmation loop) are load-bearing for every success metric. The product is defensible if those mechanics get specified before build; right now it is selling a promise the spec does not yet know how to keep.

**Dangerous assumptions:**
- A live reader pool will be active within 60 minutes of any post from day one, despite no cold-start mechanic and a target user who bakes only every two weeks.
- Reader accuracy can be measured via 'baker confirmation,' but the confirmation mechanic is undefined and the baker has no ground truth for whether the cluster was right.
- The fixed structured tag set and variable preset list cover the real diagnosis space well enough that bakers do not revert to free-form prose.
