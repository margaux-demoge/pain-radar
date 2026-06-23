# Tally — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The post-Mint vacuum has been actively contested since 2024 by Copilot, Monarch, Simplifi, Rocket Money, PocketGuard, Cleo, Emma, plus a long tail of minimalist apps (Bobby, Simple Budget, Budget Calendar, Koody, Easlo's template). The "one number, no categories" angle is genuinely thinner than the rest of the space, but PocketGuard's "In My Pocket" number and Cleo's chat-first nudge already occupy that exact emotional job (anxiety relief, not optimization). The graveyard is small in the strict minimalist niche (mostly indie shutdowns, not indexed), so the dominant risk is differentiation against well-funded incumbents, not a hidden failure pattern.

**Top competitors:**
- PocketGuard — 'In My Pocket' is literally one safe-to-spend number after bills/goals, closest direct analog, active and well funded (https://pocketguard.com)
- Copilot Money — premium minimalist UX with a 'Month in Review' single-glance spend snapshot, Plaid-based, growing fast post-Mint (https://copilot.money)
- Cleo — chat-first, anxiety/affect angle ('roast mode'), explicitly competes for the 'I don't want to budget, just tell me' user (https://meetcleo.com)
- Emma — open-banking aggregator with a clean spend overview, EU-strong, active (https://emma-app.com)
- Rocket Money (ex-Truebill) — surfaces spend and subscriptions in a simplified dashboard, mass-market post-Mint winner (https://rocketmoney.com)

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Soulager l'anxiété de fin de mois en répondant en trois secondes à "est-ce que je suis okay financièrement ce mois-ci?".
Classification: naturally recurring (l'anxiété budgétaire revient quasi quotidiennement, et le cycle salaire/dépense est mensuel et structurel).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. Il y a un signal "tracking vs running hot" qui peut donner un sentiment de contrôle, mais aucun système de progression, pas de streak, pas de milestone. La baisse de spend M2 vs M1 (H2) est un effet espéré, pas une mécanique ressentie.
- Autonomie (sentiment d'être en contrôle): Weak. L'app affirme l'autonomie par la sobriété (pas de catégories imposées, pas de notifs), mais l'user ne configure rien, ne choisit rien. Autonomie passive plutôt qu'active.
- Lien social (sentiment d'être connecté à d'autres): Absent. Aucune dimension sociale, aucun partage, aucune comparaison à des pairs.

**Boucle d'habitude**
- Déclencheur: anxiété/curiosité ponctuelle sur "où j'en suis ce mois-ci", typiquement avant un achat ou en fin de journée. INTERNAL (potentiellement), mais non explicitement designé. Le seul cue externe assumé est le résumé email/push du dimanche, optionnel.
- Routine: ouvrir l'app, lire un chiffre. Friction quasi nulle (3 secondes), c'est le point fort.
- Récompense: information immédiate + soulagement (ou alerte douce "running hot"). Immediate Y, mais la récompense est faible quand le chiffre est "normal" — pas de variabilité, pas de surprise, pas de progression visible.
- Push reliance: faible par design (seulement un résumé hebdo opt-out). C'est cohérent avec la thèse anti-noise mais retire un cue externe de rappel, ce qui fragilise la boucle quand le cue interne n'est pas encore installé.

**Verdict line**
Un seul des trois angles passe nettement: la récurrence naturelle du besoin (regarder son solde mensuel est intrinsèquement récurrent). Les besoins psychologiques sont quasi tous faibles ou absents (zéro lien social, compétence et autonomie faibles), et la boucle d'habitude repose sur un cue interne qui n'est pas explicitement construit, avec une récompense plate quand tout va bien. Tally peut survivre comme utility consultée par à-coups, mais sans mécanique de progression ni cue installé, la fréquence d'ouverture risque de chuter une fois la curiosité initiale passée — ce qui rend la cible H1 "50% weekly à W12" ambitieuse.

**What needs to change for STRUCTURAL_RETURN**
- Quel est le cue interne précis que l'app veut installer (avant un achat? le matin? après un paiement détecté?) et comment le spec le rend explicite sans tomber dans la notification?
- Comment la récompense devient-elle ressentie quand "tout va bien" — y a-t-il une micro-variation, une comparaison à soi-même, un signal de progression d'un mois à l'autre qui crée un sentiment de compétence sans réintroduire de la complexité?
- Le besoin d'anxiété est-il vraiment quotidien, ou hebdomadaire/pré-paie? Si hebdo, est-ce que viser une ouverture quotidienne est même le bon objectif, ou faut-il assumer un rythme plus lent et ajuster H1?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Tally has a sharp, opinionated positioning ("one number, that's it") and a clearly defined disaffected-ex-budgeter persona, which is rare and a real strength. But the spec leans entirely on a single behavioral bet — that seeing one number daily reduces both anxiety AND spending — without addressing the two operational landmines: bank-connection trust (Plaid friction/cost, the same friction that kills Mint-successors), and willingness to pay $X/month for a screen with one number when free bank apps already show a running balance. The "no categories" thesis is asserted, not validated, and is exactly the kind of claim users endorse in interviews then defect from on day 7.

**Dangerous assumptions:**
- Users who say they want 'just one number' will actually stay engaged past week 2 without asking for categories, trends, or context — the product log itself flags this doubt and there is no validation plan.
- Users will pay 15% conversion for an app whose entire UI is a number their bank's own app already displays for free — the differentiation (calm, no-noise) may not clear the pricing bar, especially given Plaid unit economics force a paid tier.
- Connecting a bank account in 'two taps' to a brand-new indie app is the single biggest drop-off in this category; the spec treats it as solved infrastructure when it is the actual product risk.
