# Bare — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The personalized skincare-routine space is dense with both brand-backed AI advisors (L'Oréal Skin Genius, La Roche-Posay MyRoutine, Cetaphil MySkin) and independent apps (SkinSort, Lóvi, OnSkin, TroveSkin, FeelinMySkin, SkinGenie, Charm). Bare's wedge is not "another personalized routine" but the radical-subtraction promise (three products, hold the line, refuse additions) plus an explicit no-affiliate stance. The closest in spirit are SkinSort/Lóvi/OnSkin (independent, ingredient-led) and The Ordinary's "Simple 3-product" regimen tier, but none enforce a minimalist routine as a behavioral product mechanic. Failure signals are weak because most players are still alive, but Curology-style prescription models have well-documented user disappointments around added complexity and bias.

**Top competitors:**
- SkinSort, independent skincare scanner with routines and shelves, brand-agnostic, ingredient-led, active. https://skinsort.com/
- Lóvi, AI skincare scanner positioned as 100% independent, science-based recommendations from a 500K+ product DB, active. https://apps.apple.com/us/app/lovi-ai-skin-care-scanner/id1594167292
- TroveSkin, photo-based skin coach with personalized routines and weekly tracking, active and updated 2026. https://www.crunchbase.com/organization/troveskin
- The Ordinary Regimen Builder, free brand tool that explicitly offers a 'Simple (3 products)' tier, the most literal overlap with Bare's promise. https://theordinary.com/en-us/regimen-builder.html
- SkinGenie / Charm / FeelinMySkin, AI quiz-to-routine apps with progress tracking and product recommendations, all active in 2025-2026. https://www.skingenie.beauty/

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Tell me exactly what to put on my face every day so I can stop researching skincare and just see results.
Classification: naturally recurring (the underlying act, washing/applying skincare, happens twice daily), but with a twist: once the user has memorized the three products, the *informational* job is one-shot. Application itself does not require an app.

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. There is a weekly 1-5 rating and optional photo, plus learning one ingredient at a time, but progress is slow and skin improvement signal is noisy week to week.
- Autonomie (sentiment d'être en contrôle): Weak. Paradoxical, the product's core stance is to override the user's autonomy ("no, don't add that"). Users get clarity but not agency. Some might experience this as relief, others as constraint.
- Lien social (sentiment d'être connecté à d'autres): Absent. No social, no sharing, no community, nothing in the spec connects users to other humans.

**Boucle d'habitude**
- Déclencheur: morning and evening skincare moment, INTERNAL (tied to existing bathroom routine, this is the strongest part of the spec).
- Routine: two-tap log of "did the routine", plus a weekly 1-5 check-in.
- Récompense: confirmation you did the thing + ambient sense your face is getting better, immediate Y partial. The tap-log gives instant closure but the actual reward (better skin) lands over weeks, not seconds. No streak, no visible progress artifact in the spec.
- Push reliance: not explicitly stated, but a two-tap log without a strong on-device reward likely needs push to survive past week 2. The spec does not describe an on-app pull strong enough on its own.

**Verdict line**
One angle clearly passes, the habit loop has a strong internal cue anchored to an existing twice-daily ritual. The job recurrence is technically there but the *informational* value (the three products) is delivered on day one and not renewed, the user can memorize the routine and stop opening the app. Psychological needs are weak across the board, with autonomy actively suppressed by design and zero social fabric. The product risks becoming a glorified checkbox after week 3.

**What needs to change for STRUCTURAL_RETURN**
- What does the user *see* in the app after week 2 that they could not get from a Post-it on the mirror? Is there a visible progress artifact (photo timeline, skin score curve, ingredient education streak) that makes opening the app rewarding beyond the tap-log?
- Where does competence come in? Is there an explicit ladder (ingredient knowledge unlocked, "earning" the next move) that makes the user feel they are leveling up, not just complying?
- Is there any social or accountability layer, even minimal (a partner, a derm review, a cohort starting at the same time), that pulls the user back independently of push notifications?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Bare has a sharp, contrarian positioning (subtraction over addition) and a clearly defined overwhelmed user. But the spec leans heavily on unvalidated trust mechanics: why a stranger app's three-product verdict beats a dermatologist, a Reddit thread, or ChatGPT, and how the quiz produces a credible answer without bias. The "hold the line" feature is bold but untested — users may simply uninstall when told no, rather than feel protected. Monetization is acknowledged as existential in the log but absent from the spec, which directly undermines the no-affiliate promise.

**Dangerous assumptions:**
- Users will trust a quiz-driven app to name three ingredients for their face without any derm/MD credential or clinical basis. If wrong, the first recommendation screen kills install-to-activation. Cheap test: show 50 r/SkincareAddiction quitters a mocked three-product output and measure 'would you actually start this tomorrow' vs. 'I'd want a dermatologist first'.
- Users will experience 'no, don't add that' as care rather than as a paternalistic app blocking them, and won't just ignore Bare and buy the TikTok serum anyway. If wrong, H2 collapses and retention follows. Cheap test: Wizard-of-Oz a 2-week SMS version that tells 20 users 'no' when they ask to add something, measure compliance and NPS.
- Bare can stay ad-free and affiliate-free while still being economically viable, without that breaking the recommendation neutrality the entire product is sold on. The spec is silent on pricing; the log flags this as existential. If wrong, the product either becomes biased (premise dies) or never ships. Cheap test: price-test a $5–10/mo subscription on a landing page against the actual value prop ('we'll tell you the 3 things and refuse to upsell you') before building.
