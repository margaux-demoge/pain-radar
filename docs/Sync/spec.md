# SYNC

> **A dating app whose algorithm works for you, not against you.** No artificial scarcity, no "boost to be seen," no shadow throttling. The matching logic is published.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You have been on Tinder long enough to notice the pattern. The first week was great, matches came in, conversations started. Then something changed. The matches dried up. The same profile that worked in week one is suddenly invisible in week three. You suspect the app is throttling you, deliberately making it harder so you will pay for a boost. You cannot prove it. The algorithm is a black box and the company will not say how it works. So you either pay, and it briefly improves, just enough to make the pattern obvious, or you delete the app, knowing you were not unmatched, you were starved. The relationship between you and the app is adversarial: their growth depends on your dissatisfaction.

**Target users**

Primary: 25-40 year old dating-app veterans who suspect they are being throttled or manipulated by Tinder, Bumble, or Hinge. They are tired of paying ransom to algorithms they do not understand.

Not for: casual users who do not think about how matching works and just want the most popular app. Sync is for people who have read the discourse about dating-app dark patterns and are looking for an alternative built on the opposite premise.

---

## 2. Product experience

Sync's matching algorithm is published. The exact ranking function, with weights, is on the website and inside the app's settings page. It is a small set of factors, most of them under your control: stated preferences, mutual interest signals (you liked similar profiles, you spent time on similar prompts), distance, and recency of activity. There is no opaque "desirability score," no ELO, no engagement-maximization loop.

You see, in your own dashboard, exactly how many people your profile was shown to in the last 7 days, how many viewed it, and how many liked. If the number drops, you can see whether it dropped because fewer eligible people were online, because your preferences narrowed, or because your profile quality changed (a photo got fewer responses). The data is yours and it is legible.

There are no boosts to buy. There is no super-like economy. There is no priority placement for paying users. Every user is ranked by the same function. The monetization is a flat subscription that unlocks advanced filters and unlimited messaging, but does nothing to alter how the algorithm ranks you.

Sync also publishes, monthly, the aggregate match-rate distribution across the user base, broken down by metro and age. If the median user is getting two matches a week and the platform is claiming five, the data exposes the gap. The number being public is the discipline that keeps us honest.

In short: a dating app where the algorithm is on your side, the data is yours, and the company cannot quietly turn the dial against you.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------ |
| H1  | Algorithm transparency is a strong enough wedge to pull skeptical Tinder/Hinge users into trying a new app.         | % of new signups citing "algorithm trust" or coming from dating-app-criticism content.   | TBD    |
| H2  | A transparent, non-manipulative algorithm produces match outcomes (date frequency, relationship formation) at parity with incumbents. | Self-reported "had at least one date from a Sync match" at day 60.                      | TBD    |
| H3  | The monthly aggregate transparency report becomes a trust-building artifact that drives organic acquisition.        | Monthly report views, share count, and resulting signups attributed to it.               | TBD    |

---
