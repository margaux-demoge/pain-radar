# TIER

> **A dating app where the free version actually works.** No paywalled likes, no hidden matches, no "upgrade to see who liked you." You pay only if you want to skip the queue.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You downloaded Tinder, swiped for an evening, got a couple of matches, and the next day the app told you that you had run out of likes. To get more, $20. To see who liked you, $30. To boost your profile so your matches do not all come from 50 miles away, another $15. The free version is now barely functional. Even the paid version feels designed to keep you paying, not to actually match you. You start to suspect the algorithm is making you worse at this on purpose, so you will pay to dig yourself out. You either fork over the money and feel cheated, or you keep swiping into a void and feel ignored.

**Target users**

Primary: 22-35 year olds actively dating who use Tinder, Bumble, or Hinge and have hit the paywall wall. They will pay for a dating app, but only if the free version proves it works.

Not for: people who refuse to pay anything ever (the unit economics do not support pure free), or hookup-only users who already have the apps they want. Tier is for people looking for relationships who want a fair deal.

---

## 2. Product experience

Tier has two tiers, and that is the entire monetization story. Free, and paid. Free is fully functional: unlimited likes, you can see who liked you, you can message anyone you match with, you can filter by the things that matter (age, distance, intent). Nothing is artificially throttled. The free user has a real shot at finding someone on the app.

The paid tier exists for one reason: speed. If you pay, you skip the queue. Your profile is shown to more people sooner. Your messages reach matches without a daily limit on conversation starts. You can see profiles up to a week ahead in the discovery deck instead of waiting for them to surface. We do not unlock features behind the paywall, we unlock time.

The matching itself is built on stated preferences plus actual behavior, not on engagement maximization. The app does not throttle your matches to nudge you to pay. We publish, every month, the median number of matches per active user in each metro and age bracket. The number being public means we cannot quietly degrade it.

Tier makes money in two ways: a monthly subscription for the queue-skip tier, and that is it. No à la carte boosts, no super-likes-for-sale, no consumable items, no ads. The product economics force us to compete on whether the app actually works.

In short: free version that finds you matches, paid version that finds them faster, no other levers.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------ |
| H1  | Free users actually find matches and conversations at meaningful rates, validating that the unlocked free tier works.| % of active free users with at least one conversation reaching 5+ messages, within 14d. | TBD    |
| H2  | A non-trivial share of free users converts to the queue-skip tier because they want speed, not features.            | Free-to-paid conversion at day 30.                                                       | TBD    |
| H3  | Publishing median-matches data sustains trust and drives acquisition vs. competitors known for paywall tricks.      | % of new signups citing "fair pricing" or referral, plus organic press/social mentions. | TBD    |

---
