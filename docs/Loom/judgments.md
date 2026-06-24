# Loom — judges verdicts

## benchmark-scanner: `EMERGING`

VERDICT: EMERGING

**Problem benchmarked**
Cross-stitchers working on multi-month pieces cannot get timely, useful, image-anchored peer critique on a WIP before they stitch over the mistake.

**Direct competitors**
1. Pattern Keeper, Android pattern marker with progress tracking, no community/feedback surface, active, https://lordlibidan.com/the-best-apps-for-cross-stitchers/
2. MarkUp Rx-P, iOS Pattern Keeper alternative, PDF marking + progress, no peer review layer, active, https://www.atomheartcrossstitch.com/post/pattern-keeper-vs-markup-rx-p
3. StitchPal, iOS WIP/stash/pattern tracker, dev-responsive but solo experience, active, https://apps.apple.com/us/app/stitchpal/id1550536005
4. Stitchly, pattern maker + progress tracking, no structured feedback, active, https://stitchly.com/
5. StitchCraft project tracker, organizes WIPs on iPhone/iPad, no community, active, https://stitchpatternmaker.com/cross-stitch-progress-tracker
6. XStitch Plus, tracker with social-media publishing baked in, but publishes outward (IG), no in-app structured critique, active, https://lordlibidan.com/the-best-apps-for-cross-stitchers/
7. Stitchingly, project tracker + inventory + "social media tool in one", in development, status fragile, https://lordlibidan.com/the-best-apps-for-cross-stitchers/

