# Span — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

LDR is one of the most-attempted couples-app niches: at least 7 active products (Cupla, Flamme, Couple Joy, Locket, Rave, Between, Paired) and a deep graveyard (Couple, Meta's Tuned, Avocado, Happy Couple, Official). Most competitors already ship countdowns, synced moments, shared calendars, and prompt decks — Span's literal feature surface is covered. The differentiator can only be the "span has a shape, app goes quiet during visits" framing, which is positioning rather than a feature moat. Past failures cluster around two-sided activation and engagement decay once novelty passes, exactly the risks already flagged in product_log.md.

**Top competitors:**
- Cupla — time-zone-aware scheduling, reunion countdown widget, shared to-dos; explicitly markets to LDR couples (active, updated Dec 2025). https://cupla.app
- Flamme — daily questions, Gottman card decks, AI love coach, LDR-positioned; featured TechCrunch/Guardian (active). https://flamme.app
- Couple Joy — memory-first: shared photos, pinned map moments, micro-questions, widget; newest entrant explicitly framed as LDR intimacy (active, 2026). https://techweez.com/2026/06/19/couple-joy-long-distance-relationship-app-review/
- Locket — home-screen widget for partner photo updates; dominant 'feel close on a Tuesday' player (active, mass-market). 
- Rave — synced Netflix/YouTube watch parties with chat, the de facto shared-movie-night solution (active). 
- Paired — therapist-designed daily prompts and quizzes for couples, not LDR-specific but heavily used by them (active). 
- Between — long-running couples space with shared calendar, memory box, countdown; the original template (still active). 

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Help a long-distance couple feel like they are building something together during the stretch between visits, instead of just waiting it out.
Classification: naturally recurring (the underlying need to feel close recurs daily/weekly throughout a multi-month distance, and re-recurs each time a new distance begins)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. There is a "trail" of fifteen or twenty things built by visit-time, which gives a sense of accumulation, but no explicit mastery or skill progression for the user as an individual.
- Autonomie (sentiment d'être en contrôle): Strong. The whole framing is reclaiming agency over the gap, choosing the shape of the distance, deciding which moments to do, owning logistics that were previously implicit.
- Lien social (sentiment d'être connecté à d'autres): Strong. The entire product is relatedness with one specific person, shared moments, synced playback, question reveals, photo trades, with the explicit aim of feeling close on a Tuesday at 9pm.

**Boucle d'habitude**
- Déclencheur: the felt drift during the middle stretch (Tuesday 9pm, nothing to say), plus the partner completing their side of a shared moment. INTERNAL primarily, with a secondary external cue when the partner acts.
- Routine: open Span, do your half of a shared moment (answer the question, send the Tuesday photo, start the synced movie), or check the next logistic.
- Récompense: immediate sense of having added a small thing to the shared record, and the social signal of the partner's contribution waiting. Immediate Y.
- Push reliance: not heavy. The cue is mostly internal (the drift, the partner's pending turn), so retention does not collapse if notifications are off, though partner-action pings would clearly reinforce the loop.

**Verdict line**
Two of the three angles pass cleanly: the need recurs naturally across the entire distance period and re-triggers at each new separation (H3 is even built around this), and the habit loop has both an internal cue (the felt drift) and an immediate reward (a shared moment added to the trail). The psychological side is strong on autonomie and lien social though weak on compétence. The serious open risk is two-sided activation, if only one partner engages, the loop dies, which is exactly what H1 is set up to test.

**What needs to change for STRUCTURAL_RETURN**
N/A, verdict is STRUCTURAL_RETURN. Worth flagging for the team: what happens to retention during the visit itself when Span goes quiet, and does the "reopen at next distance" behavior (H3) actually fire without an external nudge, given that internal cues fade once the couple is co-located?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Span has a clear persona (20-32 LDR, mid-stretch) and a distinctive positioning (shape the gap, leave a trail, not a countdown). Section 2 paints the experience vividly, which answers many behavioral questions. However, the two-sided activation problem, the partner-buy-in question, and the "why this won't end up in the LDR app graveyard" are all flagged in the log as TBD, and they are exactly the questions a skeptical user would press hardest on. Simulated user: Maya, 26, grad student in Boston, partner in Berlin, currently using iMessage + Google Calendar + Netflix Party + Marco Polo, tried Couple once and both stopped after two weeks. Mildly skeptical, tired of being pitched LDR apps. Q1 "Why is this different from Couple or Between, which we already tried and abandoned?" UNANSWERED. Q2 "My boyfriend won't download a third app, he barely opens iMessage on time, how do I get him in?" UNANSWERED (log flags it). Q3 "Three or four moments across six weeks sounds thin, what fills the Tuesday 9pm void you describe in the problem?" PARTIAL. Q4 "Who picks the moments, the app or us? If it's the app, how does it not feel generic?" UNANSWERED. Q5 "We're 6 hours apart, how does synced movie night actually work when I'm asleep?" PARTIAL (log Q2). Q6 "What stops this from becoming the anxious partner nagging the other to do the questions-game?" PARTIAL (H1 names the risk, no mechanism). Q7 "When the visit gets postponed (it always does), what happens to the shape?" UNANSWERED. Q8 "You say Span goes quiet during the visit, but if I stop opening it for two weeks why would I come back?" PARTIAL (H3 measures it, doesn't solve it). Q9 "The 'logistics it holds' sounds like a shared calendar with extra steps, what's actually different?" PARTIAL. Q10 "If the relationship ends, what happens to the record of fifteen things we made, and does that fear stop me from investing in the first place?" UNANSWERED. Score: 0 ANSWERED, 5 PARTIAL, 5 UNANSWERED. The positioning prose is strong but the spec hasn't survived the two-sided adoption stress test or the differentiation-from-graveyard test, both of which the team has already flagged but not resolved.

**Dangerous assumptions:**
- Two-sided activation: that both partners will install and engage. The whole H1 metric (60% both-partner engagement) is gated on this, and the spec has no invite/onboarding mechanic that makes the second partner's first session valuable without a full install. Cheap test: prototype a one-sided invite where partner B engages via SMS/web link for the first shared moment, measure pull-through to install on a waitlist of 20 couples.
- Differentiation from the LDR app graveyard (Couple, Between, Avocado, Lasting all died). The spec asserts Span is different because it shapes the gap rather than mirrors a calendar, but doesn't name the specific churn driver it avoids. Cheap test: 10 interviews with ex-users of Couple/Between asking why they stopped, then check whether Span's mechanics address those churn reasons or repeat them.
- That curated 'three or four moments across six weeks' is the right density. Too few and it doesn't fill the Tuesday 9pm void the problem statement promises to address; too many and it becomes the nagging ritual H1 warns against. Cheap test: concierge MVP over iMessage with 5 couples for one month, manually suggest moments at varying cadences, measure both partners' self-reported closeness and irritation.
