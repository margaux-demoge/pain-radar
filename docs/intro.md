---
sidebar_position: 1
slug: /
---

> 🆕 **Interactive prototype gallery →** [/protos/](/protos/index.html)
>
> 45 HTML app prototypes (8 iPhone screens each), with thumbnails, filters, and click-through navigation.

# RADAR — pain radar v1
_Mined from 13.7K Reddit posts across 29 subreddits over the last 90 days. Filtered to 1,878 complaint-shaped posts. Clustered into 45 themes, materialized as 45 Phase 1 spec stubs._

**Pipeline:** arctic-shift (Reddit archive) → lexical complaint filter → 4 parallel LLM clusterers (one per typology) → name dedup → spec stubs.

---

## Methodology notes

- **No score column.** arctic-shift archives posts at creation, so engagement signal (upvotes, comments) was unusable. Frequency = number of distinct posts matching the theme.
- **No pre-filter (Amon-fit).** Per session decision: judges left for downstream.
- **Name collisions** resolved manually (Tally → daily_life kept, relationships' version renamed Ledger; Tether → daily_life kept, relationships' renamed Span; Verdict → app_critics kept, relationships' renamed Mull; Pulse → relationships kept, community_trends' renamed Cue).
- **Skipped 2 themes** from app_critics: 'privacy invaded' (freq 93) and 'can't delete account' (freq 34) — too generic, not Amon-shaped.

---

## Community-as-10x — niche passion communities where peer mechanic is the engine (5 stubs)

| App | Tagline | Origin signal | Freq | Subreddits |
|---|---|---|---|---|
| [**Beta**](./Beta/spec.md) · [log](./Beta/product_log.md) | Someone watching you climb, every send. Film a 30-second attempt, get the wall read, learn the beta your body actually n | I climb a route alone and can't tell if my form is efficient or if I'm using the | 22 | r/bouldering |
| [**Crumb**](./Crumb/spec.md) · [log](./Crumb/product_log.md) | A trained eye on every loaf you bake. Post your crumb, get diagnosed by bakers who have been there, learn faster than th | I bake sourdough alone and never know if my crumb is good | 75 | r/Sourdough |
| [**Lex**](./Lex/spec.md) · [log](./Lex/product_log.md) | A human on the other side, three times a week. Matched on language, level, and timezone, with the streak that keeps you  | I'm learning a language alone and have no one to speak with or stay accountable  | 19 | r/languagelearning |
| [**Loom**](./Loom/spec.md) · [log](./Loom/product_log.md) | Eyes on the piece before you've stitched another fifty rows. Post a WIP, get the tension and colour read, finish what yo | I'm halfway through a cross-stitch and want to know if I'm doing it right | 16 | r/CrossStitch |
| [**Sprout**](./Sprout/spec.md) · [log](./Sprout/product_log.md) | A second opinion before the plant dies. Photo, conditions, diagnosis in under an hour, while there is still time to save | My plant is dying and I don't know what's wrong | 14 | r/houseplants |

## App-criticism — apps that work but get tej'd → copy & improve (5 stubs)

| App | Tagline | Origin signal | Freq | Subreddits |
|---|---|---|---|---|
| [**Plate**](./Plate/spec.md) · [log](./Plate/product_log.md) | Point your camera at your food, and it logs itself. Calorie tracking without the search bar, the database, or the gram-b | As a MyFitnessPal user, logging food manually is tedious and prevents consistenc | 5 | MyFitnessPal |
| [**Prose**](./Prose/spec.md) · [log](./Prose/product_log.md) | Dating that starts with what you wrote, not how you look. Photos are blurred until you have exchanged real messages. You | As a Tinder user, I'm judged only on photos, not personality or values | 5 | Hinge |
| [**Slate**](./Slate/spec.md) · [log](./Slate/product_log.md) | The notes app that does one thing. No databases, no templates, no toggles, no AI. You write, you find it later, that's i | As a Notion user, the platform is overwhelming with features I don't need | 11 | Notion, ObsidianMD |
| [**Sync**](./Sync/spec.md) · [log](./Sync/product_log.md) | A dating app whose algorithm works for you, not against you. No artificial scarcity, no "boost to be seen," no shadow th | As a Tinder user, the algorithm frustrates me deliberately to push paid upgrades | 3 | Instagram, Tinder |
| [**Tier**](./Tier/spec.md) · [log](./Tier/product_log.md) | A dating app where the free version actually works. No paywalled likes, no hidden matches, no "upgrade to see who liked  | As a Tinder user, basic features are locked behind an expensive paywall | 3 | Hinge, Tinder |

