# Mirror — judges verdicts

## benchmark-scanner: `EMERGING`

The appearance-anxiety / BDD app space has serious clinical entrants (Perspectives, Worth Warrior, Intellect) and a broader pool of generic in-the-moment anxiety chatbots (Wysa, Rootd, Noah AI, Anima Felix), but none own Mirror's specific wedge: a private, non-clinical, in-spiral interrupter for sub-clinical appearance loops happening late at night. Recent shutdowns (Woebot, Yara) flag a real failure pattern: AI chatbots collapse when they overreach into clinical territory without safety scaffolding, which is directly relevant given the BDD/self-harm adjacency of this problem. Window is open but narrow, and the safety design will decide whether Mirror lives in the EMERGING bucket or joins the graveyard.

**Top competitors:**
- Perspectives (Koa Health + MGH) — coach-supported CBT app for BDD, NHS-recommended, clinical not in-spiral, https://perspectives.health/
- Worth Warrior — free CBT-E app for young people with negative body image and low self-worth, structured program not moment-of-spiral, https://apps.apple.com/us/app/worth-warrior-help-body-image/id1641866414
- Rootd — acute panic intervention with prominent panic button and guided grounding, closest in interaction shape but generic anxiety, https://animafelix.com/blog/best-anxiety-apps-2026/
- Noah AI — conversational AI coach with 3-minute grounding calls explicitly pitched for late-night spirals, generic emotional regulation, https://heynoah.ai/
- Wysa — clinical-grade AI CBT chatbot for anxiety/depression, broad scope, not appearance-specific, https://blog.mylifenote.ai/best-apps-for-anxiety/

## retention-validator: `WEAK_RETURN`

