# Sprout — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

VERDICT: CROWDED_SPACE

**Problem benchmarked**
Home plant parents cannot get a fast, confident diagnosis for a sick plant before it dies, because forum threads are slow, contradictory, and free-form.

**Direct competitors**
1. Greg, plant care app with community troubleshooting where "veteran growers answer plant questions in minutes," plus AI plant ID and care, active and explicitly positioned on the community-diagnosis angle (https://greg.app/community/).
2. Planta, AI plant care app with "Dr. Planta" symptom analysis plus a Plant Community where users seek expert advice, premium tier lets you email plant experts with photos, active (https://getplanta.com/).
3. PictureThis, photo-based plant ID and disease diagnosis claiming 98% accuracy, 30M+ user community, paid botanist support tier, active (https://apps.apple.com/us/app/picturethis-plant-identifier/id1252497129).
4. Blossom, photo-based plant disease identification with cause, treatment, prevention, active (https://blossomplant.com/features/plant-disease-identification).
5. Agrio, AI plant disease ID with human expert fallback when AI is unsure, feedback loop trains the AI, active (https://agrio.app/An-app-that-identifies-plant-diseases-and-pests/).
6. Plantix, AI image recognition for plant diseases/pests/nutrient deficiencies, 98% accuracy claim, more crop-leaning but covers houseplants, active (https://farmonaut.com/blogs/best-ai-plant-disease-diagnosis-app-2025-free).
7. AI Plant Doctor, AI-trained on millions of plant images with 95%+ diagnosis accuracy, active (https://theaiplantdoctor.com/).

**Failed attempts**
None surfaced. Either nothing tried at this exact crowdsourced-triage angle has died publicly, or the failures are too small to be indexed. The dominant pattern has been AI-first apps absorbing community as a side feature, not community-first apps shutting down.

**Adjacent players**
1. r/houseplants, the slow free-form forum the spec explicitly positions against, massive but unstructured (https://reddit.com/r/houseplants).
2. iNaturalist, crowdsourced species ID with expert verification, model Sprout's reputation/verification layer echoes, no diagnosis focus (https://www.inaturalist.org/).
3. PlantNet, crowdsourced plant ID with community verification, no symptom triage (https://plantnet.org/).
4. University of Minnesota Extension "What's wrong with my plant?", structured decision-tree diagnostic, no community (https://apps.extension.umn.edu/garden/diagnose/plant/).
5. Facebook houseplant groups, scattered free-form diagnosis threads, slow.

**Failure pattern**
Not enough failed attempts to identify a pattern. Worth noting that no community-first triage app has clearly succeeded either, the winners (PictureThis, Planta, Greg) all started AI-first and bolted community on, which is itself a signal that pure-community triage may struggle on cold-start density.

**Verdict line**
This is a crowded space with at least 5 well-funded active players already combining photo-based diagnosis and community help, and the largest (PictureThis, Planta, Greg) have tens of millions of users plus paid expert tiers. Sprout's wedge (structured intake, tagged vote cluster, urgency queue, confirmed-outcome reputation loop) is real but narrow against incumbents who can copy any of those mechanics in a sprint. The wedge has to be sharp. What does the team have that Greg, Planta, and PictureThis do not, and can defend once they notice?

**Top competitors:**
- Greg
- Planta
- PictureThis
- Blossom
- Agrio
- Plantix
- AI Plant Doctor

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Get a fast, confident second opinion when a plant is showing distress, so the user knows what to do before the plant dies.
Classification: occasional (recurs unpredictably, only when a plant is visibly sick, which for a 5-30 plant collection might be every few weeks or every few months)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. The roster lets a plant parent see their own patterns over months (the west window keeps killing things), and diagnosers can earn quiet reputation, but neither is positioned as a central progression mechanic. Mastery is a side-effect, not a designed loop.
- Autonomie (sentiment d'être en contrôle): Weak. The user is in control of their plant roster and what they post, but the core experience is asking others for an answer, which is the opposite of autonomous mastery. The plant page they own privately is the autonomy anchor.
- Lien social (sentiment d'être connecté à d'autres): Strong. The entire product is a community diagnosing each other's plants, with reputation, confirmed outcomes, and a shared pattern database. This is the strongest of the three.

**Boucle d'habitude**
- Déclencheur: a plant looks sick, the user notices browning, yellowing, wilting, or pests. INTERNAL cue (the visible state of a plant the user already lives with), but only fires when something is wrong. For diagnosers, the cue is less clear, possibly a push notification when a new urgent triage lands, which would be EXTERNAL.
- Routine: structured two-minute intake (photos, species, conditions) for posters; tap a tag plus optional one-line note for diagnosers.
- Récompense: for the poster, a cluster of votes within the hour and the felt relief of knowing what to do. Immediate Y for posters. For diagnosers, reputation accrues slowly and "this was it" confirmation arrives days later. Immediate N for diagnosers.
- Push reliance: the diagnoser side of the loop likely depends on push notifications to surface urgent posts, since there is no internal cue pulling a diagnoser to open the app on a quiet day. This is a warning sign for the supply side of the marketplace.

**Verdict line**
Only the social-connection angle clearly passes. The job is occasional, not naturally recurring, which the team itself flags in the open questions ("is the use case too episodic to sustain a community of regular diagnosers"). The habit loop works for posters in crisis (strong internal cue, immediate reward) but is fragile for diagnosers, who carry the supply side and have neither an internal cue nor an immediate reward. One angle out of three passes, hence WEAK_RETURN.

**What needs to change for STRUCTURAL_RETURN**
- What internal cue would pull a diagnoser to open the app on a day when none of their own plants are sick, and what reward do they feel within seconds of doing so?
- Could the plant roster become a recurring routine on its own (weekly check-in, seasonal review, watering log review) so the app is opened between crises and not only during them?
- Could the compétence loop be tightened so that a plant parent feels measurable progress as a plant-reader, not just as a plant-owner, with feedback that lands within the same session rather than days later?

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

VERDICT: WEAK_ON_ASSUMPTIONS

**Simulated user**
Hannah, 31, Brooklyn. Has 18 houseplants, mostly monsteras, calatheas, pothos, a fiddle leaf. Killed a $90 Thai constellation last winter and still feels bad about it. Uses Reddit r/houseplants (lurker, posted twice), Picture This for ID, Greg for watering reminders, and a group chat with two plant friends. Mildly skeptical, time-poor, has tried "yet another plant app" three times and deleted all of them.

**Interview**

Q1, "Honestly when my plant is dying I just text my friend Maya who's good with plants. Why would I open a brand-new app with zero people in it instead?"
> UNANSWERED
The spec assumes a populated community on day one. Nothing addresses cold-start, where the first 100 posters get their diagnoses from.

Q2, "Two minutes of structured intake when I'm panicking, is that really faster than snapping a photo and posting on Reddit in 20 seconds?"
> PARTIAL
Spec claims under two minutes via taps and presets, but doesn't compare to Reddit's actual 20-second floor or justify the trade for the poster (only for the diagnoser).

Q3, "Six strangers say root rot, two say overwatering. I still have to decide tonight whether to water. How is a vote cluster actually more confident than the Reddit thread I already ignored?"
> PARTIAL
Spec asserts the cluster is "confident" but doesn't define a confidence threshold, doesn't explain what the poster does when the cluster is split, doesn't say whether the app recommends an action.

Q4, "Who are these random people voting on my plant? On Reddit at least I can read their comment history. Why should I trust a faint badge?"
> PARTIAL
Reputation is mentioned but the badge is described as deliberately quiet. From the poster's side, trust signals are thin.

Q5, "I'm supposed to be one of the diagnosers too? I open Reddit to scroll plant content, not to do unpaid triage work for strangers. What's in it for me?"
> UNANSWERED
The spec has no motivation model for diagnosers beyond "quiet reputation". No reciprocity, no notifications design, no reason to come back when none of your own plants are sick.

Q6, "I already use Picture This for ID and Greg for reminders. Are you asking me to add a third app just for the rare week a plant is dying?"
> UNANSWERED
Episodic use case is flagged in product_log as an open question. Spec doesn't resolve it. No story for what brings Hannah back between crises.

Q7, "Within the hour, you promise. What happens at 2am when my pothos is collapsing and there are four people online?"
> UNANSWERED
H2 targets 55% within 60 minutes but there's no mechanism for off-peak coverage, time zones, or the long tail of slow posts.

Q8, "I tap 'this was it' when the plant recovers. But half the time I'm not sure if it recovered because of the advice or despite it. How is this ground truth?"
> UNANSWERED
The confirmed-outcome loop is the spine of reputation and the pattern database, yet the spec doesn't address noisy/biased self-reporting or false positives.

Q9, "If my plant dies after I followed the cluster's advice, do I tap a 'this killed it' button? Because right now this app only learns from wins."
> UNANSWERED
No negative-outcome capture. Reputation and pattern data are systematically optimistic. This is a structural flaw the team likely hasn't asked.

Q10, "What stops the top reputation diagnosers from becoming a clique whose vote drowns out the new person who actually owns this exact rare species and knows the answer?"
> UNANSWERED
Weighted voting plus a quiet badge can converge to authority bias. Spec doesn't address how minority-but-correct voices break through, especially for rare species where the verified-identifier layer is thin.

**Score:** 0/10 answered, 3/10 partial, 7/10 unanswered

**Top 3 dangerous assumptions**

1. Diagnosers will show up and stay engaged for an episodic, unpaid triage workflow. Why dangerous: without a steady diagnoser pool, the under-60-minute promise (H2) collapses and the whole value prop dies. Cheap test: post 10 fake sick-plant intakes in r/houseplants with structured format, measure how many tagged diagnoses arrive within 60 minutes from volunteers given no incentive.
2. The "this was it" recovery tap is reliable enough ground truth to power reputation and a pattern database. Why dangerous: garbage-in reputation produces confidently wrong clusters, which kills H3 (35% confirmed recoveries) and trust in the diagnosis. Cheap test: take 30 historical r/houseplants threads where the OP came back, hand-code whether the "it worked" claim is actually attributable to the advice vs time / regression to the mean.
3. Cold-start, the first 500 posters get useful diagnoses from somewhere. Why dangerous: H1 (40% post monthly) is moot if early posts sit unanswered, the flywheel never spins. Cheap test: run a 2-week Discord or seeded subreddit version with 50 invited plant parents, see whether organic diagnoses materialize before paid/seeded ones run out.

**Verdict line**
Strong, specific positioning and a clear 10x mechanic versus Reddit, but the spec leans heavily on an unbuilt community arriving on time, self-reporting honestly, and showing up between personal crises. Three load-bearing assumptions are untouched. Validate the diagnoser-supply and ground-truth questions before building.

**Dangerous assumptions:**
- Diagnosers will show up and stay engaged for an episodic, unpaid triage workflow, sustaining the under-60-minute response promise
- The 'this was it' recovery tap is reliable enough ground truth to power reputation weighting and the pattern database
- Cold-start works: the first wave of posters get useful diagnoses from somewhere before a real community exists
