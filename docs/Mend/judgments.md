# Mend — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "AI helps you write to your partner after a fight" wedge is already populated by at least 5 active products (Repair, Relationship Ref, CoupleWork, Ember, TextMeI), plus a deep bench of structured couples apps (Lasting/Talkspace, Paired, Relish, OurRitual) that own the "repair ritual" frame. A 2025 Marriage.com stat cited 44% of adults (65% of millennials) have already used AI for relationship advice, so generic ChatGPT is also a default substitute. Mend's specific wedge (one sentence to break a three-day silence + longitudinal log of past repairs) is defensible but narrow, the team needs to articulate why Repair's "AI-guided Repair Session" doesn't already eat this use case.

**Top competitors:**
- Repair (startarepair.com), AI-guided Repair Sessions explicitly framed as post-conflict reconnection, the closest direct competitor — https://www.startarepair.com/
- Relationship Ref: AI Mediator (iOS), analyzes conversations and suggests de-escalating responses during/after conflict — https://apps.apple.com/us/app/relationship-ref-ai-mediator/id6752880675
- CoupleWork: AI Couples Coach, positions as 'first AI relationship coach,' affordable alternative to counseling — https://apps.apple.com/us/app/couplework-ai-couples-coach/id6504302751
- Ember: AI Relationship Coach, AI coach 'Em' built by a real couples coach, communication + connection focus — https://apps.apple.com/us/app/ember-ai-relationship-coach/id6744977130
- Lasting (Talkspace), Gottman-based modules including a 'Repair' track, 3M downloads, owns the structured-program frame — https://play.google.com/store/apps/details?id=com.lasting.lasting

## retention-validator: `WEAK_RETURN`

The job (break a specific silence after a fight) is occasional and unpredictable, not naturally recurring. SDT scores weakly: competence is absent (you don't "get better" at fighting), autonomy is weak (you mostly accept a draft), social connection is indirect (mediated through your partner, not in-app). The habit loop has an internal cue (the silence) but the cue is rare and aversive, and there's no reason to open Mend outside of an active rupture except the history log, which is speculative (H3 target only 30%).

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

The problem framing is vivid and the persona is constructible (cohabiting late-20s, post-fight freeze), and the product offers a concrete, low-friction mechanic (3-minute intake, one sentence out). But the spec leans heavily on three unvalidated bets: that frozen people will actually open an app mid-silence, that an AI-drafted sentence won't feel like a betrayal if discovered, and that "both partners lean in slightly" can be assumed when by definition one is the one who needs to break first. Interview simulation: Q1 problem recognition, Q2 mechanic clarity, Q3 register matching, Q5 history log value are ANSWERED or close. Q4 mid-silence behavior, Q6 AI disclosure, Q7 single-user product needing two-side buy-in, Q8 privacy of raw venting, Q9 differentiation vs ChatGPT, Q10 what happens when the sentence fails, are PARTIAL or UNANSWERED. Score ~4 ANSWERED, 3 PARTIAL, 3 UNANSWERED, with two of the top-3 dangerous assumptions UNANSWERED. Not built on sand, but the central behavioral bet (will they reach for it while frozen) is the same question the product log already flags as TBD #1, which is exactly where validation must happen before build.

**Dangerous assumptions:**
- Users will actually open Mend while mid-silence. The whole pain is paralysis, and reaching for a tool is itself a form of action they're failing to take. If they only open it after they've already started reconciling, the product is a journal, not a bridge. Cheap test: run a 2-week diary study with 10 cohabiting couples, ping them daily, ask 'are you in a cold spell right now, would you open an app like Mend in the next hour'. Measure intent-to-open during the actual frozen state, not retrospectively.
- An AI-drafted opening sentence will feel authentic enough to send, and won't poison the relationship if the receiving partner ever learns it was AI-assisted. The spec waves at 'your register' but doesn't address the disclosure problem at all. Cheap test: show 20 people in established relationships 5 AI-drafted reconciliation openers vs 5 human ones, ask which they'd send and how they'd feel if their partner had sent the AI one to them.
- Mend works as a single-user product even though repair is two-sided. The 'not for' carve-out says both must lean in 'even slightly', but the product only equips one. If partner B reads the message as manipulative or scripted, Mend made the silence worse. Cheap test: 5 paired interviews where partner A drafts with Mend and partner B reacts blind, measure whether B feels closer or more suspicious.
