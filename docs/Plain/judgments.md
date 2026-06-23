# Plain — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "calm, anti-diet, no-tracking" position is already a crowded category. Way, MEAL, Eated, See How You Eat, Munch and Recovery Record all sell some version of "skip the calorie tracker, build awareness, eat without dogma." Way explicitly won Healthline's Best Non-Diet App three years running, and Simple/no.Diet have raised the noise floor with "no counting" marketing while still being subscription weight-loss products. Plain's wedge (5 fixed rules, 50 fixed recipes, refusal to update with trends) is sharper than most, but the editorial / boring-on-purpose stance has to beat incumbents that already own the anti-diet keyword.

**Top competitors:**
- Way (eatmyway.com) — intuitive eating app, $9.99 one-time, Healthline Best Non-Diet App 2023-2025, closest brand-voice rival to Plain
- MEAL - Mindful Eating & Living — dietitian/CBT-curated, no diets/macros, addresses overeating without tracking
- See How You Eat (SHYE) — visual food tracker with no calories, awareness over numbers
- Simple Life — markets 'no calorie counting, no restrictions' with 5-rule-style habits, but at AI-coach scale (Top 100 AI Companies 2025)
- no.Diet — Mediterranean-diet app explicitly positioned against strict counting, flexible balanced rules
- ZOE — 'add don't subtract' plant-diversity rules, anti-restriction framing but science-heavy not boring
- Noom — behavioral / habit-based, not rule-based, but owns the 'kinder than calorie counting' category

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Help me feel calm and confident about what to eat without having to think about it. Classification: naturally recurring (eating happens 3x/day, every day).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. The weekly hit/miss chart hints at progress but is deliberately muted ("no number, just a small calm chart"), so the feeling of mastery is faint by design.
- Autonomie (sentiment d'être en contrôle): Strong. The whole pitch is reclaiming control from diet tribes, five rules you own, no dogma, no algorithm pushing trends.
- Lien social (sentiment d'être connecté à d'autres): Absent. No social layer, no sharing, no community, the product is explicitly a private calm zone.

**Boucle d'habitude**
- Déclencheur: end of a meal, the user taps hit / missed / didn't try. INTERNAL (the meal itself is the cue, encountered 3x/day in real life regardless of the app).
- Routine: one tap among three buttons after a meal, occasional chat question, occasional recipe lookup from the 50-recipe library.
- Récompense: a sense of calm and "I'm on track" via the small weekly chart; immediate reward per tap is thin (no number, no streak, no celebration). Immediate Y/N: partial, the tap itself yields little, the reward is cumulative over the week.
- Push reliance: not mentioned in the spec; retention does not appear to depend on push, the meal itself is the cue.

**Verdict line**
The need recurs naturally (eating is daily) and the cue is internal (each meal triggers the log), so the habit-loop angle and the recurrence angle both lean positive. However the reward is intentionally muted (the product's whole stance is "boring on purpose"), competence signals are deliberately weakened, and social connection is absent by design. Autonomy is the only Strong psychological need. That gives roughly 1.5 of 3 angles, the loop exists but its reward is fragile, so this sits at WEAK_RETURN rather than STRUCTURAL.

**What needs to change for STRUCTURAL_RETURN**
- What is the felt reward in the two seconds after a user taps "hit the rules"? Without something immediate, the calm chart alone may not pull the next tap.
- Is there a lightweight competence signal (a streak of "rule-compliant days", a personal rotation of favorite meals surfacing) that fits the boring-on-purpose tone without becoming gamified diet drama?
- Should the chat or the 50-recipe library carry a recurring discovery moment (one new rotation suggestion a week) so the user has a second reason beyond logging to reopen the app?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Plain has a sharp editorial position ("boring middle", anti-trend, 5 rules) and a clearly defined target (diet-war-fatigued adults), which gives it real positioning strength. But the spec leaves the hardest user objections unanswered: why trust these 5 rules over a doctor or a louder app, why pay/stay engaged when the value is "nothing happens", and how the chat stays boring without a credentialed advisor (an open question even in the product log). The persona's most likely friction points (habit decay, lack of feedback loop, free alternatives like "just eat vegetables") aren't addressed. Solid hypothesis, but multiple core assumptions are untested and one is structurally fragile (credibility source).

**Dangerous assumptions:**
- The 5 rules carry enough authority on their own to be trusted and followed without a named nutritionist, MD, or institutional backing. Cheap test: A/B landing pages, one with anonymous rules, one signed by a credentialed advisor, measure signup intent.
- Users will stay engaged 8+ weeks with an app that deliberately offers no novelty, no streaks, no numbers, no progress drama. The 'calm chart' may be too thin a feedback loop to beat the boredom it celebrates. Cheap test: 4-week paper prototype with 10 users logging 3-button meals, measure day-7 and day-21 drop-off.
- The target user (diet-fatigued adult) actually exists as a buyer segment and not just a vibe. People who reject diet culture often reject food apps entirely rather than switch to a calmer one. Cheap test: 15 interviews with people who've quit MyFitnessPal/Noom in last 6 months, ask what they replaced it with, see if 'a calmer app' is a real desire or if they just want to stop thinking about food.
