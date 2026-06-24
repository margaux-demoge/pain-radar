# Norm — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "AI parenting coach for behavior worries" category exploded in 2024-2025. At least 4 apps (KidSense, Tantrum AI, Tantrum Tamer, Good Inside) explicitly let parents describe a behavior and get age-calibrated guidance, the exact Norm wedge. Adjacent but well-funded players (CDC Milestone Tracker, Bark) cover the "is it a flag" question from screening and monitoring angles. Failure pattern is thin because the wave is recent, but the differentiator Norm claims (calibrated frequency baseline + "phase or flag" threshold) is already partly delivered by KidSense and Good Inside.

**Top competitors:**
- KidSense — AI parenting app where parents log tantrums/meltdowns/defiance and get age-appropriate scripts and analysis. Active, well-marketed. https://www.sheknows.com/parenting/articles/1234950803/kidsense-ai-parenting-app-explained/
- Tantrum AI — On-demand AI tantrum coach, real-time de-escalation strategies tailored to the child. Active on iOS/Android. https://apps.apple.com/mt/app/tantrum-ai-calm-toddler-chaos/id6469646860
- Good Inside (Dr. Becky) — $279/yr membership with AI chatbot for parenting questions, huge brand authority. Active. https://www.goodinside.com/
- CDC Milestone Tracker — Free, age-calibrated checklists with explicit 'when to act early' thresholds, the closest free analog to Norm's phase-or-flag promise. Active. https://www.cdc.gov/act-early/milestones-app/index.html
- Tantrum Tamer — AI-guided in-the-moment prompts for what to say. Active. https://skidamarinkkids.com/tantrumtamerapp/

## retention-validator: `WEAK_RETURN`

The core job ("is this worrying behavior normal?") is occasional, triggered by a fresh worry rather than a daily rhythm. The frequency log offers a real internal cue (after a meltdown, log it) with an immediate reframing reward, which is the strongest retention lever in the spec. SDT is thin: competence is weak (parent observes the kid, not their own progress), autonomy is moderate (calm read, no push), social is absent by design. Only the habit-loop angle clearly passes; need-recurrence and SDT do not.

Full assessment:

**Le job que l'app fait pour l'user**
Get a calm, calibrated second opinion on whether a specific child behavior is in the normal range or worth escalating.
Classification: occasional (recurs unpredictably, per new worry; the logging sub-job can be daily but is secondary)

**Besoins psychologiques nourris**
- Compétence: Weak. The parent gains understanding of their child, but there is no visible progression of the user themselves; no mastery arc designed in.
- Autonomie: Weak-to-Strong. Norm explicitly refuses to push, scroll-bait, or prescribe a philosophy, which respects user control, but there is no active configuration or ownership loop beyond the log.
- Lien social: Absent. By design, no forums, no community, no shared logs. This is a deliberate trade-off, not an oversight.

**Boucle d'habitude**
- Déclencheur: "Something my kid just did is bothering me" or "another meltdown happened, log it." INTERNAL (anxiety spike / post-incident moment in real life).
- Routine: Describe the behavior in plain words via structured intake, or one-tap log a recurring behavior.
- Récompense: A calibrated sentence placing the behavior on a spectrum, plus over time a frequency picture that often reduces the worry. Immediate: Y for intake, Y for log (the tap confirms, the chart accrues).
- Push reliance: None mentioned. Retention rests on internal cues (parental worry, post-incident logging), which is healthier than push but also means no safety net if the worry fades.

**Verdict line**
WEAK_RETURN. The habit loop is the one angle that clearly passes: internal cues are strong (parental anxiety, post-incident moments) and rewards are immediate. But the underlying job is occasional rather than naturally recurring, and psychological needs are at best weakly nourished (no competence arc, no social, autonomy mostly expressed as restraint). Once a worry is resolved or a parent concludes "it's a phase," the structural pull to return weakens sharply.

