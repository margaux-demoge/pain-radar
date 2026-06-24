# TRUCE

> **Is this actually a deal?** Truce checks any price against its real history before you buy, so the word "sale" stops being able to lie to you.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You're looking at a product and it says 40% off. You don't actually know what it cost last week. It could be a real discount, or it could be the retailer who marked it up by 50% three days ago to mark it back down today. You suspect the latter, more often than not, but you can't verify it in the moment, so you either trust the badge and feel stupid later, or you mistrust everything and pay full price for things that are genuinely discounted. The whole concept of "sale" is broken, and the only people who know are the merchandisers running the spreadsheets. Camelcamelcamel exists for Amazon, but nothing exists for everywhere else you shop, and it doesn't fit in the few seconds between seeing a price and tapping buy.

**Target users**

Primary: adults who shop online weekly and feel manipulated by sale pricing. They are not extreme couponers, just normal people who don't want to be played.

Not for: people who never look at price, or people who genuinely don't care about saving 20%. Truce is for the suspicious-but-not-obsessive shopper.

---

## 2. Product experience

Truce lives as a share-sheet extension and a browser extension. You see a product anywhere, share it to Truce, and within two seconds you see one verdict: real deal, fake deal, or unclear. Below that, a small chart of the actual price history of that exact product over the last 90 days, from the same retailer.

The verdict is calibrated, not generous. A "real deal" means the current price is below the median of the last 90 days. A "fake deal" means it was at this price or lower in the last month. "Unclear" means there isn't enough history to call it. The app explicitly does not tell you to buy or not buy. It just tells you whether the discount story is true.

Behind the scenes, Truce builds its price database by scraping public product pages and by crowdsourcing snapshots from its own users. Every time you share a product, the current price is logged, even if you don't buy. Over months this creates a community-owned price history for tens of thousands of products that no centralized retailer wants to expose.

Truce also has a watchlist. You can pin a product, and the app pings you only when the price actually drops below the lowest point of the last 90 days. No daily emails, no marketing, no "deals near you." The bet is that the people most ready to pay for this are not bargain hunters, they're people who hate being manipulated. The reward isn't saving money. It's the feeling that you can finally tell whether the badge is honest, and act accordingly.

In short: Truce shows you the price history behind any sale badge and tells you, in one word, whether the discount is real.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                | Metric                                                                              | Target |
| --- | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ------ |
| H1  | Shoppers will share a product to Truce before buying when the verdict is available in under 2 seconds.    | Median time-to-verdict, P95.                                                        | <2s    |
| H2  | The "fake deal" verdict actually changes purchase behavior.                                               | % of "fake deal" sessions where no purchase happens in the next 24h.                | 40%    |
| H3  | Crowdsourced price snapshots cover enough catalog to make the app useful outside Amazon.                  | % of share-to-Truce requests that return a non-"unclear" verdict by month 3.        | 60%    |

---
