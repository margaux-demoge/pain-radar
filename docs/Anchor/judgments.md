# Anchor — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The exact problem Anchor targets (interrupt the anxious-attachment spiral before sending a regrettable text) is already named, productised, and shipping in at least four direct competitors as of 2025-2026. Don't Spiral and Attached map onto Anchor's pitch almost word-for-word (including in-the-moment trigger intervention, pattern recognition, privacy stance). The space is not a graveyard (no significant shutdowns surfaced) but it is crowded with well-positioned AI-coach apps building exactly this wedge. Anchor's reflection-not-reassurance mechanic is a real angle, but every competitor already claims something close.

**Top competitors:**
- Don't Spiral (dontspiral.app) — AI coach for ROCD, jealousy, overthinking, with named session types like 'spiralling' and 'conversation prep'; explicitly 'helps you avoid sending reactive messages.' Active, iOS+Android.
- Attached (attachedapp.com) — #1 anxious-attachment app, ships 'Trigger Cards' for real-time in-moment reactions plus CBT/DBT/ACT/IFS frameworks. Active, well-funded by MWM.
- Bestie AI (bestieai.app) — Position yourself: 'text Bestie instead of your partner' when spiraling. Direct substitute for Anchor's core JTBD.
- Wellness AI / Ash (wellness-ai.app) — Ships cognitive restructuring for jealousy, defusion for anxious thoughts, distress tolerance modules. Active.
- Reframe (joinreframeapp.com) — Combines breath + cognitive reframing for the panic spiral; publishing content explicitly on 'three-dot dread' and partner texting anxiety.

## retention-validator: `STRUCTURAL_RETURN`

The job (catch an anxious-attachment spiral before sending a regrettable text) recurs naturally for the target user since spirals are described as a recurring loop, not a one-shot crisis. The habit loop has a strong internal cue (the somatic moment of a spiral triggered by partner behavior) and immediate reward (seeing the thought structured back, slowing the urge). SDT is mixed: compétence is Strong via pattern recognition over weeks ("fifth time this month"), autonomie is Strong (private workspace, no advice, no reassurance), lien social is Absent by design. Two of three angles clearly pass; verdict is STRUCTURAL_RETURN with the caveat that retention depends on spiral frequency holding up and on the intervention not feeling like cognitive overload mid-spiral (open question 1).

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

The persona is sharp and the problem narrative is vivid, but the product makes two big bets the spec doesn't defend: (1) that someone mid-spiral has the cognitive bandwidth to type out a raw thought and read a structured reflection back, and (2) that "mirroring" won't feel cold, robotic, or worse, validate the loop. Trust, privacy, and the line between Anchor and a therapist are also under-addressed. The positioning is credible but several load-bearing assumptions are unvalidated, putting it in WEAK_ON_ASSUMPTIONS territory. Simulated user: Maya, 24, Brooklyn, in a 2-year relationship, uses How We Feel + Notes app voice memos + Stutz/Baum TikToks, mildly skeptical of "AI for feelings" apps after trying Replika and Wysa. Interview score: 3 ANSWERED / 4 PARTIAL / 3 UNANSWERED across 10 questions covering in-the-moment usability, mirror vs reassurance risk, privacy of partner-identifying text, differentiation from journaling apps, what happens when the spiral IS justified, dependency risk, cost/willingness to pay, why type instead of voice, what Anchor does that a Notes app + therapist text doesn't, and whether pattern callbacks feel insightful or judgmental.

**Dangerous assumptions:**
- Users mid-spiral will type out the thought rather than act on it. The cognitive load assumption is unvalidated (log Q1 flags this). If typing feels impossible in the activated state, the whole intervention model collapses. Cheap test: 5 anxious-attachment users try a paper/Notes version during a real spiral and self-report whether typing helped or felt like one more obstacle before the text they sent anyway.
- Structured mirroring interrupts the loop rather than reinforcing it. The spec assumes seeing the spiral named breaks the hypnosis, but it could equally crystallize the fear ('yes, exactly, she IS pulling away'). Cheap test: Wizard-of-Oz 10 sessions with two prompt variants (pure mirror vs mirror+gentle challenge) and measure post-session 'did you send the text' and 'do you feel more or less certain of the fear'.
- Users will entrust an app with partner-identifying, jealous-thought content they wouldn't put in iCloud Notes or say to a therapist. No privacy/trust story in spec. If the target is privacy-sensitive (they want a 'private workspace, not another therapist'), the data handling story is load-bearing. Cheap test: landing page with privacy-forward copy vs neutral copy, measure email signups from r/AnxiousAttachment traffic.
