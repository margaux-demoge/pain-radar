# LOOP

> **Seven meals. That's your week.** Loop helps you find the small set of meals you actually cook and rotate them on repeat, guilt-free.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You wanted to cook for your family. You bought the cookbooks, you saved the Instagram recipes, you tried meal kits, and you still find yourself at 6:15pm staring into the fridge with nothing planned. By 6:30 you've ordered something, again. You feel like you're failing at one of the basic parts of being a parent or partner, which is feeding the people you love consistently. The cooking apps don't help, they hand you a thousand recipes and zero structure. Pinterest hands you ten thousand. The actual problem isn't that you don't know what to cook, it's that decision-making at the end of the day is broken, and what you need is a small repeating rotation you barely have to think about. Nobody admits that good home cooking is mostly repetition.

**Target users**

Primary: parents and household cooks who feel chronically behind on home cooking, have tried meal kits, and want a simpler system. They cook three nights a week and want it to be five without it being a project.

Not for: cooking hobbyists who enjoy novelty, or people in food deserts where ingredient access is the actual problem.

---

## 2. Product experience

Loop starts by asking what you've actually cooked successfully in the last month. Just type the meal names. From those, plus a short interview about what your family eats and what you have for equipment, the app proposes seven dishes, total, that become your rotation for the next four weeks.

That's the whole product. Seven meals, on repeat, with the grocery list auto-generated and the cooking order suggested for the night. You get one easy weeknight meal, one ten-minute meal, one slow-cooker meal, one make-ahead meal, and three middle-difficulty meals you already know you like. Loop deliberately does not give you a different set every week.

Each night at 4pm Loop pings you with what tonight's meal is from the rotation, and a single tap takes you to the grocery list update or the recipe. If you cooked it, you tap a star. If you didn't, you tap a frown. After two weeks Loop knows which of the seven are landing and which aren't. The ones that aren't get gently swapped, one at a time, never the whole rotation.

The thing Loop won't do is overwhelm you with novelty. There's no recipe feed. There's no algorithmic discovery. The premise is that good family cooking is a small loop of reliable meals, and that the cultural pressure to cook something new every night is the actual reason you order in. Loop's reward is a quiet kitchen on Wednesday at 6pm, with food on the table and no decision made under fatigue.

In short: Loop gives you seven meals on rotation, swapped only when one isn't working, so dinner stops being a decision.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                | Metric                                                                              | Target |
| --- | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ------ |
| H1  | A fixed 7-meal rotation actually increases home-cook nights compared to a recipe app.                     | Median home-cook nights/week, week 1 vs week 4.                                     | +2     |
| H2  | The "swap one, not all" rule keeps users on the rotation long enough to find their stable set.            | % of users still using the same 7-meal rotation (with ≤2 swaps) at week 6.          | 50%    |
| H3  | Loop's restraint (no recipe feed) is the differentiator that earns retention vs. Mealime/Plan to Eat.     | % of week 4 users citing "doesn't overwhelm me" as a reason they stayed.            | 50%    |

---
