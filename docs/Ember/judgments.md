# Ember — judges verdicts

## benchmark-scanner: `EMERGING`

The couples-app space is crowded with shared-calendar / messenger / milestone-counter products (Lovewick, Coupled, Cupla, Love Counter) and Gottman-style prompt decks, but almost none attempt Ember's specific wedge: passive signal reading (texts, camera roll, calendar) translated into a single weekly observation that reframes feeling-state. Couples Analytics is the closest direct competitor on "rhythm + analytics," but it relies on active check-ins, not background signal. The graveyard (Tuned, Couple/Pair, Official) confirms the hard part is not the idea but distribution and the two-sided install, Ember's single-user framing dodges that trap. Window is genuinely open, but iOS permission reality (open question #1) is the real moat or the real wall.

**Top competitors:**
- Couples Analytics, AI relationship app with daily/weekly/monthly rhythm check-ins and a 'relationship health score', closest framing match but active-input not passive (https://couplesanalytics.com/)
- Smart Couple, tracks time together, affection, caring actions, negativity, manual logging based (https://www.smartcoupleapp.com/)
- Lovewick, relationship tracker for dates, memories, milestones, no passive signal reading (https://lovewick.com/)
- Cupla, shared calendar for couples that finds shared free time, adjacent on the calendar signal but no synthesis layer (mindfulsuite review)
- LoveTrack / Happy Couple / Gottman Card Decks, prompt-based intimacy apps, adjacent on 'reignite spark' goal but solve via questions not data (https://lovetrackapp.com/, https://www.gottman.com/couples/apps/)

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Tell me whether my fading feeling in a long-term relationship means the relationship is in trouble, or whether it is the normal floor of a steady curve.
Classification: occasional. The anxious question recurs but unpredictably (after a quiet week, a fight, a doomscroll), not on a fixed cadence. The Sunday-screen ritual is a designed cadence layered on top, but the underlying need does not pull the user back daily.

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. There is no skill to build, no progression. Marking moments is a light agency act, not mastery. The "rhythm score" could feel like progress but the spec explicitly warns against score-shaming.
- Autonomie (sentiment d'être en contrôle): Strong. The entire emotional payoff is "stop guessing", regaining control over an anxious narrative. Marking moments and seeing your own rhythm reinforces self-authored interpretation.
- Lien social (sentiment d'être connecté à d'autres): Absent. Single-user product (open question 3 still TBD). The partner is the subject, not a participant. No social loop.

**Boucle d'habitude**
- Déclencheur: Sunday weekly observation delivered as one screen. EXTERNAL (push/notification driven). A secondary internal cue exists ("lying next to them feeling nothing, open Ember to check the line") but is not designed into the loop, only implied.
- Routine: Read the one observation, optionally tap deeper into the year line, optionally mark a moment.
- Récompense: Reframing of the anxious feeling, "I feel more clear" (H2). Immediate Y, but emotionally muted, a calming rather than a hit. Risk: when the line is flat or dipping, the reward inverts into more anxiety.
- Push reliance: High. Retention appears to depend almost entirely on the Sunday push. Turn off notifications and the loop collapses to the ad-hoc anxious check-in, which is occasional at best.

**Verdict line**
Only one of the three angles clearly passes (autonomie). The job is occasional rather than naturally recurring, and the habit loop's cue is external (Sunday push) with no designed internal trigger. Compétence is weak by design (the team rightly fears gamifying love), and lien social is absent because it is a solo product. The Sunday ritual is a real anchor, but stripped of push it has nothing structural pulling the user back.

**What needs to change for STRUCTURAL_RETURN**
- Is there an internal cue the team can name and design for, the specific in-life moment ("after a quiet evening", "after a fight", "Sunday morning coffee alone") that would make users reach for Ember without a notification?
- Can the product nourish a second psychological need without turning love into a score? For instance, is there a version where the partner participates (shared rhythm, mutual marking) that adds lien social without becoming evidence in a fight, as flagged in open question 3?
- Beyond the weekly observation, is there a between-Sundays reward, something the user gets value from when the anxious feeling hits mid-week, that does not require waiting six days for the next screen?

## user-interview-simulator: `BUILT_ON_SAND`

Ember promises a passive, background read of a relationship using iOS signals that aren't actually accessible without heavy permissions or manual logging — and the spec's own product_log flags this as TBD. The emotional premise (a weekly one-liner will reframe "the spark is gone" into "you're in a dip") is doing enormous work without any evidence users want their relationship quantified at all; the opposite reaction (anxiety, surveillance creep, weaponization between partners) is just as plausible. The persona Lou wouldn't trust this app with her texts and camera roll based on the current pitch, and the spec has no answer for what happens when the line actually trends down.

**Dangerous assumptions:**
- Passive signal-reading (texts, photo content recognition of a specific person, calendar co-presence) is technically feasible on iOS without breaking the 'no work added' promise. Cheap test: spike the actual iOS permissions flow and measure how many of 10 target users complete it without bailing.
- Users in a quiet phase WANT their relationship plotted as a line. The opposite is plausible: seeing a flat line confirms the fear and accelerates the spiral. Cheap test: paper-prototype a downward-trending Ember screen with 8 target users and watch reactions — relief or panic?
- A weekly one-screen observation written 'like a friend' can be generated from thin behavioral signals without sounding like a horoscope or a Fitbit notification. Cheap test: hand-write 20 observations from fake signal data, show them to target users blind, ask which feel true vs generic.
