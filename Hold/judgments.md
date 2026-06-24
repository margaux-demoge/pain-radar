# Hold — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "remember the people you love" space is densely populated: birthday-reminder apps (Hip, birthdays.app, Birthday AI), full personal CRMs (Monica, Dex, Clay, Social Compass, UpHabit), and even niche apps for grief/illness check-ins (Follow the Nudge, Lifeboat) already cover Hold's three pillars (timed reminders, suggested gestures, asymmetric/grief reminders). The graveyard is also real (Etacts, ConnectedHQ, Conduit) and points to a recurring failure mode: people resist running friendships like a CRM, retention collapses once the novelty fades. Hold's wedge (3-days-ahead + memory log + asymmetric reminders) exists in pieces across these competitors, the differentiation has to be sharper than "smarter Facebook birthday reminder."

**Top competitors:**
- Hip — birthday/anniversary reminders with curated gift suggestions and cards, active iOS app (https://www.hip.app/)
- Dex — personal CRM with keep-in-touch reminders and per-contact cadence, well-funded and active (https://getdex.com/)
- Monica — open-source personal CRM logging birthdays, gifts, conversations, life events; mature and active (https://www.monicahq.com/)
- Social Compass — personal CRM explicitly designed for friendships/family (no sales features), with overdue cadences (https://socialcompass.social/)
- Follow the Nudge — text reminders to check in with grieving/ill friends at anniversaries, directly overlaps Hold's asymmetric-reminders wedge (https://www.psu.edu/news/impact/story/app-wpsu-offers-text-reminders-check-grieving-friends-family)

## retention-validator: `WEAK_RETURN`

The job (remember dates that matter for people I love) is naturally recurring at the calendar level, since birthdays/anniversaries cycle yearly and a real network produces multiple dates per month. But the user-side action is thin and almost entirely externally cued: the 3-day push is the only thing pulling the user back. There is no internal cue ("I'm bored, let me open Hold"), and the reward is mainly relief from guilt, felt only on the few occasions when a date is near. Competence is weak (no real sense of mastery), autonomy is weak (the app is in charge of timing), and relatedness is indirect (the connection is to the friend, not through the app). The habit loop closes externally via push, with no second loop pulling users in between dates. Setup is a one-shot data-entry burst, and after that the app sits silent until the next ping. STRUCTURAL_RETURN would require a between-events reason to open the app (the relationship log being browsed, a weekly digest, a social or reflective ritual). Verdict: WEAK_RETURN — survives because dates do recur, but retention rides almost entirely on push notifications, which is fragile.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Hold has a sharp emotional hook (shame of forgetting) and a clear differentiator (3-day-ahead + suggested action + memory of past gestures), which gives it more positioning strength than a generic reminder app. But several core assumptions remain unvalidated: that users will do the upfront work of seeding people/dates/notes, that the "suggested action" will feel personal rather than generic, and that the asymmetric reminders (grief, illness) won't feel creepy or like surveillance. The persona Sarah, 32, NYC, already uses iOS Calendar + Facebook + a Notes list, would push back hard on data entry cost and on whether a third app earns a permanent home screen slot.

**Dangerous assumptions:**
- Users will do the upfront work of adding people, dates, and context-notes before the app proves value. Cheap test: a paper prototype where 5 target users try to seed 10 relationships in under 5 minutes; measure drop-off and completeness.
- The 'suggested action' (e.g. 'last year you sent a voice note') will feel personal and continuous, not generic or LLM-flavored. Cheap test: show 5 users hand-crafted vs generic suggestions side by side and ask which one they'd actually act on, and whether they'd trust the app to write them.
- Asymmetric reminders (dad's death anniversary, friend's surgery) feel caring rather than creepy/surveillance. Cheap test: interview 5 people about whether they'd trust an app to remind them of a friend's grief anniversary, and whether they'd worry the friend would find out they used an app to remember.
