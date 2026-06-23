# Worth — judges verdicts

## benchmark-scanner: `EMERGING`

No app surfaced that targets the exact wedge — adults who have explicitly conditioned dating on hitting a weight target and need to decouple the two. The closest plays split into two camps that don't meet in the middle: (a) body-image/self-worth CBT apps (Worth Warrior, Body+) that ignore dating, and (b) plus-size dating coaches (Curvy Cupid, Kelsey Wonderlin, Date Brazen) that ignore the weight-loss-as-prerequisite mental contract. The "I'll date when I lose the weight" frame is well-documented in r/loseit but is unaddressed as a product category. Window is open, but the wedge is narrow and the name "Worth" collides with an existing NHS-recommended app.

**Top competitors:**
- Worth Warrior (stem4, UK NHS-recommended) — CBT app for body image and self-worth in young people, free, clinician-built; adjacent problem but name collision is a real branding risk. https://apps.apple.com/us/app/worth-warrior-help-body-image/id1641866414
- Curvy Cupid Course (Krista Niles) — group online course teaching plus-size women a step-by-step dating approach; closest to Worth's dating-action layer, but built on body acceptance not weight-loss-decoupling. https://christyharrison.com/foodpsych/6/how-to-find-love-at-every-size-with-krista-niles
- Babecamp (Virgie Tovar) — 4-week online course to 'break up with diet culture'; targets the same internal contract but pushes anti-diet ideology rather than Worth's neutral decoupling stance. https://www.virgietovar.com/courses.html
- Body+ App — 500+ CBT challenges on appearance-based shame and fear of judgment; covers the inner work but never crosses into dating action. https://apps.apple.com/us/app/body/id1240093612
- Date Brazen / Main Character Dating (Kelsey Wonderlin, Hayley Quinn Real Academy) — 6-week dating coaching programs for women; same format as Worth but treat body image as a side topic, not the core blocker. https://datebrazen.com/dating

## retention-validator: `WEAK_RETURN`

The job ("decouple my dating life from the scale") is explicitly framed as a one-shot, finite 6-week course — by design the user graduates and leaves, so natural need recurrence fails. SDT is partially nourished: competence is Strong (the freeze-meter bends weekly, visible progress on Worth's own axis), autonomy is Weak (linear sequence, app dictates the path), social relatedness is Absent (no peers, no coach in-loop confirmed). Habit loop has a weekly external cue (the program cadence/push) rather than an internal one, with a reflective reward that is meaningful but not instantly felt in seconds — the loop closes once a week at best and dies at week 6. Only competence clearly passes, so exactly one angle holds: WEAK_RETURN, consistent with the open question in the product log about whether a 6-week finite course is a viable shape.

## user-interview-simulator: `BUILT_ON_SAND`

Worth identifies a real, specific emotional pattern (the conditional-on-weight dating freeze) and writes about it with empathy, but the spec leans almost entirely on assertion rather than evidence that this user will (a) self-identify with the framing, (b) pay for or download a 6-week emotional course rather than continue scrolling r/loseit, and (c) trust an app to mediate this shame-loaded territory without a therapist. The core mechanic (measuring "freeze" via weekly questions) is a novel metric users have no relationship to, and the wedge against BetterHelp/Noom/dating apps is unresolved in the product log itself. Persona is constructible but the simulated user pushes back hard on almost every pillar.

**Dangerous assumptions:**
- Target users will self-identify as 'I'm waiting to date until I lose weight' and seek a product for it. The Reddit evidence shows the theme exists in venting, but venting on r/loseit is not the same as downloading a separate app that names the shame back to you. Cheap test: a landing page with the exact spec headline and a waitlist CTA, run as a paid ad to r/loseit lookalikes, measure click-through and email capture.
- A 6-week finite course produces enough perceived value upfront to get a week-1 user to commit, when BetterHelp offers a human and Noom offers a familiar shape. The spec offers no reason a skeptical user picks Worth over a $20 therapy session or a journaling app. Cheap test: 5 user interviews with women 25-40 in active weight loss, show the pitch, ask what they'd pay and what they'd compare it to.
- The 'dating freeze' can be moved by weekly prompts and small tasks without a human in the loop. This is the territory where content-only apps historically fail (shame + avoidance + identity). Cheap test: run the week-1 and week-2 content as a manual concierge over WhatsApp with 5 users, measure whether the freeze score actually moves before building anything.