## Utilitarian-emotional — daily-life pain charged with feeling (15 stubs)

| App | Tagline | Origin signal | Freq | Subreddits |
|---|---|---|---|---|
| [**Bare**](./Bare/spec.md) · [log](./Bare/product_log.md) | Three products. That's your routine. Bare cuts through the skincare noise and tells you the smallest possible thing that | I'm confused about the right skincare routine for me | 5 | r/SkincareAddiction |
| [**Cradle**](./Cradle/spec.md) · [log](./Cradle/product_log.md) | A health plan that respects the fact you just had a baby. Cradle is the postpartum coach that lowers the bar on purpose, | I had a baby and can't stick to being healthy, feeling trapped | 5 | r/Parenting, r/loseit |
| [**Crest**](./Crest/spec.md) · [log](./Crest/product_log.md) | The plateau isn't the end of the story. Crest is the coach that meets you on the flat part of the curve and shows you wh | I hit a weight loss plateau and feel hopeless about progress | 5 | r/loseit |
| [**Even**](./Even/spec.md) · [log](./Even/product_log.md) | The binge isn't the failure, the restriction is. Even tracks the loop you're actually in and helps you exit it from the  | I binge then restrict, hating myself in the cycle | 5 | r/loseit |
| [**Hold**](./Hold/spec.md) · [log](./Hold/product_log.md) | The people you love deserve to be remembered. Hold makes sure the birthday, anniversary, and follow-up doesn't slip past | I keep forgetting important dates and feel like a bad person | 4 | r/Parenting, r/personalfinance |
| [**Loop**](./Loop/spec.md) · [log](./Loop/product_log.md) | Seven meals. That's your week. Loop helps you find the small set of meals you actually cook and rotate them on repeat, g | I can't cook consistently and feel like I'm failing my family | 5 | r/Cooking, r/Parenting |
| [**Lull**](./Lull/spec.md) · [log](./Lull/product_log.md) | A bedtime routine that adapts to your kid, not the other way around. Lull learns what works in your house and stops you  | Bedtime with my kids exhausts me and ruins my evening | 5 | r/Parenting |
| [**Norm**](./Norm/spec.md) · [log](./Norm/product_log.md) | Is this a phase or a flag? Norm walks you through the behavior you're worried about and tells you, honestly, where it si | My child's behavior worries me but I don't know if it's normal | 5 | r/Parenting |
| [**Pare**](./Pare/spec.md) · [log](./Pare/product_log.md) | Decide once, donate the rest. Pare walks you through your closet item by item and makes the keep/donate call feel light  | I have too many clothes and can't decide what to keep | 5 | r/Frugal, r/declutter |
| [**Plain**](./Plain/spec.md) · [log](./Plain/product_log.md) | Eat like a normal person. Plain ignores the diet wars and gives you the simple eating rules your body actually needs. | I'm overwhelmed choosing between conflicting diet advice | 5 | r/Cooking, r/loseit |
| [**Range**](./Range/spec.md) · [log](./Range/product_log.md) | Your kid is probably fine. Range shows you the real normal range for their age and tells you, honestly, when interventio | My child is behind other kids and I'm terrified about their future | 5 | r/Parenting |
| [**Tally**](./Tally/spec.md) · [log](./Tally/product_log.md) | One number. That's the whole app. Tally tells you how much you've spent this month and stops there, because the categori | I should track my budget but all the apps are too complex | 5 | r/Frugal, r/personalfinance |
| [**Tether**](./Tether/spec.md) · [log](./Tether/product_log.md) | Five minutes of you, fully there, counts. Tether helps you stitch together the small presence moments that actually buil | I don't show up consistently for my child and feel guilty | 5 | r/Parenting |
| [**Truce**](./Truce/spec.md) · [log](./Truce/product_log.md) | Is this actually a deal? Truce checks any price against its real history before you buy, so the word "sale" stops being  | I can't tell if sales are real deals or marketing tricks | 5 | r/Frugal |
| [**Worth**](./Worth/spec.md) · [log](./Worth/product_log.md) | You don't owe a number on a scale your dating life. Worth is the coach that uncouples your value from your weight loss t | I'm waiting to date until I lose weight because appearance matters | 5 | r/loseit |

