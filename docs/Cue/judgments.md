# Cue — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "couples app with prompts to scaffold hard conversations, including sex" category is densely populated and well-funded, with Paired, Coral, Blueheart, Lasting (Talkspace), Relish, and Ultimate Intimacy all live and actively marketing therapist-curated prompts and intimacy exercises. Several are explicitly built around mismatched desire and two-sided pairing (Coral, Blueheart, Kindu, Xplore, Spicer). Failure signal exists (Relish stagnant, Pillow stuck bootstrapping after VC passed) but the dominant pattern is consolidation, not graveyard. Cue's differentiator (small async cues, no gamification, partner-paired) overlaps directly with Paired and Coral's daily prompt loops.

**Top competitors:**
- Paired, daily therapist-backed prompts and quizzes for couples, including sex and mismatched libido modules, active and dominant (paired.com)
- Coral, sexual wellness app for couples with guided exercises, daily prompts and 300k+ members, explicitly targets the same intimacy conversation gap (getcoral.app)
- Blueheart, sex-therapy-led app for couples, markets directly to mismatched desire and disconnection, two-sided usage (blueheart.io)
- Lasting (Talkspace), relationship counseling app, acquired 2020, evidence-based sessions including intimacy modules (talkspace.com)
- Kindu, longest-running 'awkward sex things' prompt app with double-blind matching to avoid embarrassment, directly the conversation-scaffolding wedge Cue claims (kindu.us)

## retention-validator: `WEAK_RETURN`

The job (start the avoided sex conversation with your partner) is occasional and arguably finite — once the "real conversation" happens (H2 target at 8 weeks), the core job is done. Psychological needs: relatedness is strong (paired with partner, intimate exchange), but compétence and autonomie are weak/absent (no progress signal, scaffolded library limits autonomy). Habit loop is fragile: cue is largely external (partner sends, or app suggests via push), reward is delayed (partner answers when they have words, no read-receipt urgency by design), no internal cue tied to a daily life moment. Only relatedness clearly passes; the product is structurally designed to resolve itself.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Cue has a sharp, well-articulated problem and a precise persona, and the cue-format mechanic feels emotionally credible. But the spec collapses on the two-sided install problem: asking a partner to install a sex-conversation app is itself the bomb the product claims to defuse. Trust, privacy, and what-happens-when-answers-hurt are unaddressed. The positioning is solid; the operational reality of getting two people in and keeping them honest is not.

**Dangerous assumptions:**
- The pairing invite is survivable. Spec assumes the initiating partner can ask the other to install 'a sex app' without that ask being the same bomb the product is meant to avoid. If the invite itself feels accusatory, Cue never gets past install. Cheap test: prototype 5 invite flows (SMS copy, in-app, neutral framing) and run a 10-person wizard-of-oz ask-your-partner test, measure who actually pairs.
- Written, asynchronous answers to intimacy questions are answerable, not avoidable. The spec assumes removing read-receipt pressure unlocks honesty, but writing a sentence about desire to your partner-of-7-years may be HARDER than saying it. No evidence cited. Cheap test: send 10 target-segment couples a single cue via Google Form, measure 72h response rate and qualitative friction.
- The receiving partner's answer won't make things worse. Spec explicitly says 'a product where one ghosts makes things worse' but offers no mechanism for when an answer lands badly (hurt, defensiveness, escalation). No safety rails, no therapist-in-the-loop, no exit ramp. Cheap test: interview 5 couples therapists on failure modes of written intimacy disclosure and what guardrails they'd require before endorsing.