The job (escape an appearance-anxiety spiral) recurs occasionally and unpredictably, not on a daily schedule. SDT is mixed: compétence is weak (the spec deliberately refuses streaks/progress as content), autonomie is strong (private, closed, user-driven), lien social is absent by design. The habit loop has a strong internal cue (the spiral itself) and immediate emotional reward (relief), which is the main retention engine, but recurrence is event-driven and the product explicitly rejects mechanics that would deepen habit. Verdict: WEAK_RETURN, carried by the habit-loop angle alone.

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Get me out of an appearance-anxiety spiral when I am already inside it, so I can put the phone down and reclaim the rest of my evening.
Classification: occasional (recurs but unpredictably, triggered by life events: a photo, a mirror, a comment)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. Mirror surfaces patterns gently over time and recognition shortens the loop, but the spec explicitly refuses streaks, timelines, and any visible progression mechanic.
- Autonomie (sentiment d'être en contrôle): Strong. Private, closed, no feed, no audience, the user types or talks freely, the interaction is short and on their terms.
- Lien social (sentiment d'être connecté à d'autres): Absent. Designed out on purpose, no community feed, no shared content, the bet is that the spiral does not need an audience.

**Boucle d'habitude**
- Déclencheur: the spiral itself (caught reflection, photo, late-night rumination, comment), INTERNAL. Strong internal cue tied to a real-life felt state.
- Routine: open Mirror, describe what just happened, receive a named diagnosis of the loop plus a fitted exit (grounding, reframe, fact, or sitting with it).
- Récompense: relief, exit from the loop, ability to put the phone down. Immediate Y.
- Push reliance: none, retention does not depend on push, the cue lives entirely inside the user.

**Verdict line**
Only the habit-loop angle passes cleanly: the internal cue is strong and the reward is immediate. The job is occasional rather than naturally recurring (spirals do not happen on a schedule, and on calm days the app has no reason to be opened), and only one of three psychological needs is Strong. The product can survive launch on the strength of in-the-moment relief, but week 4+ retention is fragile because the team has deliberately removed the mechanics (progress, streaks, social) that usually deepen return visits.

**What needs to change for STRUCTURAL_RETURN**
- Is there a calm-day job Mirror can do, between spirals, that does not turn appearance anxiety into content (e.g. a private pattern review, a "what shortened the loop last time" reflection) and that would lift compétence from Weak to Strong?
- Can the pattern surfacing become a felt sense of progress without becoming a tracker the user fears breaking?
- Is the team comfortable accepting an event-driven retention curve (users return only when spirals hit) as the success shape, and does H3's 35% / 3+ sessions in 14 days target match that reality?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Mirror has a vivid problem statement and a sharp target wedge (late-night spirallers, 16-35, sub-clinical appearance anxiety), and the product experience is concrete enough to simulate. But the spec rests on three unvalidated behavioral bets: that people in a spiral will reach for an app instead of Instagram/TikTok/the mirror, that an LLM can "name the loop" accurately enough to feel like a friend rather than a chatbot, and that opening up about appearance shame to a phone is something this user will actually do. The "in short" promise (you open Mirror, Mirror gets you out) is asserted, not evidenced. Persona pushes back hard on trust, on the moment-of-spiral capture, and on what makes this different from texting a friend or just scrolling. Interview: 3 ANSWERED, 4 PARTIAL, 3 UNANSWERED out of 10.

Simulated user: Léa, 24, Lyon. Works in marketing, lives alone. Uses Instagram and TikTok daily, follows skincare and "that girl" creators she knows are bad for her. Has tried Stoic and Finch journaling apps, abandoned both after two weeks. Saw a therapist twice last year, stopped because of cost. Mildly skeptical, tired of wellness apps that promise to fix her and then ask for 70 euros a year.

Interview:

Q1, "It's 11pm, I'm in bed, I just spent 40 minutes zooming into my jawline in selfies. Why would I open YOUR app instead of just keep scrolling like I always do?"
> PARTIAL. Spec asserts Mirror is "the friend who picks up the phone" but does not address the competing pull of the doom-scroll, which is what the user is already doing in the spiral.

Q2, "How does Mirror even know I'm spiralling? I'm not going to open an app called Mirror at the worst moment of my night. That requires me to admit it first."
> UNANSWERED. No trigger mechanism, no notification logic, no entry point hypothesis. The spec assumes the user opens it; that is the entire premise of H1 and it has zero acquisition mechanism described.

Q3, "I type 'I hate my nose'. What does the app actually say back? Give me the first three sentences."
> PARTIAL. Spec describes naming the loop ("this is a comparison loop") but does not show example output. The quality of the LLM response is the entire product and is undefined.

Q4, "I've used Finch and Stoic. They both promised me they were different. Why isn't this just another journaling app I'll quit in two weeks?"
> PARTIAL. Spec explicitly differentiates from journaling ("not after, in the moment") and from streak-based apps, but does not address the deeper retention question once the novelty wears off.

Q5, "Why would I trust an AI with the most shameful thing about me, that I haven't even told my best friend?"
> UNANSWERED. No trust-building mechanism, no privacy story beyond "closed, private, small", no explanation of why an AI feels safer than a human here.

Q6, "What stops me from using Mirror as the new thing I do compulsively? Another loop, another tab in my brain?"
> ANSWERED. Spec explicitly addresses this: no streaks, refuses to be a place where appearance anxiety is content, "small on purpose".

Q7, "If Mirror 'learns my loops', am I going to get a weekly summary telling me I spiralled about my face 14 times? That sounds like hell."
> PARTIAL. Spec says patterns are surfaced "gently, without making the patterns themselves into another thing to spiral about" but no mechanism for how that is calibrated.

Q8, "I tell it I want to lose 5 kilos. Does it agree with me, or does it tell me I'm fine? Either answer is wrong."
> UNANSWERED. The hardest product question. Spec mentions "a hard fact about the math of how often other people are actually noticing" but does not define the stance on user-stated appearance goals vs the spiral. This is the BDD-adjacent edge case the spec gestures at without resolving.

Q9, "Five minutes from now, I close Mirror. What happens tomorrow at 11pm? Same conversation again?"
> ANSWERED. Spec addresses recurrence via H3 (return on next spiral) and pattern learning over time.

Q10, "Honestly, why isn't this just a really good system prompt I could paste into ChatGPT for free?"
> ANSWERED. The wedge is moment-of-spiral capture, pattern memory, and refusal-to-be-content, none of which a raw ChatGPT prompt provides. But the spec should make this explicit, because the user will ask.

Score: 3 ANSWERED, 4 PARTIAL, 3 UNANSWERED.

Verdict: WEAK_ON_ASSUMPTIONS. The positioning is sharp but three core mechanisms (in-spiral entry trigger, LLM response quality, stance on appearance goals) are undefined and any one being wrong kills the product.

**Dangerous assumptions:**
- The user will open Mirror DURING the spiral, not after. There is no entry-point mechanism described — no notification, no widget, no trigger detection. If users only open it the next morning, Mirror is a journaling app, which the spec explicitly says it is not. Cheap test: 5 paid diary-study participants log every appearance-anxiety spiral for 14 days and record whether they reached for any app, which one, and when relative to the spiral peak.
- The LLM can 'name the loop' accurately and helpfully on the first try, in the user's worst moment, without sounding like a chatbot or making it worse. The entire product is the quality of this response, and the spec does not show a single example. Cheap test: Wizard-of-Oz with a clinical psychologist responding via SMS to 10 recruited spirallers for 2 weeks, measure 'did this help you put the phone down' self-report.
- Mirror can hold a coherent stance when the user states an appearance goal that is itself the spiral (e.g. 'I need to lose 5kg', 'my nose is wrong'). Validating reinforces BDD-adjacent behavior; dismissing breaks trust. The spec does not pick a side. Cheap test: write the 20 hardest user inputs and red-team the desired response with a clinical advisor before any build.
