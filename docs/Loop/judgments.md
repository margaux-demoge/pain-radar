# Loop — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "small repeating dinner rotation" angle is not a gap, it is the explicit positioning of multiple shipping apps: OnRotation, MealPlanned, Spinning Meals, and the rotation features in Plan to Eat all sell "your favorites on repeat" with auto grocery lists. Mealime and eMeals dominate the broader weeknight planner segment with millions of installs. The graveyard is real too (Yummly killed in Dec 2024 after Whirlpool acquisition), and a recurring user complaint about Mealime is precisely that the rotation gets repetitive, meaning Loop's "restraint = feature" thesis may already be how users experience competitors negatively. Loop's wedge (a hard-capped 7, "swap one not all", no feed) is plausible but needs to be sharper than UX restraint to beat incumbents with grocery integrations and recipe libraries.

**Top competitors:**
- OnRotation (onrotation.app), active, explicit 7-day meal pack with shared household, freezer reminders, auto shopping list — closest direct match to Loop's core promise
- MealPlanned (mealplanned.io), active, automates rotation by tracking recently-cooked meals and surfacing the next dinner — same anti-decision-fatigue thesis
- Spinning Meals (spinningmeals.com), active, lets you fix recurring meals to specific weekdays (Pizza Night Thursday) — the literal 'on repeat' UX
- Mealime, active and dominant, simple weeknight 'dinner list + shopping list' planner; small-rotation complaint surfaces in reviews — Loop is essentially Mealime with a hard cap and no novelty feed
- Plan to Eat, active, bring-your-own-recipes with built-in meal-rotation feature and grocery list — the incumbent Loop's H3 directly targets

## retention-validator: `STRUCTURAL_RETURN`

The job (feed the family on weeknights) recurs every single evening at the same moment, which is the strongest possible recurrence signal. SDT: compétence is Strong (visible star/frown progress narrowing toward a stable rotation, more cook-nights/week), autonomie is Strong (user types meals they already cook, controls swaps), lien social is Absent (no household sharing, no community). Habit loop closes on an internal cue (6pm fridge-stare / dinner decision fatigue) reinforced by a 4pm push, with a fast routine (tap to recipe/grocery, star/frown) and an immediate reward (dinner decided, food on table). Two of three angles pass cleanly, making this a structural return product despite the lien social gap and the partial reliance on the 4pm push as external scaffolding.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Loop has a sharp, contrarian positioning (restraint over novelty, fixed rotation over feed) and a clearly defined target (parents who cook 3 nights, want 5). The persona scrutiny holds up on the core "why a small loop" thesis and the 4pm nudge. But it falls apart on the practical mechanics that determine whether a real parent uses it past week 2: family variety tolerance (kids/partner eating the same 7 meals on rotation), the cold-start when "what you've cooked successfully" is a thin list, what "swap" actually means when the user hates 3 of 7, and the trust gap of typing meal names with no recipe library backing it. Evidence base in product_log.md is also misaligned (links are about parenting/sleep, not cooking), which weakens the signal claim.

**Dangerous assumptions:**
- Families will tolerate eating the same 7 meals on a 4-week loop. Kids and partners often drive variety demand, and the spec never addresses pushback from non-cookers in the household. Cheap test: 10-question survey to target parents asking 'would your kids/partner accept the same 7 dinners for a month?' before any build.
- Users have enough recall to seed the rotation by typing meals they've 'cooked successfully in the last month.' Many target users feel behind precisely because they haven't cooked much, so the cold-start input is thin or empty. Cheap test: paper prototype the onboarding with 5 target parents, count how many meals they can name unaided in 2 minutes.
- Restraint (no recipe feed) is a retention driver rather than a churn driver. Users may equate 'no new content' with 'app is done, why open it' and uninstall after the rotation is set. Cheap test: concierge MVP via SMS for 4 weeks with 5 parents, measure whether they keep engaging once the rotation stabilizes.
