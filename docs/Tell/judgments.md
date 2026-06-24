# Tell — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "decode their texts / are they into me" space is densely populated as of 2025-2026, with multiple active AI products (ReadHim, Lucen, Chat Analyzer by MWM, SituationshipAI, ChatVisor tools) all promising the same core read: paste evidence, get an honest signal score. Crushh (2017-2019) and Mei (2018-) are the foundational failed attempts, both killed not by demand but by Play Store data-access policy — a relevant scar for any product wanting deeper integration. The recurring failure pattern is twofold: (1) platform / data-access restrictions when apps try to integrate with messaging, and (2) the validation-vs-truth tension users repeatedly flag in reviews. Tell's wedge ("holds the thread across days, refuses to prescribe moves") is real but narrow; the team needs to articulate why the over-analyzer chooses Tell over Lucen or ReadHim, which already brand on the same honesty promise.

**Top competitors:**
- ReadHim — paste texts, get a 0-100 green/red flag score, explicit 'decode his messages' positioning (readhim.app)
- Lucen — AI chat analyzer + dating coach, breaks down mixed signals, response patterns, red flags (lucen.app)
- Chat Analyzer: Recap & Insight (MWM) — decodes WhatsApp/IG/iMessage with romance index, interest level, red flag detection
- SituationshipAI — paste-and-analyze tool targeting exactly the ambiguous-stage user Tell is going after
- ChatVisor Dating Text Analyzer / Love Signs Detector — multiple tools under one brand for 'does he/she like me' decoding

## retention-validator: `WEAK_RETURN`

The job (decode one specific ambiguous romantic situation) is occasional, not naturally recurring: it lasts as long as the situation lasts, then resolves. SDT is thin: competence is absent (the user does not get better at anything, Tell does the reading), autonomy is weak (you describe, it interprets), social connection is deliberately absent (private, nothing shared). Habit loop has a strong internal cue (the 2am rumination spike) and immediate emotional reward (relief from uncertainty), which is the one angle that genuinely passes; but once the situation resolves, no structural reason brings the user back for the next crush. Verdict: WEAK_RETURN — the habit loop angle passes, the other two do not.

Le job que l'app fait pour l'user: donner un avis calme et structuré sur "est-ce que cette personne s'intéresse vraiment à moi", quand le user tourne en boucle sur une situation ambiguë. Classification: occasional (recurs per crush, not on a predictable cadence; one situation can last weeks then end). 

Besoins psychologiques: Compétence Absent — le user ne progresse pas, l'app lit à sa place et il n'y a pas de skill tree / sense of mastery. Autonomie Weak — le user contrôle ce qu'il raconte mais pas la lecture, et l'app refuse explicitement de lui rendre l'agency sur le "next move". Lien social Absent — design choice assumé, rien n'est partagé, c'est l'inverse du group chat qu'elle remplace.

Boucle d'habitude: Déclencheur = moment de rumination (nouveau texto, replay d'une soirée, scroll 2am), INTERNAL et fort. Routine = paste/type/talk ce qui s'est passé. Récompense = soulagement immédiat de l'incertitude + lecture structurée, immediate Y. Push reliance: pas mentionné, la boucle repose sur le trigger interne, ce qui est sain mais ne couvre que la durée de la situation.

H1 (40% adding evidence across 3+ days) tente justement de forcer la récurrence intra-situation, mais ne résout pas la question post-résolution déjà soulevée dans le product_log ("does the user return for the next one, or churn permanently?").

Pour passer STRUCTURAL_RETURN: (1) Y a-t-il une raison de revenir une fois la situation résolue — pattern recognition à travers plusieurs situations, journal des reads passés qui éclaire les nouvelles? (2) Le user peut-il développer une forme de compétence — apprendre à mieux lire les signaux lui-même au fil du temps, plutôt que rester dépendant de l'app? (3) Le besoin d'analyser quelqu'un est-il vraiment occasional pour la cible "over-analyzer", ou y a-t-il toujours quelqu'un dans la tête — auquel cas la récurrence est naturelle et il faut juste le nommer?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

The persona is clear and the wedge (over-analyzer 18-30) is sharp, and the product experience answers the basic "what is this" question with a distinctive promise (read, not prescription). But the spec leans heavily on unvalidated bets: that users want truth over validation, that an LLM read feels more trustworthy than friends who know the people involved, and that "no next-move advice" is a feature rather than a missing half. Three of the questions a real skeptic would ask are unanswered, and at least two map directly to the open questions already flagged in product_log.md — meaning the team knows the risk but has not tested it.

**Dangerous assumptions:**
- Users want an honest read more than they want validation. If the wedge persona (the over-analyzer) churns the moment Tell says 'not consistent with romantic interest', H3's 60% resolution target collapses and the product becomes a sad-mirror people uninstall. Cheap test: run 20 paid interviews where a stand-in 'reader' delivers a deliberately unflattering read on a real situation, measure whether the user comes back the next day with new evidence or ghosts.
- An AI with zero knowledge of the other person can produce a read that feels sharper than a friend who has met them. Friends bring priors Tell cannot access (tone of voice, history, body language IRL). If the read feels generic-horoscope to over-analyzers (who are pattern-sensitive by definition), H2's 50% 'primary debrief place' target is fantasy. Cheap test: Wizard-of-Oz 10 situations with a human writing the structured read, A/B against ChatGPT with the same prompt, ask users which felt more useful and why.
- The loop is multi-day, not one-shot. The whole pricing/retention model implied by H1 (40% adding evidence across 3+ days) assumes users return unprompted to a private journaling-style app during an emotionally charged period. Most people either resolve the ambiguity in their head within 48h or push it down. Cheap test: ship a minimal landing + waitlist with a 'check back tomorrow' email flow on a fake situation, measure D2/D3 return rate on the email before building anything.
