# Tide — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "mood lens on the cycle, not fertility" angle is now a well-occupied category. Moody Month, Stardust, Peony, Belle, HealCycle and Harmony all explicitly market psychological insight, daily mood logging, and phase-based pattern reads, several with the same "AI learns your personal patterns" framing Tide proposes. Clue and Flo have also shipped phase-mood subfeatures inside the giants. No meaningful graveyard surfaced, the failure mode here is being a feature, not a startup.

**Top competitors:**
- Moody Month — daily hormone/mood tracker explicitly positioned around mental health across cycle phases, actively updated 2025 (https://moodymonth.com/app)
- Stardust — privacy-first cycle tracker with AI-generated personalized phase trends and mood/hormone reads, strong design wedge (https://apps.apple.com/us/app/stardust-period-pregnancy/id1495829322)
- Peony — voice-first mood tracker whose AI surfaces lines like 'your mood typically dips 3 days before your period' (https://www.heypeony.com/blog/period-mood-tracker)
- Belle Health — cycle app explicitly not for fertility, focused on mental health, energy, behavior with journaling tools (https://bellehealth.co/female-health-app/)
- Clue Cycle Phase Insights — six-subphase breakdown with mood/focus tracking, shipped by the category incumbent (https://helloclue.com/articles/about-clue/discover-cycle-phase-insights-understand-your-body-feel-empowered)

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Help me understand why I feel the way I feel today by tying it to where I am in my cycle, so today's mood stops feeling like a verdict on my life.
Classification: naturally recurring (daily, the cycle itself is a permanent recurring biological clock, and mood happens every day)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong, the product explicitly builds a "cycle profile" over time, users see themselves get more legible to themselves cycle after cycle, mastery of one's own pattern is the core promise.
- Autonomie (sentiment d'être en contrôle): Strong, the framing is explicitly anti-extractive (no feed, no supplements, no community pressure), and the payoff is "you can plan: hold the hard conversation for next Tuesday", which is autonomy over one's calendar and choices.
- Lien social (sentiment d'être connecté à d'autres): Absent, by design, Tide is a private mirror with no social layer.

**Boucle d'habitude**
- Déclencheur: morning, the user wakes up and wants to know what kind of day this is going to be, plus a daily push with the read, INTERNAL (the cue is the felt mood of the morning itself, reinforced by an external push)
- Routine: 30 second check-in with two or three real questions, then read the day's short interpretation
- Récompense: immediate, a one-line read that reframes today's feeling as a phase, not a verdict, felt within seconds, Y
- Push reliance: present but not exclusive, the internal cue (waking up unsure how you feel) is strong enough that the loop survives push being off, especially for the introspective-journaller wedge.

**Verdict line**
Two of three angles pass clearly and the third passes as well. The job recurs daily and forever (cycle + mood are both naturally recurring), two of three psychological needs are Strong (compétence via the growing cycle profile, autonomie via private planning leverage), and the habit loop has an internal cue (morning self-check) with an immediate reward (the day's read). The main structural risk is not retention but cold start: the read needs to become personally meaningful fast enough, which product_log flags correctly.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Tide has a sharp, well-written positioning (mood lens, not fertility) and a clearly defined wedge persona (the introspective journaller). But the spec leans on three load-bearing assumptions that haven't been pressure-tested: (1) that women already journaling will switch from a free-text habit to constrained daily questions, (2) that 1-2 cycles is enough data to produce reads that feel personal rather than generic phase horoscopes, and (3) that Clue/Flo/Stardust users will install a separate app rather than wait for those incumbents to ship the same feature. The product_log itself flags the crowded-category and cold-start risks as still-open. Score: roughly 5/10 answered, 3 partial, 2 unanswered.

Simulated user: Léa, 29, Lyon, designer. Tracks with Clue for 4 years, journals in Notion most evenings, has tried Stardust and uninstalled after a month. Mildly skeptical, intrigued by the "mood lens" framing but expects it to collapse into the same phase-based generic content she has seen elsewhere.

Q1 "Clue already shows me my phase and lets me log symptoms. What does Tide actually do that Clue doesn't?" PARTIAL — spec asserts incumbents only predict periods, doesn't address Clue's existing mood/symptom logging.
Q2 "I already journal every night. Why would I add a second check-in with prefab questions instead of just keeping my journal?" UNANSWERED — no story for the journaller's existing habit displacement.
Q3 "You say it learns my version of each phase. How many cycles before the read is actually about me and not a generic luteal-phase script?" UNANSWERED — flagged in product_log as open.
Q4 "On day 1 with zero history, what does the morning read even say? Because if it's a textbook phase blurb I'm out." PARTIAL — spec implies learning over month 1, doesn't describe the cold-start read.
Q5 "How is this not horoscopes for hormones?" PARTIAL — spec preempts this verbally but offers no mechanism (only intent) for why it won't drift there.
Q6 "I'm going to give an app my mood every day. Where does that data live, who sees it, is it sold?" UNANSWERED — no privacy/data posture in spec.
Q7 "What happens the week I forget to log for 4 days, does the pattern break, do I get nagged?" UNANSWERED — no recovery/streak behavior described.
Q8 "I'm on hormonal birth control. Does this work for me or am I not your user?" PARTIAL — spec excludes contraception optimization but doesn't say whether HBC users are served.
Q9 "You're telling me 'don't make the big call today' based on a pattern. What if you're wrong and I act on it?" ANSWERED — spec frames reads as weather not verdicts, language is careful.
Q10 "Why wouldn't Flo just ship this next quarter and make Tide redundant?" UNANSWERED — defensibility against incumbents not addressed, product_log flags it.

Score: 1/10 answered, 4/10 partial, 5/10 unanswered.

**Dangerous assumptions:**
- The introspective journaller will adopt a structured 30-second check-in instead of (or alongside) their existing free-text journal. Why dangerous: if Tide doesn't replace or clearly complement the journal, the target wedge churns by week 2. Cheap test: 10 journaller interviews, show two example daily-read screens and a mock question set, ask if they would do it for 28 days alongside their journal.
- The personalized read becomes meaningfully better than a generic phase script within 1-2 cycles. Why dangerous: if month 1 reads feel like horoscopes, users uninstall before personalization kicks in, exactly the Stardust failure mode. Cheap test: hand-write reads for 5 women using 1 cycle of retro-logged mood data, blind-compare against generic phase content, measure 'feels about me' rating.
- Defensibility against Clue/Flo shipping the same mood-lens feature. Why dangerous: incumbents have the cycle data and distribution; if mood-by-phase is just a feature inside Clue, Tide has no moat. Cheap test: audit Clue/Flo/Stardust roadmaps and recent releases for mood-pattern features, talk to 5 ex-Clue users about why they would install a second app.
