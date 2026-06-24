# Even — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The restrict-binge / anti-diet / intuitive-eating app space is densely populated with active, well-positioned players (Thora, Cravr, R.care, Way, Peace With Food, Recovery Record, Rise Up + Recover) all explicitly addressing the binge-restrict cycle, several with the same anti-diet, anti-streak, pattern-awareness framing Even proposes. Thora in particular markets near-identical language ("stuck in the binge-restrict cycle... without diets, restriction, or food guilt") and is already monetizing at $14.99/mo. Failed attempts are hard to surface in this category because the apps that die tend to be small and uncataloged, but the bigger risk here is differentiation, not absence of demand. Even's wedge (visualize the loop as bands of color, intervene at the front not the back) is plausible but not yet defensibly distinct from Thora's "understand the WHY behind your patterns."

**Top competitors:**
- Thora — anti-diet binge-restrict cycle tracker with pattern check-ins and intuitive-eating program, active, $14.99/mo, https://www.thoraapp.com — closest analog to Even's positioning
- Cravr — neuroscience-framed craving/binge companion targeting emotional eating, active, https://apps.apple.com/us/app/cravr-craving-companion/id6737430665
- R.care — binge-eating recovery with real-time meal coaching and stress-free mood/food logs, active, https://apps.apple.com/us/app/r-care-binge-eating-recovery/id6470239697
- Way — Healthline's 'Best Non-Diet App' three years running, CBT + intuitive eating sessions, active, https://apps.apple.com/us/app/way-intuitive-eating-app/id1589188038
- Recovery Record / Rise Up + Recover — CBT-based self-monitoring of meals and behaviors, clinician-connected, active, https://www.recoveryrecord.com/

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Help me see and gently exit the restrict-binge cycle I'm stuck in, without being shamed for it.
Classification: naturally recurring (the job is tied to eating, which happens multiple times every day, and the cycle itself repeats weekly).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong. The colored band visualization makes pattern softening visible over weeks (shorter restriction bands, more green), giving a felt sense of progress that isn't tied to weight.
- Autonomie (sentiment d'être en contrôle): Strong. The app explicitly refuses to prescribe a diet or calorie target. Inputs are three self-defined states, nudges are permissions not commands, and binge days carry no penalty. Control sits with the user.
- Lien social (sentiment d'être connecté à d'autres): Absent. No mention of community, sharing, peers, or coaches in the spec.

**Boucle d'habitude**
- Déclencheur: Each meal (eating or skipping one) is the cue to open the app and tag a state. INTERNAL (tied to a bodily/contextual moment that recurs multiple times a day on its own).
- Routine: Log meal as eaten/skipped, tap one of three states (freely / restricted / binged). Very low friction.
- Récompense: Immediate Y. The colored band updates and the pattern becomes visible; on stacked-restriction days, a permission nudge arrives. Reward is informational and emotional (being seen without shame) within seconds.
- Push reliance: Some external push is implied (the front-of-loop permission nudge), but the core cue is internal (the meal itself), so retention does not hinge on notifications.

**Verdict line**
All three angles pass: the underlying job recurs multiple times daily, two of three psychological needs are Strong (compétence via visible pattern softening, autonomie via the explicit anti-prescription stance), and the habit loop closes on an internal cue (the meal) with an immediate visual + emotional reward. The one structural gap is social connection, which is intentionally absent and could be a long-term retention ceiling, but the spec already clears the bar for STRUCTURAL_RETURN.

**What needs to change for STRUCTURAL_RETURN**
N/A.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Even has a sharp, differentiated thesis (track the loop, intervene at the front) and a well-defined target who self-identifies with the restrict-binge cycle. The persona "Jess, 31, Portland, ex-MyFitnessPal user" recognizes the pain immediately. But the spec leans heavily on three unvalidated bets: that self-labeling a meal as "restricted" or "binged" won't itself become a shame trigger, that a one-sentence "permission to eat" nudge can actually interrupt a restrictive streak, and that users who explicitly want weight loss will stay engaged with an app that refuses to promise it. Six of ten questions land partial or unanswered; the core mechanic survives scrutiny, the surrounding promises don't.

**Dangerous assumptions:**
- Self-tagging meals as 'restricted' or 'binged' is therapeutic rather than shame-inducing. If labeling oneself a binger three times a day deepens the shame loop instead of revealing it, Even becomes a new vector of the same problem. Cheap test: 5-day diary study with 8 target users using paper cards with the three labels, measure self-reported shame delta vs MyFitnessPal baseline.
- A timely one-sentence 'permission to eat' nudge can actually break a restrictive streak in users who have been restricting for years. The spec asserts this will work in 40% of cases but offers no mechanism beyond the sentence itself, and these users have already ignored the same message from books, therapists, and Instagram. Cheap test: SMS-based wizard-of-oz for 2 weeks with 10 users, manually send the nudge when they log a restricted meal, measure next-meal label.
- Users in the restrict-binge cycle will stay 8 weeks with an app that explicitly does not promise weight loss. Open question #3 in the log flags this. Most of the r/loseit evidence is from people actively trying to lose weight, the framing 'cycle gets less violent' may not be a strong enough hook against MyFitnessPal's scale-down promise. Cheap test: landing page A/B, 'break the binge-restrict cycle' vs 'lose weight without binging', measure email signup rate.