**What needs to change for STRUCTURAL_RETURN**
- Is there a way to make the logging routine the primary job rather than a secondary feature, so that a daily or per-incident rhythm anchors retention even after the initial worry is answered?
- Can Norm surface a sense of parent-side progression (e.g., "you have observed X transitions, here is what the pattern shows") that turns the parent into a competent observer over time, without tipping into gamification?
- Does the product accept being a worry-cycle tool that users return to only when a new worry surfaces, and if so, how is that re-acquisition cost handled (memory of prior worries, easy re-entry, multi-child support)?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Norm has a sharply defined pain ("phase or flag?") and a clear target (parents 2-10 worried about a recurring behavior), and the calibration framing differentiates it cleanly from Google and parenting-philosophy apps. But the spec leans heavily on three unvalidated trust claims: that an app (not a clinician) can credibly say "this is normal", that parents will trust a non-diagnostic verdict enough to stop googling, and that the calibration data behind those verdicts actually exists at age-by-behavior granularity. Persona scrutiny finds the "calm second opinion" promise compelling in concept but thin on proof. Simulated user, Claire, 34, Lyon, mother of a 5-year-old who melts down at every transition, currently uses Google, a Facebook moms group, and occasionally Maman Blues podcast, mildly skeptical of "AI tells me my kid is fine." Interview: Q1 "Why would I trust an app over my pediatrician's 11 minutes?" PARTIAL — spec positions Norm as a second opinion but doesn't say who built the calibration. Q2 "What's the source of your 'typical for this age' data?" UNANSWERED — no mention of clinical basis, dataset, or expert review. Q3 "I already googled and got 40 answers, why is your answer the right one?" PARTIAL — calibration framing helps but credibility source missing. Q4 "If you tell me it's normal and it turns out to be autism, who's liable?" UNANSWERED — flagged in product_log but not addressed in spec. Q5 "I'm not going to log meltdowns in the moment, my hands are full, when exactly do I open this?" PARTIAL — "tap to log" is mentioned but no friction model. Q6 "How is this different from the BabyCenter app or Wonder Weeks I already have?" UNANSWERED — no competitive positioning. Q7 "What does the 'small picture of where you sit on the spectrum' actually look like, a number, a graph, a sentence?" PARTIAL — described abstractly, not concretely. Q8 "If I describe a meltdown in my words, how do you know you understood what I meant?" UNANSWERED — the translation step from plain words to developmental categories is asserted, not shown. Q9 "Three weeks of logging to find out it's every 5 days, not every day, why would I stick around that long when I'm anxious now?" UNANSWERED — retention through the anxiety-to-relief arc is not addressed. Q10 "If Norm is 'incentivized only to be right', how do you make money without keeping me scrolling?" UNANSWERED — business model absent and undermines the trust promise. Score: 0 ANSWERED, 4 PARTIAL, 6 UNANSWERED. Verdict: WEAK_ON_ASSUMPTIONS leaning toward BUILT_ON_SAND — the positioning is clear but the credibility scaffolding required to deliver it is entirely unbuilt.

**Dangerous assumptions:**
- Parents will trust an app's 'calm calibration' instead of (or before) a clinician, without a visible credibility source. Why dangerous: the entire value prop is 'honest second opinion', if parents don't believe the source, they go back to Google. Cheap test: show 20 target parents two versions of the same Norm output, one with 'reviewed by pediatric psychologists' and one without, measure willingness to act on the verdict.
- Reliable age-by-behavior calibration data exists and can be turned into 'here's where yours falls' verdicts. Why dangerous: without a real dataset, Norm's core sentence is a hallucinated guess and H3 (70% pediatrician-confirmed flags) is unachievable. Cheap test: pick 5 common behaviors (meltdowns, eye contact avoidance, hitting sibling), try to source published norms by age, see if the granularity is real or marketing.
- Anxious parents will log behaviors over three weeks to reach the 'it's actually every 5 days' insight. Why dangerous: H2 depends on this, but acute worry collapses to zero engagement once the first verdict lands as 'normal'. Cheap test: run a 3-week diary study with 10 worried parents using a paper or Notion log, measure day-7 and day-21 drop-off without any product magic.
