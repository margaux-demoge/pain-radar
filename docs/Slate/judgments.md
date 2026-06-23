# Slate — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The "minimalist markdown notes app, local files, one-time purchase, anti-Notion" positioning is one of the most saturated indie software categories in 2026. Bear, iA Writer, Apple Notes, Obsidian, and a fresh wave of paid local-first apps (Glyph, Nota, Octarine, NotesHub) all occupy the exact territory Slate is aiming at, several with Apple Design Awards and years of distribution. Simplenote's July 2025 shutdown confirms demand exists but also that radically minimal notes apps struggle to monetize, and the "Notion refugee" wave has largely been absorbed by Apple Notes and Bear by default. Slate has no surfaced wedge beyond "even more minimal," which every competitor here already claims.

**Top competitors:**
- Bear — markdown-first, Apple Design Award, hashtag organization, the default paid Mac minimalist notes app
- iA Writer — one-time purchase per platform, plain text files, the gold standard for distraction-free writing
- Apple Notes — free default on every Apple device, zero setup, the actual destination most Notion refugees end up at
- Obsidian — local markdown files in a folder, free for personal use, dominant among the own-your-notes crowd
- Glyph / Nota / Octarine — new wave of one-time-purchase local-first markdown macOS apps, near-identical pitch to Slate

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Capturer une pensée tout de suite et la retrouver plus tard, sans avoir à concevoir un système pour la ranger.
Classification: naturally recurring (les pensées à noter surgissent quotidiennement, plusieurs fois par jour, indépendamment de l'app)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Absent. Pas de progression, pas de skill tree, pas de feedback de maîtrise. L'app refuse explicitement les hooks d'engagement.
- Autonomie (sentiment d'être en contrôle): Strong. Le pitch entier tourne autour du contrôle: fichiers .md sur disque, pas de serveur, pas de lock-in, possession à vie, l'utilisateur décide où vivent ses notes.
- Lien social (sentiment d'être connecté à d'autres): Absent. Solo writing only, pas de collaboration, pas de partage, revendiqué.

**Boucle d'habitude**
- Déclencheur: une pensée surgit dans la journée que l'utilisateur veut capturer, ou un besoin de retrouver une note. INTERNAL.
- Routine: ouvrir l'app (curseur déjà dans une nouvelle note), taper, escape. Ou swipe down et taper deux mots pour retrouver.
- Récompense: la pensée est sortie de la tête et stockée, ou retrouvée en 5 secondes. Immediate Y.
- Push reliance: aucune dépendance au push, l'app revendique l'absence totale de hooks. C'est cohérent avec H3.

**Verdict line**
Deux des trois angles passent clairement: le besoin "capturer une pensée" recourt naturellement et plusieurs fois par jour, et la boucle d'habitude repose sur un déclencheur interne (la pensée elle-même) avec une récompense immédiate (la pensée est sortie ou retrouvée). Le pilier psychologique est faible (seule l'autonomie est forte, compétence et lien social sont assumés absents), mais c'est un choix produit explicite, pas un oubli. La vraie fragilité n'est pas la rétention structurelle mais la différenciation contre Apple Notes/Bear, ce qui relève de H1 et du product_log, pas de ce judge.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Simulated user: Julien, 34, Lyon, product manager. Burned by Notion (abandoned workspace with 12 broken databases), tried Obsidian for 3 weeks, now defaults to Apple Notes on iPhone + a Google Doc called "brain dump." Mildly skeptical, has heard the "minimal notes app" pitch from Bear, IA Writer, Simplenote, Craft, Tana-lite. Not hostile, but his wallet is closed by default.

Interview:

Q1, "Apple Notes est déjà ouvert sur mon téléphone, gratuit, synchro iCloud, recherche full-text. Pourquoi je paierais 30 balles pour faire la même chose?"
> PARTIAL. Spec says .md files on disk + "owned forever", but never articulates a concrete wedge over Apple Notes beyond philosophy.

Q2, "Bear existe depuis 2016, fait exactement ça, markdown + recherche. Qu'est-ce que Slate fait que Bear ne fait pas?"
> UNANSWERED. Spec never names or differentiates from Bear, iA Writer, Simplenote, Drafts.

Q3, "J'ai churné de Notion il y a 6 mois et je suis revenu à Apple Notes. Pourquoi je changerais encore? J'ai déjà ma solution."
> UNANSWERED. Spec assumes Notion refugees are still in pain, not that they've already settled.

Q4, "Vous dites 'la première ligne devient le titre'. Et si je veux renommer? Si je commence par 'todo' et que c'est en fait une idée de roman?"
> PARTIAL. Spec implies title is locked to first line; no edit story addressed.

Q5, "Recherche full-text, ok, mais j'ai 800 notes dans Apple Notes et je trouve jamais ce que je cherche parce que je me souviens pas des mots exacts. En quoi votre recherche règle ça?"
> UNANSWERED. Spec says "if you can't find it by typing two words, it wasn't important", which is a dodge, not an answer.

Q6, "Vous vendez 'pas d'IA'. Mais moi l'IA dans Notion c'est la seule chose que j'utilise vraiment. C'est un feature, pas un bug. Pourquoi me priver?"
> UNANSWERED. Spec treats no-AI as virtue, doesn't validate that the target actually rejects AI.

Q7, "Sync. Je suis sur Mac + iPhone + iPad. Ic loud c'est cassé une fois par mois. Comment vous gérez les conflits quand j'édite la même note sur deux appareils?"
> UNANSWERED. Spec waves at "iCloud or a folder", no conflict story, no multi-device promise.

Q8, "Paiement one-shot 20-40 euros. Et dans 2 ans quand iOS 22 sort et que l'app crash? Vous mettez à jour gratos pendant combien de temps?"
> UNANSWERED. Spec says "the app is finished" but doesn't address OS-update maintenance economics.

Q9, "Vous dites 'pas de serveur'. Donc pas de partage de note par lien, pas de version web pour dépanner du poste d'un client. C'est un dealbreaker pour moi, vous avez pensé à combien de gens comme moi?"
> UNANSWERED. Spec excludes sharing/web by design without sizing the cost.

Q10, "Honnêtement, le 'manifeste anti-Notion' j'en ai vu cinq sur Product Hunt cette année. Tous morts. Qu'est-ce qui fait que vous, vous tenez 18 mois?"
> UNANSWERED. Spec has no distribution story, no defensibility story, no answer to category graveyard.

Score: 0/10 answered, 2/10 partial, 8/10 unanswered.

Positioning is philosophically coherent but commercially naive. The spec confuses "we know what we won't build" with "we know why someone pays." Three competitors (Apple Notes free, Bear paid, iA Writer paid) already occupy this exact slot, and the spec never names them. The "Notion refugee" persona is a Reddit artifact, not a validated paying segment. Open questions in product_log already flag the two biggest holes (Apple Notes/Bear wedge, willingness to pay) but the spec hasn't answered them.

**Dangerous assumptions:**
- Notion refugees will pay $20-40 upfront for a minimal notes app rather than default to free Apple Notes. Why dangerous: the entire revenue model rests on this, and the spec offers no evidence the refugee segment converts to paid alternatives instead of just downgrading to the default. Cheap test: landing page with Stripe pre-order at $29, drive 500 visitors from r/Notion churn threads, measure conversion before writing code.
- The wedge against Bear/iA Writer/Simplenote is meaningful enough to switch. Why dangerous: these apps already deliver 'minimal markdown notes' and have years of polish; if Slate's only differentiator is philosophy, switching cost beats it. Cheap test: 10 user interviews with current Bear/iA Writer paying users asking what would make them switch, look for a concrete missing capability not a vibe.
- Users actually want 'no AI, no sync drama, no sharing' rather than tolerating them. Why dangerous: the spec treats absence-of-features as the product, but the loudest churned-Notion users on Reddit often still want AI search and cross-device sync, just without the database overhead. Cheap test: post the Slate manifesto on r/Notion and r/ObsidianMD, measure ratio of 'shut up and take my money' to 'but I need X'.