## Community trends — implicit patterns suggesting a missing tool (10 stubs)

| App | Tagline | Origin signal | Freq | Subreddits |
|---|---|---|---|---|
| [**Cast**](./Cast/spec.md) · [log](./Cast/product_log.md) | The man, woman, or person you actually want to be. Cast helps you pick the traits, drop the ones that aren't yours, and  | What should my gender role be in modern society | 4 | AskMen, NoStupidQuestions |
| [**Cue**](./Cue/spec.md) · [log](./Cue/product_log.md) | The conversation about sex you've been avoiding, broken into pieces small enough to actually have. Cue gives you and you | Sexual desire mismatches are straining relationships | 11 | r/AskMen, r/AskWomen, r/LifeProTips, r/Millennials, r/NoStup |
| [**Held**](./Held/spec.md) · [log](./Held/product_log.md) | Touch is a basic human need, and nobody talks about not getting any. Held finds the people near you who are missing it t | I'm struggling with lack of physical affection | 4 | AskWomen, NoStupidQuestions |
| [**Mirror**](./Mirror/spec.md) · [log](./Mirror/product_log.md) | The flaw you can't stop seeing isn't the one anyone else sees. Mirror catches the spiral, names what's happening, and ge | I'm constantly self-conscious about my appearance | 10 | AskMen, AskWomen, CasualConversation, LifeProTips, Millennia |
| [**Pulse**](./Pulse/spec.md) · [log](./Pulse/product_log.md) | The conversation about sex you and your partner keep almost having. Pulse opens it, gently, with both of you in the room | Sexual desire mismatches are straining relationships | 11 | AskMen, AskWomen, LifeProTips, Millennials, NoStupidQuestion |
| [**Tell**](./Tell/spec.md) · [log](./Tell/product_log.md) | The honest read on whether they like you back. Drop in what they did, what they said, how it felt, and Tell tells you wh | I need help reading if someone is romantically interested | 12 | AskMen, AskOldPeople, AskWomen, NoStupidQuestions |
| [**Tide**](./Tide/spec.md) · [log](./Tide/product_log.md) | Today's mood, explained by where you are in your cycle. Log a feeling, see the pattern, stop wondering why you feel like | I want to understand how my cycle affects my mood | 3 | AskMen, AskWomen |
| [**Tune**](./Tune/spec.md) · [log](./Tune/product_log.md) | The feeling under the feeling, named. Tune teaches you to read what's happening inside you before it leaks out everywher | I struggle to feel or regulate emotions | 12 | AskMen, AskWomen, CasualConversation, LifeProTips |
| [**Voice**](./Voice/spec.md) · [log](./Voice/product_log.md) | The exact words for the thing you can't bring yourself to say. Tell Voice what's wrong and who it's with, get a script t | I struggle to communicate boundaries and discomfort | 6 | AskMen, AskWomen, CasualConversation |
| [**Yore**](./Yore/spec.md) · [log](./Yore/product_log.md) | The inside jokes only your generation gets, in one feed. Yore remembers the things you forgot you remembered. | I want to laugh and share generational memories | 41 | GenZ, Millennials |

