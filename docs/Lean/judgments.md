# Lean — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The attachment-style app space has consolidated quickly around well-funded, content-heavy players (Attached/Eden, Personal Development School/Thais Gibson, Paired, Lasting) plus general urge-surfing tools (Pallie, Ahead). None target the exact eight-second moment-of-bolt for avoidants with a one-question pattern-interrupt, but they all claim the same outcome (heal avoidant attachment, stop self-sabotage). Lean's wedge has to be the in-the-moment intervention loop and the "smallest counter-move" mechanic, because the educational and journaling territory is fully owned. No clear graveyard surfaced, the failures here are not yet indexed, which is itself a signal that retention in this category is hard but companies stay alive on subscription revenue.

**Top competitors:**
- Attached (attachedapp.com) — AI coach Eden, daily exercises, journaling and meditations for anxious/avoidant/disorganized; the closest direct competitor in branding and target user. https://www.attachedapp.com/
- Personal Development School / PDS app (Thais Gibson) — 90-Day Attachment Bootcamp, 55+ courses, dominant authority voice in the avoidant audience. https://university.personaldevelopmentschool.com/
- Pallie — explicit urge-surfing scripts and no-contact tracker for relationship impulses; same eight-second-pause mechanic but framed around exes. https://relationship.pallie.ai/
- Ahead — emotion regulation app with heartbreak/borderline urge-surfing content, owns the impulse-control framing. https://ahead-app.com/
- Paired — daily couples prompts including self-sabotage content, mainstream distribution, expert-panel content. https://www.paired.com/
- Lasting — self-guided couples counseling app, large install base, overlapping pattern-change positioning. https://apps.apple.com/us/app/lasting-marriage-couples/id1225049619
- Sentari / urge-surfing tools — mindfulness apps explicitly marketing the wave-ride technique Lean's mechanic depends on. https://withsentari.com/urge-surfing-emotional-wave/

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Intercepter l'impulsion de fuir une relation au moment exact où elle survient, et la transformer en un petit geste de présence.
Classification: occasional (the urge recurs, but unpredictably; it depends on having an active relationship and on triggering events that may go days or weeks between occurrences).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong. Lean explicitly "keeps the receipts" of wins, banks small counter-moves, and makes pattern shift legible over weeks. This is mastery over a deeply ingrained pattern.
- Autonomie (sentiment d'être en contrôle): Strong. The framing is "co-conspirator, not therapist"; the user sets up their own patterns, Lean asks (not prescribes), and offers a single small move the user chooses to take. Reclaiming control over the eight seconds is the whole point.
- Lien social (sentiment d'être connecté à d'autres): Absent. The product is entirely solo. No shared feed, no peer support, no partner-facing surface. The relationship being protected is offline.

**Boucle d'habitude**
- Déclencheur: the felt urge to bolt (emotional text received, partner gets serious, conflict spike), INTERNAL. This is a strong internal cue rooted in body sensation and relational context, exactly the kind that survives notifications-off.
- Routine: open Lean, tag the trigger, answer one question, see one small counter-move.
- Récompense: immediate Y. The slowing of the eight seconds, the named pattern, the doable micro-action, plus the longer-arc receipts ledger.
- Push reliance: low. Retention rides on the internal cue (the urge), not on push. This is structurally healthy but also fragile in a different way: if the urge doesn't fire, the app doesn't open, and avoidant users may avoid the app itself (open question #1 in product_log flags this exact risk).

**Verdict line**
Two of three angles pass cleanly: psychological needs are well served (compétence + autonomie Strong) and the habit loop has a genuine internal cue with immediate reward. The job itself, however, is occasional rather than naturally recurring, and product_log open question #1 names the core retention risk: avoidant users may avoid the app in the moment it matters most. Without a recurring non-crisis use case (weekly review, calm-state ritual, partner check-in), opens will cluster around crisis moments that may be sparse, leading to long dormancy gaps.

**What needs to change for STRUCTURAL_RETURN**
- Is there a calm-state ritual (weekly pattern review, "receipts" digest, planned reflection) that brings the user back when no urge has fired, so the loop does not depend solely on crisis moments?
- How does Lean handle the avoidant-avoiding-Lean failure mode flagged in product_log Q1: is there a gentle external nudge tied to known high-risk windows (after a long emotional text was tagged, the next 48h) that does not feel like surveillance?
- Could a lightweight relational surface (anonymous shared wins from other avoidants, or an opt-in partner-facing "holding message" template) add a lien social dimension without breaking the solo, non-therapy framing?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

The spec has a sharp, specific persona and a vivid problem articulation that resonates with the avoidant pattern. However, the core mechanic (opening an introspection app *in* the moment of avoidance) is the exact behavior avoidants resist — this is acknowledged in the product_log but unanswered in the spec. Trust, privacy of intimate relationship data, and the trigger-to-open mechanism are also underspecified. Strong positioning, but the central behavioral assumption is unvalidated.

**Dangerous assumptions:**
- Avoidants will open an introspection app in the exact moment they're avoiding — the very brain state that drives the bolt urge also drives 'don't engage with feelings tools'. If this is wrong, H1 (45% open within 5 min of trigger) collapses and the product becomes a retrospective journal, which already exists. Cheap test: 1-week Wizard-of-Oz SMS with 20 self-identified avoidants — send them a single check-in prompt when they self-report a trigger, measure whether they engage in <5 min.
- Users will pre-load their personal patterns and triggers during setup — but avoidants resist structured self-disclosure, especially about romantic vulnerabilities. If setup friction is too high, nobody gets to the in-the-moment value. Cheap test: paper-prototype the onboarding with 5 target users, measure completion and quality of pattern entries.
- The 'small counter-move' suggestion will feel like coaching rather than nagging in the heat of an urge. If users experience it as the app taking the other person's side, they close it and bolt anyway. Cheap test: show 10 avoidants three sample suggestions mid-scenario role-play, ask whether each lands as ally or judge.
