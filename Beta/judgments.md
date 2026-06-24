# Beta — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

VERDICT: CROWDED_SPACE

**Problem benchmarked**
Solo gym boulderers can't tell if their sequence on a route is efficient or right for their body, and YouTube/strong-climber beta doesn't match their reach, weight, or wingspan before the route gets stripped.

**Direct competitors**
1. KAYA, climbing log + per-climb page with 300k+ beta videos, fist-bumps, comments, gym partnerships (Touchstone, Movement, Momentum). Status: active and scaling. https://kayaclimb.com/ and https://gearjunkie.com/climbing/kaya-climbing-app-strava
2. Beta Bud, gym-focused app with per-route "Beta Views" where users upload beta videos and view tips from others, plus progress tracker and leaderboards. Status: active. https://betabud.app/map and https://apps.apple.com/us/app/beta-bud/id6476326306
3. SocialBoulder, per-route community videos with comment threads, gym map, spraywall route creation. Status: active. https://mwm.ai/apps/socialboulder/6736912174
4. Bouldering AI, film an attempt and get a 0-100 score plus frame-by-frame annotations on hip distance, foot precision, engagement timing; chat coach "Coach Seb". Status: active, iOS launch. https://www.titans-grip.com/blog/best-bouldering-app-2026/
5. Cima, upload a climb and get portrait-first AI breakdown with pose tracking, movement scores, coaching notes, credits-based pricing. Status: active. https://getcima.app/
6. ClimbAI, computer vision AI trained on 6,000+ hours of climbing footage annotated by coaches, peer-reviewed validation. Status: launching with bouldering. https://climbai.app/
7. Belay AI, computer vision movement analysis with tailored feedback. Status: beta. https://belay.ai/

**Failed attempts**
None surfaced. The Kilter Board app shutdown was a third-party operator dispute, not a product-market failure, and it recovered with 35k downloads in three days. The category is in a growth wave (2024-2026), not a graveyard.

**Adjacent players**
1. Beta Friend, AI-assisted route setting for gyms via wall scan to 3D boulder proposals. Why relevant: same wall-scan primitive Beta would lean on, but aimed at setters not climbers. https://climbingbusinessjournal.com/beta-friend-launches-ai-assisted-route-setting-platform-for-climbing-gyms
2. ClimbAlong SPOT, camera + deep learning to auto-track ascents on any wall. Why relevant: infrastructure for automatic climb capture, could commoditise the "film your attempt" step. https://climbingbusinessjournal.com/ai-powered-routesetting-management-climbalong-spot-system-puts-route-data-at-your-fingertips/
3. Crimpd, training and conditioning programs for climbers. Why relevant: holds the "improve your climbing" intent without touching per-route video.
4. TopLogger, gym route management and logging used by many EU gyms. Why relevant: owns the per-route page in many gyms already, would be a default expansion target for video beta.
5. Mountain Project, route database and community comments, outdoor-focused. Why relevant: the canonical "route page is the unit" model Beta wants to bring to gyms.

**Failure pattern**
Not enough failed attempts to identify a pattern. The signal is the opposite: a 2025-2026 wave of well-funded entrants all converging on AI video analysis and per-route beta.

