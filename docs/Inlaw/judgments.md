# Inlaw — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The broader "AI for relationship conflict / scripts / pattern logging" space is crowded with well-funded players (Lasting, Paired, BetterCouple, CoupleWork, Gottman Adviser, BestInterest for co-parenting). None of them specifically own the in-law wedge, but they all sell the same core promise: log dynamics, get scripts for hard conversations, see patterns over time. The in-law angle is a genuinely under-served niche inside this crowded category, but the wedge has to be sharp because users already have generic tools (and ChatGPT) drafting these lines today. The privacy risk flagged in product_log.md (a partner discovering the log) is the real moat-or-killer, not feature differentiation.

**Top competitors:**
- Paired — AI-personalized couples coaching with conflict tools and daily prompts; covers in-laws as a sub-topic (https://www.paired.com)
- Lasting (Talkspace) — clinical relationship app, Gottman-based modules including extended-family conflict (https://www.talkspace.com/blog/ai-couples-therapy/)
- BetterCouple — AI couples counseling explicitly pitches setting boundaries when family dynamics complicate the relationship (https://bettercouple.app/)
- CoupleWork — AI relationship coaching, real-time conflict scripts and pattern analysis (https://couplework.ai/)
- BestInterest — high-conflict co-parenting app with journal + AI message coaching, closest mechanic (log incidents, get calibrated lines), adjacent target (https://bestinterest.app/)

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Help me navigate a chronic, emotionally loaded relationship with my partner's family without it costing me my peace or my couple.
Classification: occasional (incidents and visits recur, but unpredictably, not daily)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong, the win log and pattern surfacing are explicitly designed to make the user feel they're slowly learning to handle a situation that previously felt static.
- Autonomie (sentiment d'être en contrôle): Strong, the whole product reframes a powerless dynamic into something the user can map, prepare for, and choose a line about, putting them back in the driver's seat.
- Lien social (sentiment d'être connecté à d'autres): Absent, the experience is entirely solo and private (privacy is even flagged as a risk in the log), no shared or community dimension.

**Boucle d'habitude**
- Déclencheur: an in-law incident just happened, or a visit/call is coming up, INTERNAL (the emotional residue of a slight, or the dread before a dinner, are real felt cues).
- Routine: log the incident in three sentences, or ask for a line before the next interaction.
- Récompense: relief from seeing the pattern named, or a concrete sentence to say tonight, immediate Y.
- Push reliance: low, the cues are internal (post-incident emotional charge, pre-visit dread), though calendar-linked push for upcoming visits could reinforce.

**Verdict line**
Two of three angles pass: psychological needs are strongly nourished on competence and autonomy, and the habit loop has plausible internal cues with immediate reward. The job itself is occasional, not naturally recurring, which is the weakness: between incidents and visits, there is no daily reason to open the app, and a stretch of family peace could lead to dormancy. Per protocol (2 of 3 angles needed for STRUCTURAL_RETURN, with psych needs counted as one combined angle: 1 passes here), this lands as WEAK_RETURN.

**What needs to change for STRUCTURAL_RETURN**
- Is there a lightweight daily or weekly touch (a partner check-in, a reflection prompt, a "how is the temperature this week") that gives the user a reason to open Inlaw between incidents?
- Could the win log become a periodic ritual (monthly recap, anniversary of a hard moment now handled) that converts an occasional job into a recurring one?
- Is there a way to introduce a relatedness dimension (anonymous shared patterns from other users, "others in your situation also logged this") without breaking the privacy constraint the product log already flagged?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

The problem is sharp and the persona constructs cleanly (Sarah, 32, partnered 5 years with a tight-knit MIL). The product hangs together as a concept: map, log, line, wins. But three load-bearing assumptions are unvalidated: (1) people will keep logging emotionally charged incidents about named family members over weeks, (2) AI-drafted "lines" will feel calibrated rather than generic-therapy-speak, (3) the privacy model is safe enough that a partner discovering the app isn't relationship-ending. The spec acknowledges #3 in the log but ships no answer. Positioning is credible, execution risk is high.

**Dangerous assumptions:**
- Users will keep logging incidents week after week. Logging an in-law slight requires re-entering the bad feeling on a calm evening, which is exactly when people want to forget it. H1 targets 35% at 5+ incidents by week 6, but nothing in the spec creates pull to log when nothing acute just happened. Cheap test: 2-week diary study with 10 target users using a Notes app template, measure unprompted log rate.
- The drafted 'lines' will feel specific and usable, not like ChatGPT therapy-speak the user would be embarrassed to deliver. The spec promises calibration to 'the specific person and specific trigger' but offers no mechanism for how 4 logged incidents become a line that sounds like the user. Cheap test: hand-write 5 lines for 5 real Reddit cases, show to target users, measure 'would actually say this' rate.
- The privacy model survives a partner discovering the app. Logging 'your mother was rude on Sunday' under named family members is relationship-nuclear material. The product_log flags this as TBD with no design. If the first viral story is 'Inlaw broke us up', the product dies. Cheap test: 5 user interviews asking 'where would you store private notes about your MIL, and what happens if your partner finds them?' before designing storage.
