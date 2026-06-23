# Tier — judges verdicts

## benchmark-scanner: `GRAVEYARD`

The "anti-paywall, fair dating app" positioning is a well-worn pitch with multiple active and failed attempts. Facebook Dating already occupies the "100% free" extreme with 21.5M DAU; SciMatch markets unlimited free use; Thursday tried a differentiation play and shut down in 2025 citing "rapidly declining consumer interest." Even with Tinder/Bumble losing paying subs (8% and 16% drops), no challenger has converted that frustration into a sustained subscription-only business, suggesting the bottleneck is liquidity and distribution, not pricing fairness.

**Top competitors:**
- Facebook Dating — fully free, no paywall, no IAP, 21.5M DAU; the structural incumbent for the 'free actually works' promise (https://www.swipestats.io/blog/free-dating-apps-without-payment)
- SciMatch — markets unlimited swipes/likes/messaging free forever, sees-who-liked-you unlocked, positions explicitly against paywall apps (https://scimatch.com/unlimited-swipes-and-likes-returning-to-the-dating-scene/)
- OkCupid — long-standing free messaging, freemium but core matching unlocked (https://www.datingnews.com/daters-pulse/free-dating-sites-without-payment/)
- Hinge — freemium, but most-used 'relationships' app the target user is fleeing; still the default benchmark for 22-35 daters (https://www.mindbodygreen.com/articles/best-dating-apps)
- Plenty of Fish — free messaging, weaker brand but covers the no-paywall promise for older demos (https://www.datingadvice.com/online-dating/dating-sites-with-no-payment-or-subscription)

## retention-validator: `STRUCTURAL_RETURN`

The job (find a romantic partner / get matches) recurs daily while the user is single, which is a naturally recurring need with a strong internal cue (loneliness, evening downtime, post-work boredom). Lien social is Strong by category definition (the entire product is connecting with other humans), and competence is Weak (profile improvement, conversation skill) while autonomy is Weak-to-Strong (real filters, no manipulative algorithm). Habit loop closes well: internal cue (free moment, want to feel desired), routine (swipe), reward (immediate dopamine of likes/matches), and matches themselves create external cues via messages. Two of three angles clearly pass (recurring job + habit loop with internal cue and immediate reward), with lien social as a third anchor; the main risk is that the job terminates on success (user finds partner and churns), which is structural to dating apps not to Tier specifically.

## user-interview-simulator: `BUILT_ON_SAND`

Simulated user Jules, 29, Lyon, active on Hinge + Bumble, mildly burned by Tinder Gold. The spec sells a moral stance ("free actually works") but skips the hardest mechanics: how a brand-new app gets the liquidity Tinder has, how it filters bots without paywalls, how queue-skip is valuable enough to fund the company, and why a skeptical dater trusts a self-published median-match number. 6 out of 10 questions land as UNANSWERED or PARTIAL on questions the team almost certainly hasn't pressure-tested. The positioning is righteous but the unit economics, liquidity bootstrap, and trust mechanism are unvalidated, and they are exactly what would kill it.

**Dangerous assumptions:**
- Liquidity bootstrap: a dating app is worthless without dense supply on both sides locally. Spec assumes users will sign up for a fair deal, but Jules in Lyon needs hundreds of matches near him on day one or he churns in 48h. No GTM/seeding plan. Cheap test: pick one metro, run a closed waitlist with gender-balanced invite caps, measure 7-day retention against a 200-profile density floor before opening a second city.
- Queue-skip willingness-to-pay: spec asserts people will pay for speed alone when all features are free. This contradicts the entire dating-app monetization literature: people pay to unlock visibility (likes-you, rewinds), not to be served faster. Cheap test: fake-door a paid tier on a landing page with only 'skip the queue' as the offer and measure CTR/checkout-intent vs a Tinder-Gold-style feature bundle.
- Spam/bot economics without paywalls: removing the price-of-entry removes the cheapest spam filter. Spec says nothing about identity verification, invite gating, or moderation cost. Cheap test: estimate per-active-user moderation cost from public Bumble/Hinge data and check if subscription ARPU at realistic conversion (3-5%) covers it before a single match happens.
