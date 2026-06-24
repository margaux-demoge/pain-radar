# Yore — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

Generational nostalgia is a mature, well-trodden category. There is a direct, recently-launched competitor with Yore's exact wedge (When You Were: Nostalgia, cohort-keyed by birth year), an established editorial nostalgia social platform (DoYouRemember.com), and the dominant gravity well of Reddit's r/Millennials and r/nostalgia plus TikTok nostalgia niches where the behaviour already lives for free. Past attempts (Timehop, DailyBooth, Ello) show the failure pattern: personal-archive or generic-nostalgia apps get squeezed by platform giants (Facebook On This Day, Google Photos Rediscover) and struggle to keep users posting once the novelty fades. Yore needs a wedge sharper than "cohort feed", because that already exists.

**Top competitors:**
- When You Were: Nostalgia (Minner Labs) — daily personalized nostalgia feed keyed to your birth year, ages 5-18, 380+ curated items, the closest 1:1 match to Yore's cohort wedge (https://apps.apple.com/us/app/when-you-were-nostalgia/id6757958974)
- DoYouRemember.com — long-running nostalgia social network with memory posting, chat rooms, communities; editorial-led but covers same emotional contract (https://doyouremember.com/)
- Reddit r/Millennials and r/nostalgia — the de-facto home for generational 'remember when' posts, where Yore's own evidence base is sourced from, 1M+ subscribers combined
- Timehop — 20M+ users, pivoted from personal throwback to generic 'Nostalgic News' pop-culture cards, acquired by Sincere Corp 2023, shows the gravity of the space (https://en.wikipedia.org/wiki/Timehop)
- Geriatric Millennial / TikTok nostalgia accounts — 473k+ followers, free, algorithmic; the behaviour already happens on TikTok and Instagram without a dedicated app (https://www.boredpanda.com/nostalgic-posts-millennials/)

## retention-validator: `WEAK_RETURN`

The job ("feel a warm jolt of generational nostalgia") is occasional and emotion-triggered, not naturally recurring like eating or sleep. SDT-wise, lien social is the only Strong pillar (cohort resonance, "I remember too"); compétence is absent (no progression, mastery, or measurable growth) and autonomie is weak (cohort is set, feed is curated by resonance). The habit loop lacks a clear internal cue: nostalgia surfaces randomly in life, not at a predictable moment, and the spec does not name a recurring trigger that pulls the user back. Reward is immediate and emotional when a card hits, but the loop closure depends heavily on external cues (push, friends sharing into group chats per H3).

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

The emotional contract is clearly articulated and the cohort-feed wedge is sharp enough to construct a real persona around. But the spec dodges the three hardest questions any 32-year-old already-on-Reddit user would ask: why a dedicated app instead of r/Millennials, what stops the feed from drying up after the obvious memories (Dunkaroos, dial-up) are posted, and how the cold start works before the cohort is dense. Cold start and content sustainability are even flagged in the product log as open, and competitive substitution is not addressed at all. Positioning is coherent but rests on unvalidated retention assumptions.

**Dangerous assumptions:**
- Users will leave r/Millennials and TikTok nostalgia accounts for a dedicated app, when those existing surfaces already deliver the same emotional hit inside a feed they already open daily. If wrong, Yore has no wedge. Cheap test: post 10 Yore-style memory cards to r/Millennials and to a dedicated test feed, measure which gets stronger 'oh my god yes' engagement, and ask 20 target users whether they'd open a second app for this.
- A cohort's shared memory is a deep enough well to sustain a feed-format app past month 2. The product log itself flags this. If a 1992 cohort exhausts its 500 universal memories quickly, the feed flattens into long-tail niche posts that don't trigger the chest-thing. Cheap test: hand-curate 200 memory cards for a single cohort, show to 10 users across 4 weeks, measure how quickly the 'hit rate' (cards that trigger reaction) drops.
- The 15% weekly posting target is realistic for a passive nostalgia audience. Rememberers drop 'remember when' in group chats where the audience is captive and known; posting into a feed of strangers is a different muscle. If contribution stalls, the feed dies regardless of cold-start solution. Cheap test: run a Telegram/Discord group for 30 target users for 2 weeks, measure unprompted posting rate without any product polish.
