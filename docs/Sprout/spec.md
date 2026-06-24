# SPROUT

> **A second opinion before the plant dies.** Photo, conditions, diagnosis in under an hour, while there is still time to save it.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

Your monstera has three brown leaves and the new growth is yellowing. You google it and the first result says overwatering, the second says underwatering, the third says root rot, the fourth says you need more humidity. You don't know which one is true and the plant doesn't have another week to wait. You post on r/houseplants, the comments come in slowly and contradict each other, half of them ask for more photos you already posted. By the time anyone gives you a confident answer, the plant has dropped two more leaves or you have already watered it again on the wrong advice. There is no second opinion when you need it, only a slow committee that arrives after the plant is past saving.

**Target users**

Primary: home plant parents with 5 to 30 plants, mostly indoor tropicals, who have lost at least one plant they cared about and would have paid to know what was wrong in time. They already lurk on r/houseplants and have asked for help there at least once.

Not for: gardeners working with outdoor crops or vegetable beds (different problem space, slower failure mode), or commercial growers.

---

## 2. Product experience

Sprout is a triage room for sick plants, built for speed because plants don't wait.

You open the app on the plant that is dying. The post is a structured intake, not a free-form caption. Two photos (one wide, one close on the symptom), species (auto-suggested from the image), pot type, light direction and hours, last watering, watering frequency, room humidity if you have a meter, recent moves or repots. The whole intake takes under two minutes because every field is a tap or a preset, not typing. You hit post and your plant lands in the Triage queue, which is sorted by urgency markers (wilting, mushy stems, fast-spreading symptoms) not chronologically.

The diagnosis comes back as a stacked vote, not a thread. Other plant parents tap your post and choose from a structured set: overwatering, underwatering, root rot, light too low, light too strong, pest (with sub-types), nutrient deficiency, normal acclimation, needs more info. They can add a one-line note. You see the cluster build in real time: six people say root rot, two say overwatering, one says needs more info. The target is a confident cluster within the hour, because the next watering decision is often tonight.

Reputation is earned, quietly. Plant parents who have diagnosed many cases that were later confirmed (the original poster taps "this was it" days later when the plant recovers) carry more weight in future diagnoses. A small layer of verified plant identifiers handles rare species ID. There is no public leaderboard chase, just a faint badge that says this person reads plants well, and their vote weighs more in the cluster.

Your plants live on as a roster. Each plant has its own page: the photos over time, the symptoms it has had, the diagnoses the community gave, what worked, what killed it. After a few months a plant parent can see their own patterns (the spot by the west window keeps killing things, the calatheas always crash in winter) without having to remember any of it. The collective pattern across all users also builds quietly in the background: monstera + brown edges + humidity under 40% tends to cluster around X, so the next person posting that combination gets faster context.

In short: you post the sick plant, the community diagnoses it within the hour, and the plant gets a real chance because the answer arrives in time.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | ------ |
| H1  | Plant parents will post a sick plant when the intake is structured and fast.                                       | % of weekly active users who post at least one triage per month.                        | 40%    |
| H2  | The community arrives fast enough to be useful before the plant declines further.                                  | % of triage posts that reach a confident diagnosis cluster within 60 minutes.           | 55%    |
| H3  | The diagnosis is right often enough that plants recover when the advice is followed.                               | % of confirmed recoveries (poster taps "this was it") within 14 days.                   | 35%    |

---
