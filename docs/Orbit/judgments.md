# Orbit — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "remind me to stay in touch with my people" space is dense and active in 2026: Dex, Clay/Mesh, Garden, Fabriq, Social Compass, Soonly, Foster, Friendzone, Friendward, Monica, Amicu, Nudgy and others all ship the same core mechanic Orbit proposes (named constellation + cadence + nudge + one-tap action). Several past attempts (Keep My Friends closed signups in 2023, Etacts and ConnectedHQ acquired and shut, UpHabit pivoted to sales) confirm the problem is real but retention/monetization is the recurring killer. The relationship-driven wedge ("falling deep into one person") is positioning, not product, and is not reflected in any defensible feature gap versus Fabriq or Social Compass.

**Top competitors:**
- Fabriq (ourfabriq.com), relationship tracker with reminders, cadence per contact, up to 150 people, active and updated through 2026
- Social Compass (socialcompass.social), personal-friendship-first tracker with per-person reminder cadence, positions explicitly against business CRMs
- Garden: Stay in Touch (Apple App Store), set reminder frequency per contact and get nudged, on the store since 2018, still active
- Dex (getdex.com), the dominant personal CRM, reminders + follow-ups + LinkedIn sync, ~$12/mo, networking-leaning but heavily used for friends too
- Soonly, reminders plus 'Sparks' conversation drivers to lower the friction of the actual outreach, very close to Orbit's 'voice note in 90s' wedge

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Keep peripheral friendships from dying while the user is deep in a romantic relationship, by lowering the activation cost of reaching out.
Classification: naturally recurring (friendship maintenance is an ongoing, lifelong need, with weekly/monthly cadence built into the product itself)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. Gap-time shrinking exists as a back-end metric (H2) but the spec doesn't surface a visible progression artifact to the user (no streak, no "constellation health" view described). Sense of mastery is implicit, not designed-in.
- Autonomie (sentiment d'être en contrôle): Strong. User defines who's in the constellation, the cadence per person, can let people drift off with confirmation. The tone explicitly refuses to rank or shame. Control is central.
- Lien social (sentiment d'être connecté à d'autres): Weak. The app facilitates connection with people outside the app, but there's no in-app social layer, no mutual presence, no shared experience. Relatedness is downstream of using the app, not produced by it.

**Boucle d'habitude**
- Déclencheur: Weekly nudge ("Anna's gone three weeks, want to send her a voice note now?"), EXTERNAL. Monthly planning prompt also external. No internal cue surfaced in the spec, the user has no in-life moment that pulls them to open Orbit unprompted.
- Routine: Tap the nudge, record a voice note or accept a calendar window, ~90 seconds. Friction is well engineered.
- Récompense: The message is sent, the date is on the calendar, a small relief of guilt. Immediate Y, though the deeper reward (the friend responding, the dinner happening) is delayed and outside the app.
- Push reliance: High. The entire loop is anchored on the weekly nudge and the monthly prompt. If the user mutes notifications, the loop collapses, there is no internal cue described that would bring them back on their own.

**Verdict line**
One angle clearly passes: the underlying need recurs naturally and is in fact built into the product cadence. Autonomy is also strong, which is rare and worth noting, but competence and relatedness are weak, and the habit loop depends entirely on external push with no internal cue. Net: WEAK_RETURN, the product can hold users who keep notifications on, but has no structural pull once push is muted or the novelty of the first few nudges fades.

**What needs to change for STRUCTURAL_RETURN**
- What does the user see when they open the app on their own, that gives them a reason to return between nudges? Is there a constellation view, a sense of "my world is alive", that rewards a check-in?
- What internal cue, a feeling or a moment in the user's day, could trigger an unprompted open? (e.g. a quiet evening, a moment of guilt after declining a plan, finishing dinner with the partner.)
- Is there a visible progression artifact, something that makes the user feel they are getting better at this over weeks, not just performing isolated micro-actions?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Orbit has a sharp emotional hook (drift inside a relationship, not personal-CRM) and a defined persona, which gives it more positioning strength than most personal-CRM clones. But the spec doesn't survive basic user scrutiny on three load-bearing assumptions: that a weekly nudge with the "most overdue" friend won't feel exactly like the nagging it claims to avoid, that users will trust the app with enough context (calendar, contacts, conversation history) to actually compute "gap-time," and that the framing as a relationship-era product won't simply repel the very users who'd quietly resent being told their world is shrinking. Persona: Camille, 29, Lyon, in a 3-year relationship, uses WhatsApp + iOS Calendar + occasional BeReal, tried Monaru for a week and deleted it, mildly skeptical, doesn't want to be lectured.

Interview:
Q1 "Camille, 29: why do I need an app for this when I literally have WhatsApp open all day?" PARTIAL — spec says friction is the issue but doesn't explain why WhatsApp's existing UI isn't already friction-zero.
Q2 "Once a week you'll tell me which friend I'm failing the most. How is that not exactly the guilt-trip you say you're avoiding?" UNANSWERED — "tone is gentle" is asserted, not designed. The mechanic IS a ranking by neglect.
Q3 "How does Orbit actually know I haven't seen Anna in three weeks? Are you reading my messages and my calendar?" UNANSWERED — gap-time detection is central and the spec is silent on data sources.
Q4 "I tried Monaru and quit in a week. What stops Orbit from becoming another to-do list I dread opening?" PARTIAL — "one nudge a week, 90 seconds" is the answer but it's the same promise every personal CRM makes.
Q5 "Why is this framed around my relationship? I don't want to open an app that reminds me my partner is eating my life." UNANSWERED — the positioning is the wedge but may actively repel the target.
Q6 "What happens the week I'm sick, traveling, or just busy and ignore the nudge? Does it pile up?" UNANSWERED — no mention of recovery, snoozing, or graceful degradation.
Q7 "You say I list 6-10 people. That setup feels like homework. Why would I do it on day one?" UNANSWERED — onboarding cost vs. payoff is not addressed.
Q8 "How do you measure 'I saw Anna' — do I have to log it, or do you detect it? If I have to log it, that's the work you said you'd remove." UNANSWERED — the logging loop is the hidden tax in every personal CRM and the spec doesn't resolve it.
Q9 "My partner sees me using this. How do I explain it without it becoming a fight about whether I'm unhappy with us?" UNANSWERED — relationship-framed product introduces a social cost the spec ignores.
Q10 "In six months, am I supposed to still be using this? Or is the win that I don't need it anymore?" UNANSWERED — H2 implies habit shift, H3 implies retention; the product's own theory of success is contradictory.

Score: 0/10 answered, 2/10 partial, 8/10 unanswered.

Verdict: WEAK_ON_ASSUMPTIONS leaning toward BUILT_ON_SAND. The hypotheses are crisp but the product mechanic relies on three unvalidated bets (passive gap detection, non-nagging weekly call-out, relationship-era framing being a wedge not a repellent). One of these likely breaks in the first 10 user interviews.

**Dangerous assumptions:**
- Passive gap-time detection works without invasive permissions. The entire mechanic depends on Orbit knowing when you last contacted someone, but the spec is silent on whether this comes from contacts, messages, calendar, or manual logging. If users have to log every interaction, Orbit becomes the chore it claims to eliminate. Cheap test: 5-user prompted interview asking 'how would you want the app to know you saw Anna?' — see if anyone willingly grants message access.
- The weekly 'most overdue friend' nudge feels gentle, not accusatory. The mechanic IS a ranked-by-neglect call-out, and tone alone may not save it. If it lands as guilt, the target user (who explicitly doesn't want to be lectured) churns in week 2. Cheap test: paper-prototype the nudge copy with 5 target users and measure flinch vs. tap intent.
- Framing Orbit as a relationship-era product is a wedge, not a repellent. The target user feels quiet guilt about their shrinking world; an app that names that out loud may be intolerable to open. Cheap test: A/B two landing pages (relationship-framed vs. friendship-maintenance-framed) to the same audience and compare signup intent.