**Verdict line**
The space is crowded on two fronts at once. KAYA, Beta Bud and SocialBoulder already own "per-route page with community video", and Bouldering AI, Cima, ClimbAI and Belay AI already own "film your climb, get body-anchored feedback" (with frame-by-frame hip and foot annotations, which is exactly Beta's wedge minus the human reviewer). Beta's actual differentiator collapses to "human annotations from same-grade climbers at your gym, per-route trust", which is a real wedge but a narrow one stacked between AI coaches that don't need a community and community apps that already host video. The wedge has to be sharp. What does the team have that the top 3 competitors do not, and why won't KAYA ship timestamped video annotations as a feature inside their 300k-video network before Beta reaches critical mass at a single gym?

**Top competitors:**
- KAYA
- Beta Bud
- SocialBoulder
- Bouldering AI
- Cima
- ClimbAI
- Belay AI

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
Help a solo gym climber figure out, attempt by attempt, whether their body is doing the route the right way, by getting someone who has actually sent it to read the footage.
Classification: naturally recurring (gym sessions twice a week, every session produces new climbs to read)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong, the entire product is built around getting better at specific routes, seeing your sequence change between attempts, comparing your body to climbers who sent it cleaner.
- Autonomie (sentiment d'être en contrôle): Weak, the climber chooses what to film and which beta to try, but the structure (route page, trust ranking, body annotations) is mostly imposed by the app rather than configurable.
- Lien social (sentiment d'être connecté à d'autres): Strong, the unit of community is the route page where local climbers read each other's bodies, trust is earned by climbing, and the gym surface stays local so faces recur.

**Boucle d'habitude**
- Déclencheur: finishing a climb (or failing one) in the gym and wanting to know if you did it right, INTERNAL. Secondary external trigger: notifications when someone annotates your clip.
- Routine: film a 30s attempt, tag wall/grade (auto-detected), post to the route page; or open the app to annotate someone else's clip.
- Récompense: for the poster, seeing timestamped annotations on their own body within hours; for the reviewer, building per-route trust by reading someone else's climb. Immediate Y for the reviewer, delayed (couple of hours) for the poster.
- Push reliance: moderate, the poster-side reward depends on push to notify them when annotations arrive, but the internal cue of "I just climbed and want a read" carries the loop independently.

**Verdict line**
STRUCTURAL_RETURN because two of the three angles clearly pass: the underlying job recurs every gym session (2x/week minimum for the target user), and the product nourishes both compétence and lien social strongly through per-route stacking and per-grade trust. The habit loop is real and has an internal cue (finishing a climb), but the reward for the poster is not immediate, which is the weak point. The main structural risk is not retention shape but the bootstrap question already flagged in the product log: if a route page does not cluster enough readers within the 4-8 week set cycle, the loop dies on supply, not on demand.



## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

VERDICT: WEAK_ON_ASSUMPTIONS

**Simulated user**
Maya, 29, Brooklyn. Climbs at Brooklyn Boulders 3x a week, V3-V4 plateau, been stuck for 4 months. Logs sessions in KAYA, watches YouTube beta videos from Mani the Monkey and Magnus Midtbø. Films her hard projects on her own iPhone, sends them to a climbing friend over iMessage sometimes. Has tried Instagram for beta but the algorithm shows her pros, not peers. Mildly skeptical of new climbing apps, has churned out of three already.

**Interview**

Q1, "I already film my projects on my iPhone. Why do I open your app instead of just texting the clip to my one climbing friend who actually knows my body?"
> PARTIAL
Spec says the social cost of asking is high and friends aren't always there, but doesn't address why a stranger's annotation beats a known friend's text.

Q2, "Who is going to annotate my V4 at 7pm on a Tuesday when I post it? If nobody's there in the first hour the route is cold and I'm not coming back tomorrow."
> UNANSWERED
Spec aspires to "first annotated read within a couple of hours" but has zero supply-side mechanism. No reason given for why strong climbers would spend their gym evening reviewing strangers' clips.

Q3, "Why would the strong V8 climber at my gym waste her session annotating my hip position instead of climbing?"
> UNANSWERED
No incentive model for reviewers. Trust is "per-route per-grade-band" but that rewards the receiver, not the giver.

Q4, "My gym sets like 60 new problems a cycle. What are the odds three other climbers post on the same V4 within my one-week window?"
> UNANSWERED
This is exactly the open question flagged in product_log. Density math is not addressed. The "route page is the unit of community" only works if N>=3 per route per cycle.

Q5, "Wall-scan to identify the route, sure, but my gym has four walls with overlapping orange holds and the setters tape grades on. How reliable is this actually?"
> PARTIAL
Spec hedges with "when possible" and product_log lists accuracy as an open question. User wouldn't trust it.

Q6, "I'm 5'4". You promise I can find the 5'4" beta. How do you know the climber tagged their height honestly, or that I can filter to it?"
> PARTIAL
Mentions creative variations tagged for body type, but no mechanism for how height/reach metadata is captured or trusted.

Q7, "What stops this from becoming a place where four bros tell a woman to 'just campus it' on every clip?"
> UNANSWERED
No moderation, no tone control, no protection for the asker. Climbing forums have a known gender-tone problem and spec is silent.

Q8, "If I post a clip and only get one annotation from someone at my grade who's wrong, am I worse off than before?"
> UNANSWERED
No quality floor. Trust-by-sends only filters who, not whether their read is correct. False confidence risk untouched.

Q9, "Why do I trust the 'cluster beta' over the setter? The setter literally designed the route."
> PARTIAL
Setter can post intended beta, but the spec elevates cluster-emergent beta as the default. Tension not resolved.

Q10, "In six months when my gym strips and resets, the entire route page archive is dead weight. Why am I building history here instead of in KAYA?"
> UNANSWERED
No durable user value beyond the active route cycle. The product is structurally ephemeral but the spec doesn't articulate what the climber keeps.

**Score:** 0/10 answered, 4/10 partial, 6/10 unanswered

**Top 3 dangerous assumptions**

1. Reviewer supply will spontaneously appear within hours of posting. Why dangerous: the entire value prop collapses if clips sit unannotated; this is a two-sided marketplace cold-start with no proposed incentive. Cheap test: post 20 fake clips in 3 partner gyms' Discord/Slack and measure annotation latency without any product, just human behavior.
2. Route-level density is high enough to form a cluster before the strip. Why dangerous: if only 1-2 climbers post per V4 per cycle, the "route page" is empty and the differentiator vs KAYA disappears. Cheap test: count concurrent V2-V6 attempters on the same problem in one gym over a week via on-site observation.
3. Body-anchored timestamped annotations are meaningfully better than a friend texting "drop your hip at 0:04". Why dangerous: if the format is only marginally better than iMessage, retention against existing free behavior is near zero. Cheap test: A/B two WhatsApp groups for a week, one with text feedback, one with a Loom-style timestamped tool, measure repeat usage.

**Verdict line**
The positioning is specific and the mechanics are coherent, but six of ten user objections have no answer in the spec and the three killers (reviewer supply, route density, reviewer incentive) are all unaddressed. The product describes a beautiful demand side and an entirely absent supply side. Validate assumption 1 before any build.

**Dangerous assumptions:**
- Reviewer supply will spontaneously appear within hours of posting, no incentive model for strong climbers to annotate strangers' clips during their own session
- Per-route density is high enough to form a useful cluster within a 4-8 week set cycle in a typical gym
- Body-anchored timestamped annotations are meaningfully better than the existing free behavior of texting a clip to a climbing friend
