# Cradle — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The postpartum app category is well populated with active, funded players across three flavors: fitness (Sweat, WeGLOW, MomsLab, SLAM/Get Mom Strong, Natal), holistic recovery tracking (Postpartum Journey, Motherocity, Femia, Mahmee), and maternal mental health (Expectful, Canopie). Most already market "gentle", "no-guilt", "10-minute" framing, so Cradle's "lower the bar" copy alone won't differentiate. No notable failed attempts surfaced, the category is growing, not dying. The wedge has to be sharp: what does Cradle have that the top 3 competitors do not?

**Top competitors:**
- WeGLOW — postpartum workouts with explicit 'time/equipment/how you feel' filters and habit-not-punishment progress tracking, already occupies the gentle-tracking lane.
- MomsLab — postpartum-only app with psychologist+coach guidance, user reviews specifically cite reduced guilt.
- Natal (Pregnancy & Postpartum) — personalized plans across TTC/pregnancy/postpartum, pelvic floor and scar tissue focus, recent launch.
- Postpartum Journey — daily logging, AI chat, mental + physical recovery for mom (not baby), holistic like Cradle.
- Expectful — large install base (500k+), maternal mental health + meditation, generously framed and well-funded.

## retention-validator: `STRUCTURAL_RETURN`

The job (stay minimally healthy through postpartum) recurs daily and the 10-second check-in is sized to clear on hard days, so need recurrence is strong. SDT: compétence is Strong (generous logging reframes tiny acts as wins, biweekly trend pullback shows progress), autonomie is Strong (bar adjusts to user's week, no streak guilt, user owns the pace), lien social is Absent (no peer or coach layer described). Habit loop closes on an internal cue (waking up tired with the baby, the daily 10-second check-in) with an immediate reward (generous logging, permission, visible "I did something today"), not dependent on push. Two of three angles pass clearly (recurring job + 2 Strong needs + internal-cue loop), so STRUCTURAL_RETURN, with the social dimension and the 18-month horizon question as the main residual risks.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Cradle has a sharp, emotionally precise positioning — the "lower the bar on purpose" frame is concrete and the persona (postpartum parent who quit MyFitnessPal/Noom) is well-defined enough to simulate. Section 2 answers the daily mechanics convincingly: 10-second check-in, generous logging, biweekly pullback. But three core assumptions go unanswered: (1) that a postpartum mother in survival mode will open ANY app daily when she barely has hands free, (2) that "generous logging" feels validating instead of patronizing once the novelty wears off, and (3) that this is a standalone app rather than a feature competitors will ship. The spec also has no answer for trust/clinical safety (diastasis recti, pelvic floor, C-section recovery) which is a hard objection from this exact user. Solid frame, soft foundations.

**Dangerous assumptions:**
- Postpartum mothers in survival mode will actually open a phone app daily — the spec assumes the bar problem is 'the plan is too big', but the real bar may be 'I cannot pick up my phone'. Cheap test: 5 user interviews with mothers 0–6mo postpartum, ask 'when did you last open a non-essential app yesterday?' before pitching anything.
- Generous logging ('walk to the mailbox = movement') feels validating, not infantilizing. The H2 target of 70% feeling 'more in control' may invert if users feel the app is lying to them about progress. Cheap test: Wizard-of-Oz a 2-week version via SMS with 10 users, measure whether they keep replying or feel mocked.
- This is a defensible standalone product rather than a postpartum mode that Apple Health, Noom or Flo will ship in 6 months. The spec's own open question flags this. Cheap test: check if any of the apps users quit have already announced postpartum modes; if yes, the moat is the tone, not the feature, and that needs explicit defense.
