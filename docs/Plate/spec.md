# PLATE

> **Point your camera at your food, and it logs itself.** Calorie tracking without the search bar, the database, or the gram-by-gram weighing.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You want to track what you eat. Not because you love tracking, but because it works: you have lost weight or gained muscle before, and the times it worked were the times you logged. So you opened MyFitnessPal, and the friction begins. Search "chicken." 4,000 results, half of them wrong, half user-generated entries with no nutrition data. Add grams. Did you cook it with oil? Add the oil. The salad on the side. The dressing. Every meal is a 4 minute data-entry chore, and dinner is usually three things on a plate. By day five you stop logging the snacks. By day ten you stop entirely. Not because you do not care, but because the tax of caring was too high.

**Target users**

Primary: 25-45 year olds with a real fitness or weight goal who have tried MyFitnessPal, LoseIt, or Cronometer and quit because manual logging is unsustainable. They have a phone with a decent camera and are willing to pay for a tool that actually fits their life.

Not for: athletes or bodybuilders who need gram-level precision for competition prep, or people with medical conditions requiring exact macro tracking. Plate trades a small amount of precision for a large amount of consistency.

---

## 2. Product experience

Plate opens to a camera. You point it at your plate, snap, and within 2 seconds it has identified what is on the plate, estimated the portions visually using known plate-size references, and logged the meal with calorie and macro estimates. You can correct anything by tapping: "that's not chicken, it's turkey," "the rice portion is bigger than that." The corrections train the model on your eating patterns over time.

For packaged food, you scan the barcode and it logs. For restaurant meals, you can search a menu by restaurant name and tap the dish, no gram math. For meals you cook regularly, after the second or third time, Plate remembers and offers them as one-tap entries: "your usual breakfast."

The dashboard is deliberately simple. You see today's calories and macros against your target, and a 7-day moving average so a single bad day does not feel like failure. There are no charts of streaks, no badges, no "you crushed it" notifications. The app's job is to keep logging frictionless, not to motivate you, that is your job.

The bet is precision-vs-consistency. A photo estimate might be off by 10-15% on any one meal, but a logged meal beats an unlogged one every time. Plate is built around the truth that the best tracking method is the one you will actually do every day for a year.

In short: snap your meal, the app does the math, you keep logging.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------ |
| H1  | Photo-based logging is fast enough that users sustain it well past the typical MFP dropoff point.                    | % of paying users logging 5+ meals/week at day 60.                                       | TBD    |
| H2  | Calorie estimates from photos are accurate enough (within ±10-15%) that users hit their weight goals at comparable rates to manual logging. | Self-reported goal progress at day 90 vs. published MFP benchmarks.                     | TBD    |
| H3  | The friction reduction unlocks a user segment that never stuck with manual tracking.                                | % of paying users who self-report having quit a manual tracker before signing up.        | TBD    |

---
