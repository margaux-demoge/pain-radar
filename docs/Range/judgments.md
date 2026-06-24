# Range — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The child development milestone-tracking space is densely populated with established free and freemium apps (CDC Milestone Tracker, Kinedu, BabySparks, Wonder Weeks, Pathways, Sparkler, ASQ-based tools), many backed by medical institutions. None positions itself exactly on "calibrated reassurance / show the range, close the conversation", but all cover the underlying milestone-data layer Range would need. Notably, the JMIR review and Harvard Health both flag that existing trackers actively *increase* parental anxiety due to high-sensitivity checklists, which is the gap Range is targeting, that's a real wedge, but the field itself is crowded. Failed-attempt signal is weak in public sources (small parenting apps rarely make shutdown news), so the graveyard is likely underreported rather than empty.

**Top competitors:**
- CDC Milestone Tracker — free, AAP-aligned checklist app, 2 months to 5 years, the de facto reference; criticized for high sensitivity / low specificity that alarms parents (active, https://www.cdc.gov/act-early/milestones-app/index.html)
- Kinedu — freemium, 1,800+ science-based activities + milestone tracking with personalized daily plans, the strongest commercial player (active, https://play.google.com/store/apps/details?id=com.kinedu.appkinedu)
- BabySparks — daily personalized activity program tied to development milestones, video-based (active, https://babysparks.com/)
- Pathways.org Baby Milestones — nonprofit, CDC/AAP-sourced milestones, explicitly positioned as reassurance + 'when to act' (active, https://pathways.org/mobile-app)
- Sparkler — ASQ-based parent screening app with referral thresholds baked in, closest to Range's 'threshold + what to ask pediatrician' model (active, used by state early-intervention programs)

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Calm down a specific low-grade worry about whether my kid is developing normally, by showing me where they actually sit on the real range and whether I should act.
Classification: occasional (recurs unpredictably, each time a new worry is triggered by comparison or a milestone moment)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. Parents may feel slightly more competent at reading developmental norms, but there is no tracked progression, no skill building, no mastery arc, the app explicitly avoids scoring.
- Autonomie (sentiment d'être en contrôle): Strong. The whole product is built around restoring agency to the anxious parent, replacing the forum spiral with calibrated information and a clear "do nothing" or "ask your pediatrician" decision.
- Lien social (sentiment d'être connecté à d'autres): Absent. Explicitly anti-forum, no community, no shared experience, no peer signal by design.

**Boucle d'habitude**
- Déclencheur: a new worry sparked by playground comparison, a milestone moment, or a family comment. INTERNAL (the anxious feeling itself is the cue), but the cue does not recur on a predictable cadence.
- Routine: pick the worry area, read the range, get a calm verdict, close the app.
- Récompense: immediate relief from anxiety, plus a clear next step. Immediate Y.
- Push reliance: the spec gestures at "check back in a month" which would be an EXTERNAL cue (push or email). Retention does not depend entirely on push, but the monthly check-in is the only structural return mechanism the spec names, and it is fragile.

**Verdict line**
Only autonomy passes cleanly among the three angles. The job is occasional rather than naturally recurring, and the habit loop, while it has an internal cue (anxiety) and immediate reward (relief), depends on the worry recurring, which the product itself is explicitly designed to suppress ("the goal is for you to stop worrying, not to come back daily"). This is a deliberate anti-retention stance, and the spec's own open question flags it: "Is stops you from scrolling actually a viable retention model." H1 (50% return within 30 days triggered by a new worry) is plausible because parental worry does recur across areas (speech this month, social next month), but the product has no structural pull beyond that.

**What needs to change for STRUCTURAL_RETURN**
- Is there a second job Range can do between worry spikes that would naturally recur, for example a light monthly milestone check the parent opts into, without turning into a scoring app?
- Could a sense of competence be built in, for example a small library of evidence-based everyday interactions the parent learns and applies across areas over time, so they feel they are getting better at reading their kid?
- Is the team comfortable accepting this as a low-frequency, high-trust churn product where the success metric is trust and word of mouth rather than DAU, and if so should H1's 30-day return target be reframed around a longer window?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Range has a sharp, well-defined target (anxious googler parents of 2-7) and a clear differentiated promise (calibrated ranges + honest thresholds, anti-engagement). The positioning survives basic scrutiny on "why not Google" and "why not pediatrician," but breaks down on trust/credibility (no MD-backed sourcing described), data input mechanics (how does the app actually know where my kid sits?), and the self-cannibalizing retention model that contradicts H1's 50% return target. Medical-liability and source-of-truth are flagged in the log but unanswered in the spec.

**Dangerous assumptions:**
- Anxious parents will trust an app's calibrated 'normal range' more than their pediatrician or Google without a visible clinical authority behind the data. Cheap test: show two landing pages to r/Parenting users, one with named pediatric advisors and source citations, one without, and measure signup intent.
- Parents can accurately self-report their kid's milestone status in a few taps so the app can place them on the range. If input is fuzzy or feels like a quiz, the 'calm screen' promise dies. Cheap test: paper-prototype the input flow with 5 parents, measure completion and whether they trust the resulting placement.
- An anti-engagement product where 'we close the conversation' can still hit 50% 30-day return (H1). Worry-recurrence frequency may be far lower than monthly, making the retention metric structurally unreachable. Cheap test: survey 30 target parents on how often a new milestone worry actually surfaces, and over what window.
