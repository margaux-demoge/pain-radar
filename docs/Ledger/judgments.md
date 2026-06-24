# Ledger — judges verdicts

## benchmark-scanner: `EMERGING`

The mental-load / emotional-labor tracker space has 3-4 serious players (Balance Together, Better Share, Tend Task) but they all frame as couples tools where both partners participate, not as a private solo journal for the over-functioning partner. Ledger's wedge (one-sided, private, no partner-facing surface, journal not scorecard) is genuinely uncrowded. Risk: the category is heating up post-2024 with several launches, window is real but closing. The bigger threat is not direct competition but the cultural narrative ("scorekeeping harms relationships") that therapists actively warn against, which Ledger must reframe head-on.

**Top competitors:**
- Balance Together (balancetogether.app), structured weekly check-ins + AI insights on mental load, designed for singles and couples, active 2025-2026, https://www.balancetogether.app/blog/mental-load-test
- Better Share (bettershareapp.com), explicitly framed around mental load tracking to reduce resentment, couples-facing, active, https://bettershareapp.com/
- Tend Task (tendtask.com), task-sharing app with AI guidance specifically for couples' invisible labor, active, https://tendtask.com/relationship-app-for-couples-mental-load-solution/
- Ohai.ai, AI household sidekick handling delegation and reminders, adjacent angle (logistics not emotional initiation), active, https://www.ohai.ai/blog/mental-load-checklist/
- Fair Play (card-deck + app ecosystem from Eve Rodsky), the cultural reference point for mental load division, couples-facing not solo-journal

## retention-validator: `WEAK_RETURN`

Job is naturally recurring (logging tiny relational acts that happen daily: texts, plans, check-ins), so need recurrence passes. But SDT is thin: compétence is absent (no progress, no mastery, explicitly no streaks/gamification), autonomie is strong (private, user picks what counts, product never prescribes), lien social is absent by design (partner never sees it). The habit loop is weak: cue is internal ("I just initiated something") but the routine's reward is delayed two weeks until the picture appears, so day-to-day logging has no immediate payoff. With no notifications by design, the loop depends entirely on the user's own discipline to log micro-events that feel trivial in the moment. Once the user has their picture and either has the conversation or lets resentment go, the job is effectively done, pushing this toward one-shot resolution despite the recurring surface activity.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Ledger has a sharp, well-articulated pain and a clearly defined persona, with prose that genuinely sounds like the target user. But the core mechanic (manually logging your partner's behavior in a private journal) sits on three untested assumptions: that hyper-vigilant logging soothes rather than feeds resentment, that the user will keep logging when they're already exhausted from over-functioning, and that "data" actually de-escalates the conversation rather than weaponizing it. The spec acknowledges some of this in product_log but hasn't resolved it. Positioning is strong, mechanism is shaky.

**Dangerous assumptions:**
- Logging every imbalance soothes resentment rather than amplifying it. The whole product depends on this, but the opposite is equally plausible: tapping a counter every time you text first turns a vague unease into a daily grievance ritual. Cheap test: 2-week paper diary with 10 target users, measure resentment delta pre/post with a 1-5 self-report.
- The over-functioning partner, who is already doing all the cognitive labor, will reliably add a new micro-task (tapping the log) to their day. The same exhaustion that creates the problem predicts they'll drop logging by week 2. Cheap test: dry-run with an SMS bot or Notes shortcut for 14 days, measure log frequency without any UI investment.
- Showing a partner 'the picture' de-escalates rather than detonates. 'I tracked you for two weeks and here's the data' reads as surveillance to most partners regardless of framing. Cheap test: show 10 non-target partners the mock picture + suggested sentence, ask 'how would you feel if your partner showed you this'.
