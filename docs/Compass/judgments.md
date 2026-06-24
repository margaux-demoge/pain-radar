# Compass — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "should I stay or go / are these differences dealbreakers" problem is densely served by three overlapping categories: clinical premarital assessments (Prepare/Enrich, SYMBIS) with millions of users and decades of research, modern couples apps (Paired, Lasting, Connected) running values-alignment modules, and newer decision-clarity tools (Hemelion, Commitment Clarity Map, Stay or Go group) targeting the exact ambiguity Compass names. Failed couples-app graveyard exists (Tuned, The Official App, Cobble) but those died on shared-utility/social angles, not on the values-mismatch use case, so they are weak precedents rather than warnings. The wedge has to be sharp: Compass's only real differentiator versus Hemelion + Prepare/Enrich is the "guess your partner first, then surface only the conflict points" mechanic, and that needs defending.

**Top competitors:**
- Hemelion, $9.90 one-shot decision engine that analyzes compatibility, values and fears to tell you if the relationship has a future, active https://www.hemelion.com/
- Prepare/Enrich, 20-area couple assessment, 31% divorce risk reduction claim, facilitator-led but with self-serve Catholic Couple Checkup, dominant incumbent https://www.prepare-enrich.com/
- SYMBIS, 1M+ couples premarital assessment covering 10 core areas including values/spirituality/money, active https://www.symbis.com/
- Lasting, Gottman-method structured sessions, 3M+ users, $29.99/mo, covers values/conflict/finances https://www.choosingtherapy.com/lasting-app-review/
- Paired, daily independent-answer questions with reveal mechanic (closest to Compass's 'guess your partner' move), 128 question packs https://www.thequalityedit.com/articles/paired-app-review

## retention-validator: `NO_RETURN`

VERDICT: NO_RETURN

**Le job que l'app fait pour l'user**
Help me decide whether the real differences with my partner are dealbreakers or workable, so I can stop oscillating and act.
Classification: one-shot (the decision resolves once: stay or leave; once clarity is reached, the job is done)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. There is a one-time exercise with output, but no visible mastery curve, no repeatable skill being built.
- Autonomie (sentiment d'être en contrôle): Strong. The whole product is built around private, judgment-free clarity, the user names their own non-negotiables, the app explicitly gets out of the way.
- Lien social (sentiment d'être connecté à d'autres): Weak. A joint partner version exists but it is a single optional artifact exchange, not an ongoing social fabric, and the spec frames it as risky.

**Boucle d'habitude**
- Déclencheur: a moment of doubt about the relationship, anchored to a pre-major-step life event (move, kids, engagement). INTERNAL but rare, not daily or weekly.
- Routine: a 30-minute deliberately uncomfortable solo exercise, plus optional re-checking "over weeks" to see if the picture changes.
- Récompense: a short list of real conflicts to discuss; emotional clarity. Immediate Y, but consumed in one sitting.
- Push reliance: spec does not lean on push, but there is also no described mechanism to bring the user back at all once the exercise is done.

**Verdict line**
The underlying job is fundamentally one-shot: users come for a stay/go decision, and the spec itself acknowledges in product_log open question #2 that once clarity is reached, churn is the natural outcome. Only autonomy scores Strong among the three psychological needs, and the habit loop has no recurring cue, the trigger fires once per relationship crisis, not on a rhythm. None of the three retention angles passes.

There is no structural reason for users to come back. Either the team accepts a churn product (and prices/positions accordingly, e.g. one-time purchase, referral-driven), or the spec needs to rethink either the job or the habit loop.

**What needs to change for STRUCTURAL_RETURN**
- Is there a recurring job adjacent to the one-shot decision, for example a weekly "check the map" ritual where the non-negotiables and the partner-guess get re-tested as the relationship evolves, that would make the cue recur naturally?
- Could competence be built explicitly, for example a visible track of how the user's own non-negotiables shift over months, turning a one-shot diagnostic into a longitudinal self-knowledge practice?
- Is there a way to make the joint/partner dimension an ongoing shared surface rather than a single risky reveal, so that lien social becomes a structural pull rather than a one-time event?

## user-interview-simulator: `BUILT_ON_SAND`

Compass asks users at the most fragile moment of a relationship to do 30 minutes of deliberately uncomfortable solo work, then trust an app's output enough to drive a stay-or-go decision. The spec is poetic but evades every hard question: why an app over a therapist or a Notion doc, how the joint mode avoids weaponization, what stops one partner from gaming their answers, and what retention looks like when the product's success means the user is done. Persona Léa, 31, Lyon, 4 years with her partner, currently journaling and seeing a therapist occasionally, would push back on most of the value chain. Three of the top dangerous assumptions sit unanswered, including the safety model for the joint version which the team's own product_log flags.

**Dangerous assumptions:**
- Users will trust an app's output enough to inform a stay-or-go decision over their own gut, friends, or a therapist. Spec asserts this but offers no trust mechanism (no methodology citation, no credentialed framing, no track record). Cheap test: show the value prop + sample output to 10 target users and ask 'would you act on this?'
- The joint version doesn't become ammunition. Spec waves this away with 'no judgment on who's right' but provides zero safety design (no facilitation, no framing of results, no guardrails if one partner is coercive or already-decided). Product_log Q3 admits this is open. Cheap test: run the joint exercise manually with 3 real couples on paper and observe the post-conversation.
- Users will actually complete 30 minutes of deliberately uncomfortable solo work at the exact moment their relationship feels fragile. Spec treats friction as a feature but never validates that the target user picks discomfort over avoidance. Cheap test: landing page with 'start 30-min uncomfortable exercise' CTA, measure click-to-start-to-finish on 100 visitors.
