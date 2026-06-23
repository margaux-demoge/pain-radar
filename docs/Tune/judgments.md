# Tune — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "name your feelings precisely, build the vocabulary, check in twice a day" space is densely populated. How We Feel (Yale-backed, 144 emotion words, free, nonprofit) sits exactly on Tune's wedge. Stoic, Rosebud, Nuju and Animi all run guided therapist-style prompts with morning/evening cadence and AI pattern reads. Reflectly is the cautionary tale: paywalled itself into review backlash but did not shut down, suggesting the journalling-app graveyard is mostly slow decay, not clean death.

**Top competitors:**
- How We Feel (Yale Center for Emotional Intelligence) — 144-word Mood Meter, multi-daily check-ins, free forever, the closest direct hit on Tune's vocabulary thesis
- Stoic — morning/evening reflection cadence, mood + journal, broad mental wellness toolkit, owns the twice-a-day ritual slot
- Rosebud — AI-guided structured reflection with weekly summaries, leads in 'therapy adjunct' positioning
- Nuju — fast daily capture + AI pattern recognition + weekly summaries + coach personas, closest to Tune's 'felt map' idea
- Animi — body-first emotional granularity flow, walks users from sensation to precise feeling name

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Help me notice and name what I'm actually feeling, so it doesn't leak out sideways into my relationships and behaviour.
Classification: naturally recurring (feelings happen every day, the need to read oneself recurs continuously, and the product anchors itself to morning/evening which are universal daily moments).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong. The entire pitch is muscle-building: vocabulary acquisition, precision over time, "the muscle was never built". Progress is the felt map and the upgrade from "irritated" to "disrespected".
- Autonomie (sentiment d'être en contrôle): Strong. Explicit anti-coercion stance: no streak punishment, no badges, no community pressure, voice or text, two minutes on your own schedule. The user is in charge of the pace and the framing.
- Lien social (sentiment d'être connecté à d'autres): Absent. Spec explicitly says no community. Pure solo practice.

**Boucle d'habitude**
- Déclencheur: morning and evening moments anchored to existing daily routine, INTERNAL (tied to waking/winding down, which the user already encounters), though likely reinforced by an EXTERNAL push at first.
- Routine: answer one short, specific question in text or voice, two minutes.
- Récompense: immediate Y. The user gets a more precise word for what they're feeling right now, the small "that's it" recognition. The Sunday read is the deferred reward, but the per-check-in payoff is in-session.
- Push reliance: not pure push reliance, the morning/evening cadence maps to natural life cues, but the product almost certainly needs push to bootstrap the cue until it becomes internal. Worth watching, not a disqualifier.

**Verdict line**
Three angles pass cleanly: the underlying need recurs daily, two of three psychological needs (compétence and autonomie) are strongly designed in, and the loop has plausibly internal cues (morning/evening) plus an immediate in-session reward (a more precise word). The deliberate absence of social is a real cost on the lien social axis and removes one of the strongest retention forces journalling apps usually lean on, but the other two pillars carry it. The main risk is not retention structure, it is whether the precision-of-vocabulary reward is felt sharply enough in the first week to bridge to habit, before the novelty of the morning cue fades.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Tune has a sharp, well-articulated problem and an unusually specific target (intellectually self-aware, emotionally underdeveloped 22-40s). The wedge is real and the prose is convincing. But the product makes three big promises (vocabulary actually transfers, twice-daily fits a busy life, "felt map" feels different from a mood graph) that the spec asserts without showing how. A skeptical user who has already abandoned Daylio and a journalling app would not be convinced by the current §2 alone. Simulated interview below.

**Simulated user**
Léa, 31, Lyon. Product manager, reads Brené Brown, did 3 weeks of Stoic, 2 weeks of Daylio, deleted both. Currently sees a therapist every 3 weeks. Calm in meetings, snaps at her boyfriend on Sunday evenings. Mildly skeptical, time-poor, has heard the "tiny habit" pitch before.

**Interview**

Q1, "I already tried Daylio and a journalling app and dropped them in a week. What makes Tune different at the App Store level, before I download it?"
> PARTIAL. Spec acknowledges in product_log that positioning is make-or-break but §2 does not give a one-liner that would survive a store listing.

Q2, "You say it teaches vocabulary. How exactly, in a 2-minute check-in? Do you show me a word list? Quiz me?"
> UNANSWERED. Spec says it "catches you when you reach for a generic word" but the mechanism (lexicon source, who decides "more precise", UX of the catch) is not described.

Q3, "Morning AND evening. I will forget the evening one by day 3. What happens then, do you nag me?"
> UNANSWERED. Spec says "no streak punishment" but says nothing about what reminder/recovery looks like, which is the actual retention mechanic.

Q4, "I journal in French and my feelings are in French. Does this work in my language or only English?"
> UNANSWERED. Vocabulary-teaching products are deeply language-bound, spec is silent.

Q5, "How is your 'felt map' not just a mood graph with a prettier name? Give me one thing it shows that Daylio cannot."
> PARTIAL. Spec gestures at "themes, people, gap between said and behaved" but product_log itself flags this as needing design exploration.

Q6, "I am praised for being calm. Why would I voluntarily poke at the thing that lets me function?"
> UNANSWERED. The motivation-to-start question is not addressed. The spec assumes the wedge user is "privately tired" but does not show what triggers them to install.

Q7, "Voice or text. If I am at my desk at 9am I am not going to talk to my phone. If I have 20 seconds I am not going to type. Which is it?"
> PARTIAL. Both are offered but the friction model for each context is not thought through.

Q8, "You said 'helps you name the feeling under the story.' That sounds like AI interpreting me. What if it is wrong, or worse, condescending?"
> UNANSWERED. The interpretive layer is the riskiest UX surface and the spec does not address tone, failure modes, or correction loops.

Q9, "I am intellectually self-aware. I will see through a prompt that is just 'how are you' rephrased. How do you keep the questions fresh for 60 days without becoming therapy-app cliché?"
> UNANSWERED. Prompt library depth, variation strategy, and the "good therapist" claim are unbacked.

Q10, "If after two months I have a precise vocabulary but my Sunday outbursts still happen, did Tune fail? What is the actual outcome I should expect?"
> UNANSWERED. The behavior-change claim (vocabulary -> in-the-moment use -> fewer leaks) is the whole bet, and there is no articulated outcome the user can hold the product to. H2 measures self-report of vocabulary use, not the downstream behavior the §1 problem promises to solve.

**Score:** 0/10 answered, 3/10 partial, 7/10 unanswered

**Top 3 dangerous assumptions**

1. Vocabulary actually transfers from in-app prompt to real-life moments. The entire value prop rests on this. Cheap test: 20-person 2-week diary study, prompt them daily, ask each Friday whether they used a new word unprompted with a real human that week.
2. Twice-daily is the sticky cadence, not the breaking one. Product_log already flags this. Cheap test: A/B a landing page with "once a day" vs "twice a day, 2 min each" and measure email signup conversion before building.
3. The interpretive "name the feeling under the story" layer reads as insightful, not as a wrong/condescending AI. Cheap test: Wizard-of-Oz 30 evening check-ins with a human therapist behind the curtain, measure "did this land" on a 1-5 after each.

**Verdict line**
WEAK_ON_ASSUMPTIONS. The positioning prose is strong and the target is specific enough to interview, but seven of ten questions a skeptical lapsed-journalling user would ask have no answer in the current spec, and all three of the make-or-break assumptions are unvalidated. Do not build §2 mechanics until at least assumption #1 has a cheap signal.

**Dangerous assumptions:**
- Vocabulary learned in-app transfers to real-life moments (the entire value bet, untested)
- Twice-daily cadence is sticky rather than the friction point that kills retention
- The interpretive 'feeling under the story' layer reads as insightful rather than as a wrong or condescending AI
