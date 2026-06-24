# Cast — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "self-discovery via traits/archetypes" space is crowded with AI journaling apps (Mindsera, Reflection, Life Note, Know Your Ethos) that already build identity portraits over time, and a thick layer of gender-role tests (IDRlabs, Psych Central, TherapyDen, Shapes AI) that occupy the masculinity/femininity framing. The masculinity-coaching niche has fresh entrants (Good Men Helping Good Men, Mastered Man, Mindful Masculine) while archetype-based portrait apps (TerraYou, Soultrace, Individualogist) cover the "build your own portrait" promise. No clearly failed shutdowns surfaced for this exact angle, the failures are likely buried in tests and indie launches that never made noise, so the risk is differentiation, not viability. Cast's wedge (private, non-prescriptive, gender-role specific, with a "try on a trait for a week" loop) is real but sits between two crowded categories that both already claim "judgment-free reflection".

**Top competitors:**
- Mindsera — AI journal that analyzes entries, surfaces patterns, and generates a visual self-portrait, active, https://mindsera.com/
- Life Note — AI journaling that produces a weekly 'Inner Portrait' from entries, matches users to mentors by values, active, https://www.mylifenote.ai/
- Shapes AI Gender Role Test — chat-based open-ended gender role exploration positioned as private introspection, active, https://shapes.inc/genderroletest
- TerraYou Archetype Test — builds an archetype-based identity profile keyed to values and traits, active, https://terrayou.com/archetype-test
- Good Men Helping Good Men (GMHGM) — newly launched 2025 app redefining modern masculinity through tracked traits and brotherhood check-ins, active, https://techadvice.life/2025/10/17/good-men-helping-good-men-the-movement-redefining-masculinity-launches-a-new-app/

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Help me figure out which traits of masculinity/femininity/identity are actually mine versus inherited or performed, in private.
Classification: occasional (the identity question recurs in waves, triggered by life events or social friction, not on a daily/weekly clock; for many users it trends toward near one-shot once a portrait "feels right", a risk the product log itself flags).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. The "try on a trait for a week" loop offers a small sense of progress, but there is no skill tree, no measurable mastery, the portrait is descriptive not progressive.
- Autonomie (sentiment d'être en contrôle): Strong. The entire product is built around the user choosing traits rather than being told who to be, no prescription, no labels, explicit "mirror with a notepad, not a coach with an opinion".
- Lien social (sentiment d'être connecté à d'autres): Absent. Explicitly designed out, nothing is shared, no community, positioned as anti-forum.

**Boucle d'habitude**
- Déclencheur: a moment of identity friction, catching yourself performing a trait, or the end-of-week check-in on a trait being tried on. EXTERNAL for the check-in (Cast prompts), INTERNAL for the friction moment but that internal cue is rare and unpredictable.
- Routine: open Cast, reflect, examine a trait, log what stuck, optionally revise the portrait.
- Récompense: clarity, a refined self-portrait, the feeling of having named something. Immediate: partially Y, the reflection feels good in-session, but the deeper reward (portrait that fits) is delayed over weeks.
- Push reliance: yes, the weekly trait check-in seems to be the main recurring cue, which means retention likely depends heavily on push to survive past the initial portrait build.

**Verdict line**
Only one angle clearly passes: autonomy is strong and well-designed. The job does not recur naturally on a predictable cadence (the product log itself names the one-and-done risk), competence and relatedness are weak/absent, and the habit loop leans on external weekly prompts with a delayed reward. Cast can hold a user through the initial portrait build but has no structural pull once that portrait "feels right".

**What needs to change for STRUCTURAL_RETURN**
- What internal cue in the user's daily life (not a Cast push) would make them want to open the app on a Tuesday evening when nothing dramatic happened?
- Is there a way for the portrait to stay alive (evolving prompts, situational replays, identity stress-tests tied to real events) so that competence, the sense of getting clearer over time, becomes visible and rewarding session to session?
- Once a user has a portrait that feels right, what is the second job Cast does for them, or does the team accept Cast as a multi-month churn product rather than a long-retention one?

## user-interview-simulator: `BUILT_ON_SAND`

Simulated user: Jordan, 26, Portland. Currently lurks on r/AskMen, saves TikToks from masculinity/femininity creators, occasionally journals in Notes app, has tried Stoic and Finch. Mildly skeptical, allergic to anything that feels like a personality quiz or a self-help grift. The spec defines a beautiful problem and a poetic experience but barely survives basic user scrutiny. Q1 "is this actually my pain or a pain you wrote elegantly", ANSWERED via Reddit evidence. Q2 "how is this different from journaling in Notes", PARTIAL (the trait workshop and try-on weeks are differentiated, but the daily prompt feels journal-adjacent). Q3 "why would I trust an LLM to mirror back something this intimate without skewing me", UNANSWERED (the spec claims neutrality but gives no mechanism). Q4 "what does a 'try on a trait for a week' actually look like Tuesday at 3pm", UNANSWERED (no concrete prompt example, no nudge format, no check-in mechanic). Q5 "I already have a sense of who I am, why would I open this twice", PARTIAL (revisit-the-portrait is asserted but no recurring trigger). Q6 "if you don't push me toward any tradition, how do you avoid being mush", UNANSWERED (neutrality-as-positioning risks blandness, no mechanism described). Q7 "what stops this from getting weaponized into trad/anti-trad screenshots", UNANSWERED, also flagged in product_log. Q8 "I'm a woman renegotiating femininity, the Reddit evidence is 3/4 male, is this really for me", UNANSWERED, product_log itself raises men-vs-women audience split. Q9 "after I build my portrait, what brings me back in week 6", UNANSWERED, product_log explicitly flags one-and-done risk. Q10 "how is this not horoscope-for-gender, traits dressed up as insight", PARTIAL. Score: 2 ANSWERED, 3 PARTIAL, 5 UNANSWERED. Three of the top dangerous assumptions are unvalidated and two are already self-flagged in product_log. Verdict: BUILT_ON_SAND. The core value proposition has not survived basic user scrutiny. Do not build before validating assumption #1 (that the "try on a trait for a week" mechanic is concrete, doable, and produces a felt insight, not a journal entry in a fancy wrapper).

**Dangerous assumptions:**
- The 'try on a trait for a week' mechanic is the load-bearing differentiator vs journaling/Stoic/Finch, but the spec describes it only abstractly. If the daily prompt feels like a horoscope or a generic CBT nudge, H1's 40% completion target collapses. Cheap test: write 5 real trait-week scripts (Monday-Sunday prompts + end-of-week reflection) for 'stoic restraint', 'hyper-feminine softness', 'androgynous independence', show them to 8 target users and ask 'would you do this for 7 days, and what would change in you'.
- Genuine neutrality on a politically charged topic is technically achievable by an LLM-driven mirror. The spec asserts neutrality as a promise but gives no mechanism (prompt guardrails, refusal patterns, framing audits). If users perceive any skew, the wedge audience (curious self-examiners avoiding tribes) bounces immediately. Cheap test: red-team a prompt prototype with 6 users, 3 trad-leaning, 3 progressive-leaning, ask each whether Cast 'has an opinion'.
- Retention past the initial portrait build. Product_log already flags this. H2 (50% revise) and H3 (6+ sessions/month) both depend on a recurring reason to return that the spec does not name. If the portrait is one-and-done, Cast is a 2-week app. Cheap test: interview 5 users who have done identity work (therapy, journaling, coaching), ask what made them return week 6 vs drop off, map those triggers against Cast's current loop.