## Relational — structural patterns in how people struggle in love (10 stubs)

| App | Tagline | Origin signal | Freq | Subreddits |
|---|---|---|---|---|
| [**Anchor**](./Anchor/spec.md) · [log](./Anchor/product_log.md) | The app that catches the thought before the spiral. Tell Anchor what's looping in your head about your partner, and it w | I can't stop worrying my partner will leave or cheat | 20 | r/relationships |
| [**Compass**](./Compass/spec.md) · [log](./Compass/product_log.md) | The map between cold feet and real incompatibility. Compass tells you which differences are growth edges and which ones  | We have mismatched needs and I don't know if we can fix it | 14 | r/relationships |
| [**Ember**](./Ember/spec.md) · [log](./Ember/product_log.md) | Proof you still love each other, even when it doesn't feel like it. Ember catches the small moments your brain forgets a | The spark died after the honeymoon phase ended | 12 | r/relationships |
| [**Inlaw**](./Inlaw/spec.md) · [log](./Inlaw/product_log.md) | The family you didn't choose, navigated. Inlaw maps the politics, drafts the lines, and tracks the small wins that turn  | My partner's family situation means I always come second | 39 | r/relationships |
| [**Lean**](./Lean/spec.md) · [log](./Lean/product_log.md) | You know you push people away. You don't know how to stop in the moment. Lean catches the urge to bolt and asks one ques | I'm scared of getting hurt so I push people away | 20 | r/relationships |
| [**Ledger**](./Ledger/spec.md) · [log](./Ledger/product_log.md) | A private record of who's been carrying the relationship. Not to keep score, to stop pretending the scoring isn't alread | I'm always the one trying while my partner sits back | 11 | r/relationships |
| [**Mend**](./Mend/spec.md) · [log](./Mend/product_log.md) | The bridge back when you've gone quiet on each other. Mend gives you the first sentence after the silence, so you don't  | I don't know how to reconnect after we've drifted | 15 | r/relationships |
| [**Mull**](./Mull/spec.md) · [log](./Mull/product_log.md) | A place to think honestly about whether this is the right person. Not a decision tool, a thinking tool, for the question | I keep second-guessing whether this person is right for me | 16 | r/relationships |
| [**Orbit**](./Orbit/spec.md) · [log](./Orbit/product_log.md) | One person can't be your whole world, even if you want them to be. Orbit is the gentle pressure that keeps the rest of y | I feel excluded or isolated even in my relationship | 17 | r/relationships |
| [**Span**](./Span/spec.md) · [log](./Span/product_log.md) | The shape of the time between visits. Span turns the gap of being apart into something you're building together, not jus | I don't know how to handle long-distance or separation | 33 | r/relationships |

---

## Next moves

1. **Triage** — go through this list, dismiss obvious nos, star the ones that earn a closer look.
2. **Judges** — for the shortlist, run `benchmark-scanner` + `retention-validator` + `user-interview-simulator` from amon-ai. None of the stubs have been judged yet.
3. **Real spec-writer** — for survivors, invoke `/spec-writer` to take the stub from Phase 1 sketch → Phase 1 validated.
4. **Naming** — none of these names have been name-checked. Many will collide on App Store / trademarks.

_Generated by the pain-radar pipeline. Raw themes saved to `/tmp/radar/themes/`, raw posts to `/tmp/radar/raw/`._

---

## Judges verdicts (sorted best to worst)

_45 stubs judged. 🌐 = community-as-10x typology. Lower score = better._

