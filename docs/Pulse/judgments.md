# Pulse — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The couples-intimacy-conversation category is dense and well-funded. Paired, Lasting, Coral, Blueheart, Ferly, Spicer, Coelle, OurRitual, Lovewick all play in or near Pulse's wedge, and Gottman card decks own the offline mental model. Most competitors are solo-content or single-user-driven; Pulse's two-sided synchronous "shared room with partner-invite gate" framing is less crowded than the broader category, but the user discovery and "is this another couples app" objection is already heavy. Rosy (women's sexual wellness) shutting down Nov 2025 after 7 years is the one clear failure signal; otherwise the failure graveyard is small but quiet, which often means private pivots rather than true survival.

**Top competitors:**
- Paired — daily question prompts for couples, broad emotional comms, light on sex specifically, active and category leader (paired.com)
- Coral — sex-specific audio exercises and self-guided programs for desire/performance issues, ~$15/mo, active (camillestyles.com review)
- Blueheart — evidence-based sex therapy exercises for couples with mismatched desire, active (dazeddigital.com)
- Ferly — guided practices and 1:1 expert calls, 500k users, originally women-focused now positioned as couples sex therapy, active (apps.apple.com/ferly)
- Coelle — guided audio intimacy sessions explicitly designed around desire-level differences, active (coelle.app)
- Spicer — playful intimacy ideas, shared matches and challenges between partners, active (spicer.app)
- Lasting — Gottman-method structured therapy programs, broader than sex but covers it, active (choosingtherapy.com)

## retention-validator: `WEAK_RETURN`

The job (open and sustain hard intimacy conversations with a partner) is occasional rather than naturally recurring, it has no daily/weekly trigger baked into life. SDT is mixed: relatedness is Strong (the whole product is two-person), competence is Weak (no progression visible, sessions deepen but no mastery signal), autonomy is Strong (no streak, no nag, pace is user-led). The habit loop lacks a clear internal cue, the spec explicitly refuses streaks and nags, so retention depends on couple-initiated re-opening or external push, which is fragile. Two angles partially fire (relatedness + autonomy) but only one of the three retention pillars (SDT) clearly passes, the cue and recurrence are weak.

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Help a couple have the intimacy conversation they keep failing to start on their own, by providing a safe shared format.
Classification: occasional (recurs but unpredictably, tied to relational tension cycles, not to a daily life trigger)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak, sessions deepen over time but the spec shows no visible progression, no mastery feedback, no sense of "we are getting better at this" surfaced to the couple.
- Autonomie (sentiment d'être en contrôle): Strong, explicit refusal of streaks and nags, pace fully user-led, "if either of you pauses, the app waits".
- Lien social (sentiment d'être connecté à d'autres): Strong, the entire product is a two-person room, the partner is the relationship, not a side feature.

**Boucle d'habitude**
- Déclencheur: not specified in the spec, presumably the felt tension between sessions or a scheduled cadence the couple sets. EXTERNAL by default if push is the only re-entry vector, otherwise unclear.
- Routine: a ten-minute guided exchange, each partner answers the same question privately, then sees the other's answer with a short prompt.
- Récompense: seeing your partner's answer side by side and being given language for the real conversation, immediate Y, the in-app reward fires within minutes.
- Push reliance: the spec is silent on cues, and explicitly rejects streaks/nags, so unless an internal cue is designed (a felt moment in the week that pulls the couple back), retention will lean heavily on push or on the wedge partner re-initiating, which is a single point of failure.

**Verdict line**
Lien social and autonomie pass cleanly, those are real structural pulls. But the underlying job is occasional rather than recurring, and the spec does not name a cue that brings the couple back, it actually removes the usual external pulls (no streak, no nag) without replacing them with an internal cue. One angle of three clearly passes, hence WEAK_RETURN: Pulse can launch and the first session has strong magic, but week 4+ is exposed.

**What needs to change for STRUCTURAL_RETURN**
- What internal cue, in a couple's week, will reliably pull them back to open a new session, given that streaks and nags are off the table by design?
- Is there a cadence the couple commits to together at setup (e.g. "Sunday night session") that converts an occasional job into a recurring ritual?
- What progression signal can the couple feel across sessions, so that competence becomes Strong, the sense of "we are unlocking territory we could not reach before"?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Pulse has a sharp, well-articulated problem and a credible wedge (the partner already doing the reading), and the product experience is unusually specific about what it refuses to be. But the entire product hinges on the second partner showing up, and the spec offers no mechanism, no language, no proof that the invite converts at 50%. Competitive differentiation versus Paired/Lasting/Gottman is unaddressed, and the coercion/safety risk flagged in the log has no product answer. Simulated interview: Sarah, 32, Lyon, in a 6-year relationship, has read Mating in Captivity, tried Paired with her partner who installed it and never opened it again. Skeptical, time-poor, has been burned by "couple apps" before. Q1 "Why would my partner, who avoids this conversation, accept a link from me about sex?" PARTIAL, spec says framing matters but gives no actual invite mechanic or copy. Q2 "I tried Paired and he ghosted it after week one, what's different here?" UNANSWERED, no competitive wedge articulated to the user. Q3 "Ten minutes, side-by-side answers, then a prompt, what stops this from becoming the same fight in a nicer wrapper?" PARTIAL, spec asserts gentleness but does not show the de-escalation mechanism. Q4 "Who writes these questions and why should I trust their judgment about my marriage?" UNANSWERED. Q5 "What happens the first time one of us answers something the other finds devastating?" UNANSWERED, no rupture-repair design. Q6 "I'm the one who downloaded it, isn't this just me dragging him into therapy-lite again?" PARTIAL, spec acknowledges the framing problem but does not solve it. Q7 "How do you know we're 'ready' for harder questions, are you reading our answers?" UNANSWERED, pacing logic unspecified, privacy implication unaddressed. Q8 "If he uses it to pressure me into saying yes to things, what does the app do?" UNANSWERED, log flags this, spec is silent. Q9 "We pay how much, and for how long before this 'works'?" UNANSWERED, no business model. Q10 "If the whole point is the conversation happens off-app, why do I need to keep the app?" UNANSWERED, retention logic contradicts stated value. Score: 0 ANSWERED, 4 PARTIAL, 6 UNANSWERED.

**Dangerous assumptions:**
- The invited partner will accept and complete a first session at 50%+ — the spec offers no invite mechanic, no copy, no friction-reducing design, and the log itself flags this as make-or-break. Cheap test: run a fake-door landing page where one partner enters their partner's number and we measure actual reply/accept rate on a plain-text invite.
- Couples in the awkward-not-crisis zone will pick Pulse over Paired/Lasting/Gottman card decks they already know about — the differentiated wedge is asserted (refusal of content, side-by-side format) but never tested. Cheap test: 10 user interviews with target couples showing the Pulse one-pager against a Paired screenshot, ask which they'd try and why.
- The side-by-side reveal of private answers will de-escalate rather than detonate — spec assumes gentleness emerges from format, but offers no rupture-repair design for the first time an answer lands badly. Cheap test: Wizard-of-Oz 5 couples with a Google Form pair and a human writing the prompt, watch what happens when answers diverge.
