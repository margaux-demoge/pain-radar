# Crest — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The plateau problem sits squarely inside the largest, best-funded category in consumer health: weight loss apps. Two distinct waves already address it: (1) trend-smoothing apps (Happy Scale, Libra, MacroFactor) which reframe the daily number as a trend line, and (2) AI coaching apps (Simple, Noom, Carbon, Fitia, ate it., Welling) which explicitly market plateau troubleshooting, recalibration, and personalized nudges. Non-scale victories are also already a checkbox feature in WW, Noom, and dozens of trackers. Crest's three pillars (trend over daily number, NSVs, plateau troubleshooter with diet break/refeed/recalibration) each map 1:1 to an existing well-funded incumbent. The wedge has to be sharp. What does the team have that the top 3 competitors do not?

**Top competitors:**
- Happy Scale (iOS): smooths daily fluctuations into a trend line, directly addresses 'don't read the flat line as failure' — active, indie hit. https://happyscale.com/
- MacroFactor: trend-weight algorithm + auto-recalibrating maintenance calories when progress stalls, basically Crest's troubleshooter as math — active, paid. https://macrofactor.com/
- Simple (AI Weight Loss Coach): conversational AI coach with plateau troubleshooting, daily nudges, NSVs — active, very well funded. https://apps.apple.com/us/app/simple-ai-weight-loss-coach/id1467720176
- Noom: psychology-based coaching, group coach that explicitly posts plateau breakthrough tips and reframes scale obsession — active, public-company scale. https://www.noom.com/
- Carbon Diet Coach (Layne Norton): science-based weekly recalibration with diet break / refeed protocols built in — active, paid. https://www.joincarbon.com/

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Help me keep believing I'm still making progress when the scale stops moving, so I don't give up.
Classification: naturally recurring (daily weigh-in ritual is already in the user's life, and the plateau anxiety recurs every morning until it breaks)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong. The whole product is built around making invisible progress visible (trend line, non-scale victories curve, troubleshooter interventions to "try one thing"). Mastery over the plateau itself is the core reward.
- Autonomie (sentiment d'être en contrôle): Strong. The troubleshooter explicitly hands the user one chosen lever to pull rather than prescribing a plan, and reflections are self-logged. The user stays the agent of their own journey.
- Lien social (sentiment d'être connecté à d'autres): Absent. No mention of community, comparison cohorts, sharing, or social features. The coach voice is one-to-one with the app, not relational.

**Boucle d'habitude**
- Déclencheur: morning weigh-in, an existing ritual the target user already performs daily. INTERNAL (the scale itself is the cue, encountered physically, not pushed by the app).
- Routine: weigh in, see the reframed trend line and explanation; weekly, a short non-scale reflection; during real plateaus, pick one intervention.
- Récompense: immediate Y. A calm reframe of the flat line + visible parallel progress curve delivered in seconds at the moment of maximum anxiety. Emotional relief is the payoff and it lands right when the cue fires.
- Push reliance: Low. The loop is anchored on the physical scale, not on notifications. Push could reinforce weekly reflections but isn't load-bearing.

**Verdict line**
Two of three angles pass cleanly and the third passes strongly. The job recurs naturally because plateaued users are already weighing themselves daily, so Crest grafts onto an existing ritual rather than inventing one. Compétence and autonomie are both Strong (reframed progress + user-picked interventions), and the habit loop has a real internal cue (the scale) with an immediate emotional reward (relief from the flat-line spiral). Lien social is absent, which caps ceiling but doesn't block retention.

**What needs to change for STRUCTURAL_RETURN**
N/A, verdict already STRUCTURAL_RETURN. Watch-outs to address in Phase 2 rather than blockers: what happens to the loop once the plateau breaks and the user resumes losing (does Crest still have a job, or does it hand back to the previous tracker)? And is there a lightweight relatedness layer (anonymized "others at week 4 of plateau") that could lift the third need from Absent to Weak without turning Crest into a social app?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Simulated user: Jenna, 34, Columbus OH, 14 months into a cut, down 52 lbs, stalled 4 weeks. Uses MacroFactor for adaptive TDEE, Happy Scale for trend smoothing, Renaissance Periodization for lifting, and lurks r/loseit daily. Mildly skeptical, allergic to "coach voice" wellness apps, already pays for a tracker that does adaptive math. The spec nails the emotional moment and the persona shape (calorie-aware, scale-obsessed, r/loseit literate), and the troubleshooter list (recalibration, diet break, refeed, sleep) maps cleanly onto what this audience already discusses. Where it gets weak: Crest assumes plateaued users will switch FROM the tracker they already trust TO a coach app that doesn't track macros, will tolerate having the daily number hidden, and will trust generic intervention picks over MacroFactor's adaptive algorithm. Interview: 4 ANSWERED, 3 PARTIAL, 3 UNANSWERED out of 10. Q1 (why switch from MacroFactor that already does adaptive TDEE?) UNANSWERED. Q2 (will I tolerate the daily number being hidden, isn't that paternalistic?) PARTIAL, spec acknowledges in product_log but doesn't resolve. Q3 (do I really want coach voice or just better data?) UNANSWERED, this is literally the open question. Q4 (NSV logging weekly, sounds like journaling I'll abandon by week 3) PARTIAL. Q5 (how does Crest know my true maintenance without tracking my intake?) UNANSWERED, critical gap. Q6 (six to eighteen months in, I already know what a diet break is, why pay you to tell me?) PARTIAL. Q7 (plateau biology explainer, I've read every r/loseit FAQ already) ANSWERED weakly via reframing angle. Q8 (do I run Crest alongside MacroFactor or replace it?) UNANSWERED. Q9 (what happens after the plateau breaks, do I churn?) UNANSWERED. Q10 (photo comparison and clothes-fit, I've tried Happy Scale's mood tags and stopped, what makes this stick?) PARTIAL. The positioning is emotionally sharp but operationally hand-wavy on the data layer, which is exactly where this audience is most discerning.

**Dangerous assumptions:**
- Plateaued users will adopt a coach-only app that doesn't track calories/macros, when they already trust a tracker (MacroFactor, Lose It!) that does adaptive TDEE math natively. Cheap test: post a mock in r/loseit asking 'would you use a plateau coach alongside MacroFactor or instead of it?' and count replace-vs-augment responses, plus DM 10 plateau-post authors to ask what they'd actually swap out.
- Hiding the daily weigh-in number is the right move, not a paternalistic move that breaks trust with people whose entire identity is 'I weigh myself every day and look at the number.' Cheap test: A/B two Figma screens (number visible vs number hidden, both with trend line) in a 20-person r/loseit DM survey, ask which they'd open tomorrow.
- Users want a coach voice (reframing, reflection prompts, NSV journaling) more than they want raw interpretable data. The product_log flags this as open and the spec resolves it toward 'coach' without evidence. Cheap test: landing page split test, one variant 'the coach for your plateau', one variant 'the plateau dashboard that explains what your scale won't', measure signup intent.
