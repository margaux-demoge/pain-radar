# Prose — judges verdicts

## benchmark-scanner: `GRAVEYARD`

The "blur photos until you chat" mechanic has been tried at least 5 times in the last decade (Appetence, Taffy, JigTalk, S'More, Blindlee) with one closure, two pivots away from the mechanic, and one niche survivor. The recurring failure is a cold-start and gender-ratio collapse: women won't write first to faceless strangers, men over-message, and the friction kills top-of-funnel before network effects can form. Lex is the only text-first app that scaled, and it did so by anchoring to a queer community identity rather than the blur mechanic. Prose needs a sharp answer to why the same UX gimmick will work in 2026 when it has not before.

**Top competitors:**
- S'More — active US dating app where photos unblur as you chat, exact same mechanic as Prose (https://smoreapp.com/faq)
- Blurry: Personality Dating — live on Google Play, personality-first with blurred photos (https://play.google.com/store/apps/details?id=com.hyperitycorp.app.inside)
- Lex — text-first queer personals app, acquired by 9count 2024, 1M+ downloads, the only text-first app that broke out (https://en.wikipedia.org/wiki/Lex_(app))
- Blindlee — voice-first with blurred video that sharpens on mutual consent, active (covered in 2025 roundups)
- Lovetastic: Pictureless Dating — niche no-photo app live on App Store (https://apps.apple.com/us/app/lovetastic-pictureless-dating/id1482035379)

## retention-validator: `WEAK_RETURN`

**Le job que l'app fait pour l'user**
Find a romantic partner who values me for my mind, not my face. Classification: occasional (recurs while single, but the goal is to exit the app once a partner is found, and dating intent is unpredictable session to session).

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. Writing better prompts and opening messages could feel like a craft, but the spec does not design any visible progress signal (no feedback on writing, no streak, no skill ladder).
- Autonomie (sentiment d'être en contrôle): Weak. The user controls what they write, but the core mechanic (blur until 3+3 messages, no tap-to-like) actually constrains autonomy more than typical dating apps. The premise is intentional friction, not control.
- Lien social (sentiment d'être connecté à d'autres): Strong. The entire product is human-to-human conversation, with substance-first matching and a commitment-moment unblur. Relatedness is the core promise.

**Boucle d'habitude**
- Déclencheur: loneliness / desire for a date / a notification that someone replied or unblurred. Mixed: internal cue (single, want connection) exists but is diffuse and not daily; the reliable cues are EXTERNAL (push when a message or unblur happens).
- Routine: read a profile, write a 50+ char opening message, or continue a conversation toward the 3-message threshold. Heavier routine than swiping, friction explicitly raised.
- Récompense: a reply, a good conversation, eventually the unblur reveal. Immediate Y/N: No for new opens (reply comes later); Yes once a thread is live (each reply is a small reward, and the unblur is a strong delayed reward).
- Push reliance: high. Without push on "new message" and "photos just unblurred," the loop likely collapses because the internal cue (am I horny / lonely tonight) is the same cue every dating app fights over, and Prose has higher friction than competitors.

**Verdict line**
Only one of three angles clearly passes: lien social is Strong and is the structural reason people would return. The job is occasional not naturally recurring (users churn on success, which is fine for dating but means no daily pull), and the habit loop relies heavily on external push with delayed rewards on the cold-start side (writing an opener and waiting). Compétence and autonomie are both Weak, and there is no progress surface or craft loop to compensate. The product can survive launch on novelty and the social hook, but week-4 retention will depend almost entirely on whether replies come fast enough and push notifications stay on.

**What needs to change for STRUCTURAL_RETURN**
- Is there a way to make writing feel like a craft that improves visibly over time, so users get a compétence reward independent of whether a match replies?
- What is the in-app reward when a user opens Prose and has zero new replies, so the session is not a dead end?
- Can the unblur moment or conversation milestones generate an internal cue stronger than "I am lonely tonight," something tied to a specific time or ritual the user adopts?

## user-interview-simulator: `BUILT_ON_SAND`

Prose is built on a stack of unvalidated behavioral leaps: that word-strong daters will write 50-char openers to faceless profiles, that the gender ratio won't collapse on day one (the spec doesn't even address it, despite product_log raising it), and that the unblur reveal won't just relocate the photo-judgment moment to message 6 instead of message 0. The category graveyard (Lex, Pure Words, original Hinge) is acknowledged as an open question but not answered in the spec. The positioning is crisp and the persona is clear, but the three load-bearing assumptions all sit in UNANSWERED territory.

**Dangerous assumptions:**
- Women will write 50-char unsolicited openers to men whose faces are hidden, at a volume sufficient to keep the marketplace alive. Cheap test: landing page + waitlist split by gender, ask 'would you message first, blind?' and measure female sign-up rate vs male; also run a 20-person concierge round where women must write the opener.
- The unblur at message 6 does not just relocate the rejection: people who invested 3 messages each will mostly continue post-reveal. Cheap test: Wizard-of-Oz over Telegram with 30 pairs, manually blur/unblur after 3+3, measure continuation 24h post-reveal vs a control where photos were visible from message 1.
- Writing-led matching produces meaningfully better date conversion than photo-led, not just slower funnels. Cheap test: take 50 Hinge profiles, strip photos, give the text-only versions to a panel of target users, measure willingness-to-message vs the photo version and 1:1 interview the deltas.
