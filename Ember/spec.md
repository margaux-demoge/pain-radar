# EMBER

> **Proof you still love each other, even when it doesn't feel like it.** Ember catches the small moments your brain forgets and shows you the relationship your feed-state can't see.

---

## Status

- Phase 1 Exploration: stub from radar 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

The first year was electric. You couldn't stop touching them, every text was a small event, you'd cancel plans to stay in bed. Now it's been two years, three, and something has gone quiet. They're still kind, still yours, but the butterflies are gone and you can't tell if that means the relationship is dying or if it just means you're past the honeymoon phase. Friends say "that's normal, it deepens," but normal doesn't help when you're lying next to them feeling nothing. You scroll through your camera roll looking for proof you used to be in love and the photos are there but the feeling isn't. The hardest part is you can't tell anyone, because saying "I think the spark is gone" sounds like the prelude to leaving, and you don't want to leave. You just want to know if what you're feeling is the floor of a long relationship or the start of its end.

**Target users**

Primary: 23-32 year olds, 18 months to 4 years into a relationship they don't want to leave but can't currently feel. Often the higher-feeling partner in the pair. They've Googled "is the honeymoon phase ending normal" and gotten a wall of Quora; they want data on their own relationship, not generic advice.

Not for: couples in crisis or actively considering breakup, the surface area is too low for that work. Also not for new relationships, Ember needs at least a year of history to be meaningful.

---

## 2. Product experience

Ember runs in the background of your existing life. With permission, it watches the signals that already exist: how often you text each other, the length of the threads, your camera roll for photos of them, your calendar for time spent together. It doesn't add work, it reads what's already happening.

Every Sunday, Ember sends you one screen. Not a dashboard, not a chart wall. One observation about the past week, written like a friend who'd noticed something. "You sent each other 40 photos this week, the most since March." Or "You haven't been in the same room for four evenings in a row. Last time that happened you both got snappy on Sunday." The point isn't to grade the relationship, it's to surface what your in-the-moment feeling can't see.

When you tap deeper, Ember shows you the year so far as a quiet line, the rhythm of contact, the clusters of good weeks, the dips that lined up with their work trip or your sister's wedding. You see the shape of the thing you're inside. The "spark is dead" feeling, plotted, often turns out to be a six-week dip in a steady line, not the beginning of an ending. Sometimes it turns out to be the beginning of an ending. Either way, you stop guessing.

You can mark moments yourself, photos, dinners, fights, anniversaries, and Ember weaves them into the same line. Over time, the app gets specific to the two of you: it knows your version of a good week looks like three evenings together plus one shared meal out, not like other couples' versions. It compares you to you, not to anyone else.

In short: stop guessing whether the love is gone. See the year, see the rhythm, and find out what your feeling actually means.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | ------ |
| H1  | The weekly observation lands as meaningful, not generic: users feel it describes their actual week, not a horoscope. | % of weekly observations rated "felt true" by user (thumbs up in-line).                  | 65%    |
| H2  | Surfacing the rhythm reframes the user's in-the-moment feeling: they leave the app less anxious about the relationship's trajectory. | % of sessions ending with user reporting "I feel more clear" vs "more worried".         | 55%    |
| H3  | The data foundation is good enough that the weekly observation is grounded: signals correlate with self-reported relationship state. | Correlation between weekly Ember "rhythm score" and user-reported "felt week" rating.   | 0.5+   |

---