| Rank | Score | App | Type | Benchmark | Retention | User interview |
|---|---|---|---|---|---|---|
| 1 | 3 | [**Loom**](./Loom/judgments.md) | 🌐 niche | 🟢 EMERGING | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 2 | 4 | [**Anchor**](./Anchor/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 3 | 4 | [**Beta**](./Beta/judgments.md) | 🌐 niche | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 4 | 4 | [**Cradle**](./Cradle/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 5 | 4 | [**Crest**](./Crest/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 6 | 4 | [**Crumb**](./Crumb/judgments.md) | 🌐 niche | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 7 | 4 | [**Even**](./Even/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 8 | 4 | [**Lex**](./Lex/judgments.md) | 🌐 niche | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 9 | 4 | [**Loop**](./Loop/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 10 | 4 | [**Lull**](./Lull/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 11 | 4 | [**Plate**](./Plate/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 12 | 4 | [**Slate**](./Slate/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 13 | 4 | [**Span**](./Span/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 14 | 4 | [**Tether**](./Tether/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 15 | 4 | [**Tide**](./Tide/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 16 | 4 | [**Tune**](./Tune/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 17 | 5 | [**Ledger**](./Ledger/judgments.md) |  | 🟢 EMERGING | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 18 | 5 | [**Mirror**](./Mirror/judgments.md) |  | 🟢 EMERGING | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 19 | 5 | [**Mull**](./Mull/judgments.md) |  | 🟢 EMERGING | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 20 | 5 | [**Truce**](./Truce/judgments.md) |  | 🟡 CROWDED_SPACE | 🟢 STRUCTURAL_RETURN | 🔴 BUILT_ON_SAND |
| 21 | 6 | [**Bare**](./Bare/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 22 | 6 | [**Cue**](./Cue/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 23 | 6 | [**Ember**](./Ember/judgments.md) |  | 🟢 EMERGING | 🟡 WEAK_RETURN | 🔴 BUILT_ON_SAND |
| 24 | 6 | [**Hold**](./Hold/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 25 | 6 | [**Inlaw**](./Inlaw/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 26 | 6 | [**Lean**](./Lean/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 27 | 6 | [**Mend**](./Mend/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 28 | 6 | [**Norm**](./Norm/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 29 | 6 | [**Orbit**](./Orbit/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 30 | 6 | [**Pare**](./Pare/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 31 | 6 | [**Plain**](./Plain/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 32 | 6 | [**Pulse**](./Pulse/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 33 | 6 | [**Range**](./Range/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 34 | 6 | [**Sprout**](./Sprout/judgments.md) | 🌐 niche | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 35 | 6 | [**Sync**](./Sync/judgments.md) |  | 🔴 GRAVEYARD | 🟢 STRUCTURAL_RETURN | 🔴 BUILT_ON_SAND |
| 36 | 6 | [**Tally**](./Tally/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 37 | 6 | [**Tell**](./Tell/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 38 | 6 | [**Tier**](./Tier/judgments.md) |  | 🔴 GRAVEYARD | 🟢 STRUCTURAL_RETURN | 🔴 BUILT_ON_SAND |
| 39 | 6 | [**Voice**](./Voice/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 40 | 6 | [**Worth**](./Worth/judgments.md) |  | 🟢 EMERGING | 🟡 WEAK_RETURN | 🔴 BUILT_ON_SAND |
| 41 | 6 | [**Yore**](./Yore/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🟡 WEAK_ON_ASSUMPTIONS |
| 42 | 7 | [**Cast**](./Cast/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🔴 BUILT_ON_SAND |
| 43 | 7 | [**Held**](./Held/judgments.md) |  | 🟡 CROWDED_SPACE | 🟡 WEAK_RETURN | 🔴 BUILT_ON_SAND |
| 44 | 8 | [**Compass**](./Compass/judgments.md) |  | 🟡 CROWDED_SPACE | 🔴 NO_RETURN | 🔴 BUILT_ON_SAND |
| 45 | 8 | [**Prose**](./Prose/judgments.md) |  | 🔴 GRAVEYARD | 🟡 WEAK_RETURN | 🔴 BUILT_ON_SAND |
