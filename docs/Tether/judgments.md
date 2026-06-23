# Tether — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "presence / memory / mindful parenting" space is densely populated: Tinybeans (consolidating, just absorbed Qeepsake), TinyPal, MamaZen, Enjo, Kiddays, Little Moments, and Reflection App all touch some combination of daily prompts, memory journaling, and parent mindfulness. None of them is built explicitly on the guilt of attention-absence with a micro-dose presence loop, which is a real wedge, but the mechanics (daily prompt, weekly recap, kid memory log) overlap heavily with existing products. Few visible failed attempts at this exact angle, the indexed casualties are co-parenting/logistics apps (AppClose, TalkingParents free tier) rather than presence apps, which suggests the failure pattern here is silent stagnation rather than public shutdown. The wedge has to be sharp. What does the team have that Tinybeans, TinyPal, and MamaZen do not?

**Top competitors:**
- Tinybeans, private family memory journal with photos/milestones, now consolidating the category by acquiring Qeepsake, active (tinybeans.com)
- TinyPal, daily research-based parent prompts paired with planner and AI child-development coaching, active (tinypal.com)
- MamaZen, mindful parenting app with reflection journal and guided prompts, active (mamazen.com)
- Enjo, daily mindful family reflection prompts (gratitude, meaningful moments), active (referenced in MamaZen 2025 roundup)
- Kiddays, private ad-free child memory journal capturing small moments, active (kiddays.app)

## retention-validator: `STRUCTURAL_RETURN`

The job (showing up briefly for your kid) recurs daily because parenting recurs daily. Compétence is Strong via the visible accumulating mosaic of presence moments, and the habit loop has a strong internal cue (the parental guilt at end-of-day / scheduled moment) with an immediate emotional reward (relief, "that counted"). Autonomie is Weak (user picks the time but not the prompt content), Lien social is Absent (no other-human connection through the app). Two of the three angles pass: naturally recurring job, and a habit loop with internal cue plus immediate reward. The risk is over-reliance on push to deliver the daily prompt, which should be watched, but the underlying guilt-trigger is internal enough to survive notifications-off.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Tether has a beautifully written emotional wedge and a clearly defined target (working parents of 2-10 year olds, distracted, guilt-ridden). The problem framing is sharp and differentiated from milestone/screentime apps. But the spec leans heavily on the assumption that guilt-ridden parents will voluntarily open an app that reminds them of their guilt daily, and that a 5-minute prompt clears the actual blocker (which is attention, not ideas). The product experience is concrete enough to interview against, but core retention and trust assumptions are unanswered: why open the app at all once you feel seen, why trust prompt quality, and whether the "soft" no-punishment posture survives a week of misses without becoming invisible.

**Dangerous assumptions:**
- Guilt-ridden parents will open a daily reminder of their guilt. The spec assumes the wedge attracts; it may repel exactly the people most affected, who already avoid parenting content for this reason. Cheap test: post the Tether pitch on r/Parenting and r/workingmoms and measure whether replies are 'I need this' or 'this would make me feel worse' — ratio over 50 comments.
- The blocker is having ideas, not having attention. Spec assumes a prompt unlocks the moment, but parents in the evidence threads describe being mentally absent, not idea-less. A prompt may be answered with 'yes I'll do it later' and forgotten. Cheap test: 10-parent concierge week — text one prompt/day manually, measure same-day completion rate and ask what stopped them when they skipped.
- The weekly mosaic + kid-memory log creates enough pull to retain past novelty (H3 = 40% at week 12). Nothing in the spec explains why a parent returns after they've already 'felt seen' once. Cheap test: show 5 parents a mocked week-4 mosaic + memory log and ask 'would you open this app tomorrow, and why' — listen for whether the artifact or the prompt is the hook.
