# Truce — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

Price history and "is this sale real" verification is a heavily occupied category. Keepa and Camelizer dominate Amazon, while Karma (100K+ retailers), Honey/Droplist (200+ stores), Capital One Shopping (ex-Wikibuy, 100K+ stores), PriceBlink, and Google Shopping's native price-tracking feature cover the multi-retailer space Truce is targeting. The recent Honey scandal (lost ~3M of 20M users in two weeks after the MegaLag exposé) is the real opening: trust in incumbent extensions cracked, but several well-funded competitors are already serving the cross-retailer price history use case Truce describes. Truce's wedge (a calibrated 1-word verdict, no affiliate conflict, crowdsourced snapshots) is plausible but not unique enough on its face. Sources: [Karma top trackers](https://www.karmanow.com/the-blog/top/the-best-price-trackers), [CamelCamelCamel alternatives](https://rigorousthemes.com/blog/best-camelcamelcamel-alternatives/), [Honey lawsuit / 3M user loss](https://en.wikipedia.org/wiki/PayPal_Honey), [Keepa Chrome](https://chromewebstore.google.com/detail/keepa-amazon-price-tracke/neebplgakaahbhdphmkckjjcegoiijjo).

**Top competitors:**
- Karma — price tracking + drop alerts across 100K+ retailers via extension and app, active and growing
- Honey (PayPal) Droplist — price drop tracking across 200+ stores incl. Walmart/Target, active but reputation-damaged post-2024 lawsuit (real wedge for Truce)
- Capital One Shopping (ex-Wikibuy) — cross-retailer price comparison and history, active, distributed via Capital One
- Keepa — deep price history on Amazon, the de facto standard browser extension, active
- PriceBlink — multi-retailer browser extension comparing live prices and historical lows across thousands of US stores

## retention-validator: `STRUCTURAL_RETURN`

Job (verify if a sale price is honest) recurs every time the user shops online, which for the target is weekly+. Habit loop has a strong internal cue (seeing a sale badge triggers suspicion) plus an external cue via watchlist drops, with verdict reward delivered in under 2s. SDT is thinner: competence is weak (sense of not-being-fooled, but no real progression), autonomy is strong (user judges, app refuses to prescribe), social is absent despite crowdsourced data being invisible to users. Two of three angles pass clearly: recurring need + closed habit loop with internal cue.

## user-interview-simulator: `BUILT_ON_SAND`

Truce has a sharp pain ("sale badges lie") and a credible persona, but the spec leans on three structurally fragile bets: cold-start catalog coverage outside Amazon, a 2-second verdict over scraped pages, and a behavior change ("I won't buy") on top of a friction-heavy share-sheet flow. The hypotheses table acknowledges the coverage and speed risks but offers no plan to de-risk them, and the spec admits the legal exposure is unknown. A skeptical shopper would land on "unclear" too often, lose trust on the first miss, and revert to gut feel before any habit forms.

**Dangerous assumptions:**
- Crowdsourced + scraped coverage will hit 60% non-unclear verdicts by month 3 across non-Amazon retailers. Why dangerous: bootstrap is circular (no users -> no snapshots -> 'unclear' -> users leave). Cheap test: pick 200 real product URLs from r/Frugal hauls and measure how many already have 90-day history available via public sources today, before writing code.
- A 'fake deal' verdict actually stops a purchase 40% of the time. Why dangerous: the spec assumes outrage beats sunk-cost of having found the product; most shoppers rationalize and buy anyway. Cheap test: Wizard-of-Oz over Telegram/SMS — 20 users send product links, you reply with a verdict by hand, track 24h purchase outcome.
- Users will adopt a share-sheet detour in the 'few seconds between seeing a price and tapping buy'. Why dangerous: every extra tap during checkout intent has historically collapsed conversion of price-check tools outside the Amazon-native CCC case. Cheap test: prototype the iOS share-sheet (static verdict), give to 10 target shoppers for 2 weeks, measure unprompted invocations per week, not satisfaction.
