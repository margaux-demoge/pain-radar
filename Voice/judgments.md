# Voice — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "AI helps you write a hard message to someone in your life" space is dense with 2025-2026 entrants. At least 5 active apps (Pancake, Mei/TextMei, Ember, Jenova, DivorceX/MessageX) plus Lucen and the workplace-conversation roleplay cluster (Yoodli, CAISY, Lio, Tough Tongue, VirtualSpeech) are shipping variants of this. Voice's wedge (multiple postures + delivery channel guidance + relationship memory) overlaps with what Pancake and Ember already advertise. There is also one notable platform shrinkage signal (Mei pulled its iOS relationship app in April 2026) suggesting the consumer relationship-texting angle is harder to retain than the B2B coaching angle.

**Top competitors:**
- Pancake (AI Relationship Coach, iOS) — paste a text, get tone/intent read and suggested reply, exactly Voice's job for couples
- Ember: AI Relationship Coach (iOS) — text analyzer + communication-pattern coaching, overlaps with Voice's 'learn the relationships' promise
- Mei / TextMei — long-running messaging-AI coach, screenshot in, suggested reply out; iOS variant pulled April 2026, Android still live
- Jenova AI Relationship Advisor — explicitly markets drafting messages, anticipating responses, preparing for multiple outcomes (same loop as Voice)
- DivorceX MessageX — calm/neutral reply drafting for high-conflict relationships, adjacent but same core mechanic

## retention-validator: `WEAK_RETURN`

**Le job que l'app fait pour l'user**
Help me find the exact words for a hard conversation I've been avoiding, so I can actually say it.
Classification: occasional. Difficult conversations recur, but unpredictably, clustered around relational friction. Not a daily ritual, not a one-shot either.

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. The app helps the user succeed in one conversation, but there is no visible skill progression, no streak, no "you are getting better at this" arc. H2 (outcome logging) hints at a feedback loop but it is not designed as mastery.
- Autonomie (sentiment d'être en contrôle): Strong. Multiple posture variants, editable scripts, user picks tone and delivery mode, private room with nothing shared. Control is the core UX.
- Lien social (sentiment d'être connecté à d'autres): Absent. Explicitly private, nothing shared, nothing posted. The relationship being helped is outside the app.

**Boucle d'habitude**
- Déclencheur: "something sitting on your chest", a real-life conflict or unsaid thing. INTERNAL, and a strong one when it fires.
- Routine: tell Voice the who/what/feel/want, get 3-4 versions, tune one, get a delivery plan.
- Récompense: words you would actually say + a small plan + reduced dread. Immediate Y.
- Push reliance: Low. The cue is internal (emotional discomfort) and does not depend on notifications. That is a strength, but the cue fires only when conflict arises.

**Verdict line**
One angle clearly passes: the habit loop has a strong internal cue (something on your chest) and an immediate reward (the words, the plan). Autonomy is Strong but competence and relatedness are weak/absent, so the SDT angle does not pass (needs 2 of 3 Strong). The job is occasional, not naturally recurring, so the recurrence angle fails. Result: WEAK_RETURN. Voice will be opened in moments of real need, which is honest, but between those moments there is no structural pull, and H3's 3+ scripts/month assumes conflicts arrive often enough to sustain weekly use.

**What needs to change for STRUCTURAL_RETURN**
- Is there a second job Voice can credibly do between conflicts (everyday "small things to say", thank-yous, check-ins, repair messages) that uses the same engine but fires more often?
- Can the "relationships Voice learns over time" become a visible mastery surface (a sense that scripts for mom/partner/best friend get sharper each round) so the user feels they are building something, not just consuming outputs?
- Should the outcome-note loop (H2) be reframed as a personal practice the user returns to, rather than a one-off report, so the rehearsal space becomes a reflective space too?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Simulated user: Léa, 29, Lyon, marketing manager, conflict-averse, drafts hard texts 4-5 times in Notes app, sometimes asks ChatGPT to "make this sound less aggressive," talks things out with her best friend on WhatsApp. Skeptical that an app knows her voice better than her best friend does. Spec nails the pain articulation and the moment of use, but leaves three big assumptions unvalidated: (1) that AI-generated scripts will sound like her and not like a HR-sanitized LinkedIn post, (2) that she'll open a dedicated app instead of pasting into ChatGPT which she already trusts, (3) that she'll come back to log outcomes (H2 at 35% feels invented, and the log itself flags this risk). Q1-Q5 are decently answered by the spec's "3-4 postures + tuning + learns relationships" promise; Q6-Q10 expose the moat, voice-fidelity, and retention loop. The positioning is sharp and the wedge is real, but the differentiator vs ChatGPT and the come-back-to-log loop are pure assertion.

**Dangerous assumptions:**
- Voice can produce scripts that sound like the user (not generically AI-polished) within the first session — if the four postures all read like ChatGPT defaults, the user pastes once and never returns. Cheap test: hand-write 20 scripts in 4 postures from real Reddit situations, show them blind next to ChatGPT outputs to 10 target users, measure 'sounds like something I'd say' rate. The product_log already names this as the central UX problem.
- Users will return to log the outcome after delivering the script (H2 = 35%). Once they have the words, the job is done; the loop that powers 'Voice learns your relationships' breaks. Cheap test: run a 2-week Wizard-of-Oz with 15 users over iMessage, measure unprompted return rate after a script is sent. If <15% come back, H2 and the personalization moat both collapse.
- Voice is worth opening instead of ChatGPT/Claude, which target users already use for exactly this. The spec never names the competitor or the wedge beyond 'four postures + delivery channel advice.' Cheap test: show 10 users the Voice flow and the ChatGPT 'help me phrase this' flow side by side, ask which they'd use next time and why. If the answer is 'ChatGPT is already open,' the app needs a sharper wedge (relationship memory, voice capture, rehearsal mode) surfaced in onboarding.