**Failed attempts**
None surfaced cleanly. The recurring community refrain across forums and blogs is "we wish we had a Ravelry for cross-stitch", which is itself evidence: many have asked, few have built, and no obvious carcass is indexed. Textillia exists as an unfunded indie attempt at the broader fibre-crafts community angle but has not become the answer for cross-stitch specifically (https://www.textillia.com/about). The absence of indexed failures may simply mean prior attempts were too small to leave a trace.

**Adjacent players**
1. Ravelry, knit/crochet community with project pages and pattern db, why relevant: the format Loom borrows, but explicitly does not sell or center cross-stitch, https://stitchtrove.com/ravelry-for-cross-stitch
2. r/CrossStitch, default WIP-posting venue today, why relevant: applause-heavy, slow, no per-photo anchoring, the exact gap Loom targets, https://reddit.com/r/CrossStitch
3. Textillia, indie sewing/quilting/embroidery community with project tools, why relevant: closest "Ravelry-for-everything-else" attempt, weak cross-stitch traction, https://www.textillia.com/about
4. Crossstitchforum, classic phpBB forum still active, why relevant: shows the audience still routes to dated tools for community, https://www.crossstitchforum.com/
5. Photo-critique tools (Picflow, Framebird, Filestage), why relevant: the image-anchored feedback primitive Loom needs exists in B2B creative review but has never been brought to a hobby craft, https://picflow.com/blog/image-annotations-the-best-tool-to-get-precise-feedback

**Failure pattern**
Not enough failed attempts to identify a pattern, but a structural observation: every existing cross-stitch tool is either a solo tracker (Pattern Keeper, MarkUp Rx-P, StitchPal, Stitchly) or a generic social surface (Reddit, Instagram, forum). No one has shipped the project-page-plus-anchored-feedback combination. The repeated community request for "a Ravelry for cross-stitch" suggests demand without a credible incumbent.

**Verdict line**
The category is full of solo tracker apps and one dominant external community (Reddit), but the specific wedge Loom claims, image-anchored structured critique on a persistent per-project page with shared pattern annotations, is currently unoccupied. Closest threats are StitchPal (active dev, listens to users, could add social) and Stitchingly (already trying the tracker+social combo, still in development). Window is open. Move fast before it crowds, and validate that stitchers will actually critique strangers' WIPs with the rigor the spec assumes, that is the real risk, not the build.

**Top competitors:**
- Pattern Keeper
- MarkUp Rx-P
- StitchPal
- Stitchly
- StitchCraft
- XStitch Plus
- Stitchingly
- Ravelry (adjacent)
- Textillia (adjacent)
- r/CrossStitch (adjacent)

## retention-validator: `STRUCTURAL_RETURN`

VERDICT: STRUCTURAL_RETURN

**Le job que l'app fait pour l'user**
"Get another stitcher's eyes on my in-progress piece before I sew over a mistake, and actually finish the projects I start."
Classification: naturally recurring (stitchers work on pieces in evening sessions, often daily or several times a week, over months)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Strong. The progress strip stacks WIP photos into a visible timeline, finished-hours and confirmed-helpful notes build reviewer credibility, the Finished shelf is the explicit reward.
- Autonomie (sentiment d'être en contrôle): Weak. Users set up their project (pattern, fabric, floss, deadline) and choose the feedback ask, but the experience is structured around prescribed asks and a fixed loop rather than open-ended self-direction.
- Lien social (sentiment d'être connecté à d'autres): Strong. Anchored peer feedback, shared pattern pages with collective annotations, project rosters visible to followers, designer responses. Connection is the core of the product.

**Boucle d'habitude**
- Déclencheur: end of an evening stitching session, the moment the user wants to check tension/colour before continuing. INTERNAL (tied to the craft routine itself), with a secondary EXTERNAL cue when feedback arrives on a tagged WIP.
- Routine: snap one photo from the same angle, optionally tag it with a specific ask, or open the app to review others' WIPs and leave anchored notes.
- Récompense: immediate Y, the photo lands in the progress strip and produces a visible satisfaction beat (Strava-like). Feedback reward is delayed up to ~24h, but the progress-strip reward closes the loop on its own.
- Push reliance: low. The spec explicitly says stitchers update without being prompted because the strip is satisfying enough. Push would carry the feedback-arrived signal but is not the load-bearing piece.

**Verdict line**
All three angles pass. The job recurs naturally with each stitching session over months; compétence and lien social are both Strong and structurally central (progress strip, anchored notes, shared pattern pages, Finished shelf); the habit loop has an internal cue (end of session), a quick routine (one photo plus optional ask), and an immediate visual reward independent of community response. Autonomie is the weakest leg but is not load-bearing here.

**What needs to change for STRUCTURAL_RETURN**
N/A, the spec already clears the bar. Watch items, not blockers: the open question in product_log.md about whether the long project horizon sustains weekly engagement between feedback moments is exactly the right one to test against H1, and the dependency on receiving anchored notes within 24h (H2) is the soft spot where the social leg could weaken if the network is thin at launch.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

VERDICT: WEAK_ON_ASSUMPTIONS

**Simulated user**
Hannah, 34, Manchester. Three years into cross-stitch, currently on a 60-hour Heaven and Earth Designs piece. Photographs WIPs on Sundays, posts to r/CrossStitch and Instagram, uses Pattern Keeper on her iPad to mark off stitched squares. Has two unfinished projects in a drawer. Mildly skeptical of new craft apps, tired of being asked to migrate her project tracking.

**Interview**

Q1, "I already use Pattern Keeper to track my progress and Reddit for feedback. Why would I run two apps instead of one?"
> PARTIAL
Spec contrasts with Pattern Keeper and r/CrossStitch but doesn't explain the migration cost or why Loom replaces rather than adds to my stack.

Q2, "Honestly, when I post a WIP I want applause, not critique. Why would I tag my piece 'tension on the dark areas' knowing strangers will pick it apart?"
> UNANSWERED
Spec assumes stitchers want critique. The emotional cost of asking for feedback on something you've spent 30 hours on is not addressed.

Q3, "Who is actually going to respond within 24 hours to my anchored note? On Reddit it takes days, what makes Loom different at day one when there's nobody on it?"
> UNANSWERED
Cold-start problem. H2 targets 45% within 24h but no mechanic explains how the supply of reviewers gets bootstrapped.

Q4, "I stitch on the sofa with the piece in my lap. Taking a clean, same-angle photo every session sounds like a chore. How long does this actually add to my evening?"
> PARTIAL
The "Strava-like satisfaction" claim assumes the photo ritual is frictionless. Lighting, framing, aida glare on fabric are not addressed.

Q5, "My pattern is a paid PDF from a designer on Etsy. Am I uploading copyrighted charts? Will I get my account nuked?"
> UNANSWERED
Pattern library licensing is flagged as an open question in the log but the spec presents shared pattern pages as a core mechanic. This is a legal cliff.

Q6, "I post a WIP asking about tension. Two stitchers tap the same spot with different opinions, one says rip it, one says blocking will fix it. What do I do?"
> UNANSWERED
Conflict resolution between anchored notes is not designed. "Confirmed-helpful" only resolves after I've already acted.

Q7, "What stops the anchored notes from being mean? On Reddit at least the upvotes filter the harsh stuff. You've removed likes."
> UNANSWERED
Moderation and tone are not addressed. Removing social signals removes the soft moderation Reddit relies on.

Q8, "I finish maybe two pieces a year. Why do I need a project roster that publicly shows my half-finished pile? That sounds like guilt-as-a-service."
> PARTIAL
Spec frames public roster as motivating ("the satisfaction of moving a piece into Finished"), but doesn't acknowledge that public unfinished-shame may push me to delete the app rather than finish.

Q9, "If I get feedback after 50 rows, I still have to frog 50 rows. The premise is feedback before the next session — what about people who stitch every night? Do I post a WIP every single day?"
> PARTIAL
H1 targets one WIP per week, but the value prop requires per-session cadence to actually catch issues early. The two don't line up.

Q10, "You're saying H3, projects with feedback get finished 20pp more. But what if the people who ask for feedback are just the more committed stitchers anyway? How do you know it's the feedback, not the selection bias?"
> UNANSWERED
The causal claim in H3 is correlational by construction. No mechanism to attribute finishing to feedback rather than to the type of stitcher who seeks feedback.

**Score:** 0/10 answered, 4/10 partial, 6/10 unanswered

**Top 3 dangerous assumptions**

1. Stitchers want critique on emotionally-invested WIPs, not applause. Why dangerous: if the dominant emotion when posting a WIP is "please validate me", the structured-ask format kills posting volume and the whole feedback loop dies. Cheap test: DM 15 active r/CrossStitch WIP posters, ask if they would have preferred anchored critique to the comments they got, and whether they would have posted at all knowing critique was the default.

2. Cold-start supply of reviewers can deliver 2 anchored notes in 24h from day one. Why dangerous: H2 at 45% within 24h requires a thick reviewer base before the first user arrives, and nothing in the spec bootstraps that. Cheap test: simulate it manually for 4 weeks in a Discord with 50 hand-recruited stitchers before building anything, see if response-within-24h is actually achievable at small scale.

3. Pattern library can be a shared object without designer licensing blowing up. Why dangerous: cross-stitch charts are paid IP. If the shared pattern page hosts user-uploaded PDFs, designers issue takedowns and the "collective annotations" value prop collapses. Cheap test: talk to 5 mid-size pattern designers on Etsy and ask under what terms they'd allow a shared chart page; if 0 of 5 say yes, the mechanic is chart-metadata-only, not chart-content.

**Verdict line**
The persona is sharp and the problem is real, but six out of ten questions have no answer in the spec, including the three load-bearing ones: emotional posture toward critique, cold-start of reviewers, and pattern licensing. The positioning survives scrutiny on what the product is, but not on why supply shows up or whether demand wants the format.

**Dangerous assumptions:**
- Stitchers want anchored critique on emotionally-invested WIPs rather than applause; if false, posting volume collapses and the feedback loop never starts.
- A cold-start reviewer base can deliver 2 anchored notes within 24h from day one with no bootstrap mechanic described in the spec.
- Shared pattern pages with collective annotations can exist without designer licensing; charts are paid IP and takedowns would gut the mechanic.
