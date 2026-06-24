# BETA

> **Someone watching you climb, every send.** Film a 30-second attempt, get the wall read, learn the beta your body actually needs.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You climb alone in a gym full of people. You top a V4 and you don't know if you flowed it or muscled through. You watch the strong climber next to you flag a heel where you used a knee bar and you wonder which one was right for your body. YouTube beta is for someone else's reach, someone else's weight, someone else's wingspan. The gym has plenty of climbers but nobody is filming you, and the social cost of asking a stranger to read your climb is high, so you keep redoing the same problem the same wrong way. By the time someone happens to watch, the route has been stripped and the lesson is gone.

**Target users**

Primary: gym boulderers climbing V2 to V6, going at least twice a week, plateaued on technique rather than strength. They already film their sends sometimes for their own camera roll and would film more if there was a point. Mostly solo or in loose pairs, not part of a coached team.

Not for: outdoor trad climbers, ropes-focused gyms where every climber has a belay partner already watching, or competition athletes with coaches.

---

## 2. Product experience

Beta turns every solo attempt into a climb that gets watched.

You film a single send or attempt, 30 seconds max, vertical, framed so the wall and your body are both in shot. Beta asks for three things on top of the video: the gym, the wall section, and the grade. Hold colour and route tags are auto-detected from the wall scan when possible, the way the recent r/bouldering app demos do, so the route gets identified without you typing it. You post the climb, and it lands in the queue for that route specifically, not in a global feed.

The feedback is anchored on the body, not the comments. Climbers reviewing your clip can drop timestamped annotations: a tap on your hip at second 4 with the note "drop your weight here", a tap on your foot at second 7 with "this is the heel everyone misses". Annotations show up as pinned moments on the timeline, not as a thread underneath. You watch your climb back and the notes appear over the frames they belong to. The target is the first annotated read within a couple of hours, because the climb is still fresh in your body and you have the route for another week before the setters strip it.

The route page is the unit of community. Every climb of the same problem stacks together: yours, the local strong climber's, the setter's intended beta if they post one. You can see four people sending it four different ways and pick the version that matches your reach and your weight. The "standard beta" emerges from the cluster, not from one authority, and the creative variations are tagged separately so a 5'4" climber can find the 5'4" beta without scrolling past three 6'2" sequences.

Reviewer credibility is earned the way it should be: by climbing. Annotations from climbers who have actually sent the route at your grade or above carry more weight, and the app surfaces those first. There is no general reputation score, only per-route, per-grade-band trust. The gym surface stays local, so the people reading your climb are mostly people who climb at the same wall and recognise the route by sight.

In short: you film the climb, the route page reads your body, and the beta finds you instead of the other way around.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | ------ |
| H1  | Climbers will film and post a clip when the upload is one route, one wall, under a minute.                        | % of weekly active climbers who post at least one clip per week.                        | 40%    |
| H2  | Per-route community shows up with body-anchored feedback fast enough to act on before the route is stripped.      | % of posts that receive at least 2 timestamped annotations within 24 hours.             | 55%    |
| H3  | The collective beta on a route page is good enough that climbers change their sequence on the next attempt.       | % of posters who report trying a new beta from the page on their next session.          | 35%    |

---
