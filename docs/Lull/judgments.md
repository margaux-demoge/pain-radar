# Lull — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The toddler bedtime/sleep coaching space is crowded with well-funded, actively-growing direct competitors: Huckleberry (pediatric expert + AI SweetSpot predictions, serves up to age 5), Smart Sleep Coach by Pampers (P&G-backed, adaptive schedule, toddler tier), Lovebug, Napper, and Happy Baby all claim "personalized, adaptive schedules that evolve as your child grows" — Lull's exact pitch. Adjacent device/routine players (Hatch Rest, Goally, Moshi) own the in-routine UX layer. Children's Hospital Colorado has publicly flagged that most kids' sleep apps lack evidence, signaling many small attempts have died unseen, but no specific named graveyard surfaced. The wedge needs to be sharper than "adaptive, non-shaming, one-thing-at-a-time" — Huckleberry already markets exactly that.

**Top competitors:**
- Huckleberry — AI + pediatric expert sleep coaching with SweetSpot predictions for kids 0-5, dominant manual-tracking incumbent (huckleberrycare.com)
- Smart Sleep Coach by Pampers — P&G-backed, 3-min assessment + tailored adaptive plan covering toddlers, real-time schedule adjustments (smartsleepcoach.com)
- Lovebug — certified pediatric sleep consultant-led app with live coaching calls through toddler years (getlovebug.com)
- Napper — adaptive sleep schedule that adjusts to natural rhythms, strong App Store presence (napper.app)
- Happy Baby — learns from sleep behavior and creates adaptive schedules that evolve as the child grows (aumio.com top-6 roundup)

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Get my kid to bed faster tonight without burning my evening, with someone telling me one thing to try differently. Classification: naturally recurring (bedtime happens every single night for years).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong. The core metric is bedtime minutes trending down, with visible week-over-week reduction and confirmed/rolled-back experiments, the parent literally sees themselves getting better at bedtime.
- Autonomie (sentiment d'être en contrôle): Strong. The app explicitly refuses templates, builds on what the family already does, lets the parent try-or-skip each suggested move, and rolls back if it doesn't work. No shame, no streak, no prescriptive consistency lecture.
- Lien social (sentiment d'être connecté à d'autres): Absent. Single-parent use, no partner sync, no community, no comparison to other families (deliberately).

**Boucle d'habitude**
- Déclencheur: 7:30pm, the start of the bedtime routine, a fixed daily life moment. INTERNAL (the kid and the clock are the cue, the app also pings but the real trigger is the routine starting). Also internal cue on bad nights, the parent reaches for the app when bedtime cracks (H3).
- Routine: Walk through routine steps on lock screen, then a single 1 to 5 tap after bedtime. One tap, sub-friction.
- Récompense: Immediate (Y), the parent gets the next step on the lock screen during bedtime, and the post-rating reward is the sense that tonight's pain produced signal toward tomorrow's smaller routine. Slower reward is the trending-down minutes.
- Push reliance: Push is used (evening ping at routine start) but is not the primary driver, the internal cue is the kid's bedtime itself. Healthy.

**Verdict line**
Two of the three angles pass cleanly and the third nearly does. The job recurs nightly for years (clear pass), competence and autonomy are both Strong by design (pass), and the habit loop has an internal cue tied to a fixed life moment plus an immediate in-loop reward (pass). The one structural weakness is the absence of social tissue, which the spec treats as a feature, not a bug, fair, but it means the only thing holding the user is personal progress, so the suggestion engine has to actually work or H2 collapses and retention with it.

**What needs to change for STRUCTURAL_RETURN**
N/A, verdict is STRUCTURAL_RETURN. Watch-outs to track in Phase 2: what happens when bedtime is "solved" and minutes plateau, does the user churn (the job becomes one-shot-ish per kid-phase) or does a new wrinkle bring them back? And, given lien social is Absent, is the single-parent install pattern (open question 3 in product_log) a retention risk if the non-installing partner breaks the routine?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

The spec has a sharp, emotionally resonant problem statement and a clear anti-positioning ("not sleep training, no shame, no streaks"). The persona is buildable and the product mechanic (one-tap log, one-thing-at-a-time nudge) is concrete. But the core engine, the "library of moves" plus the data-driven suggestion, is hand-waved, and three central trust questions (does the advice work, does it survive a co-parent, why trust an app over a book) are unanswered. The product is credible as a pitch, not yet credible as a nightly habit.

**Dangerous assumptions:**
- The suggestion engine can produce advice that's actually better than what a tired parent would Google or pull from a sleep book. Cheap test: Wizard-of-Oz it with 10 parents for two weeks, human-curated nudges, measure whether parents say the advice felt personal and worth trying.
- Parents will log a 1-5 rating every night for 4+ weeks, even on the bad nights (when logging feels like rubbing salt in the wound) and the good nights (when they forget because bedtime actually worked). Cheap test: SMS-based 1-tap rating with 20 parents for 2 weeks, measure raw adherence with zero product polish.
- Bedtime is a solo-parent decision surface. If the non-installing partner ignores the nudges or contradicts the routine, the app's prescriptions collapse. Cheap test: 5 co-parent interviews, ask who decides bedtime changes and what happens when one parent disagrees with a suggested change.
