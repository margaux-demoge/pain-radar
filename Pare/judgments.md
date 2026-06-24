# Pare — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The wardrobe-app category is dense with active, well-funded players (Whering, Indyx, Stylebook, Cladwell, Save Your Wardrobe, WithCloset, WearTracker) all touching the "what do I actually wear vs. what should go" problem. None of them, however, is laser-focused on the keep-or-donate decision with a paced, sentiment-surfacing flow plus an in-app donation booking step, so there is a real wedge but it sits inside a crowded category, not in open water. Failed attempts in this exact niche are not well indexed, which is itself a yellow flag: many cataloging apps have stalled at the "users dump 200 photos then quit" wall.

**Top competitors:**
- Whering — digital closet with cost-per-wear and 'forgotten clothes' nudges, sustainability angle; active, mobile-first (https://apps.apple.com/us/app/whering-your-digital-closet/id1519461680)
- Indyx — high-end digital wardrobe with catalog + resell, AI background removal, recently positioned as the 2026 benchmark; active (https://www.myindyx.com/)
- Stylebook — 10+ year incumbent, iOS, $4.99 one-time, wear tracking and donation candidate identification; active (https://apps.apple.com/us/app/stylebook/id335709058)
- Cladwell — outfit planner with Ask Cladwell GPT layer, frames itself as a smart closet that reduces overconsumption; active (https://cladwell.com/app)
- Save Your Wardrobe — AI closet digitisation focused on getting more life from existing pieces, sustainability framing; active (https://zerrin.com/best-wardrobe-organising-apps-sustainable-closet/)

## retention-validator: `WEAK_RETURN`

The underlying job (declutter my closet) is essentially one-shot or occasional: once the closet feels light, the user is done. SDT is partially nourished (competence via visible progress and the archive, autonomy via the 10/day cap and own pace) but lien social is absent. The habit loop has a plausible internal cue (opening the closet, feeling weight) and immediate reward (one decision off the pile, bag booked), but the loop expires when the closet is processed; the spec gestures at a post-90-day "what you actually wear" phase but doesn't define a recurring job after the initial declutter. Verdict: one angle (habit loop) clearly passes, SDT is borderline-passing on 2/3, but the job's lack of natural recurrence is the structural weakness.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Pare has a sharp emotional positioning (decision fatigue + sentimental weight) and a clear target (stuck declutterer). However, the product leans on three load-bearing assumptions that the spec doesn't defend: that people will photograph every item one-by-one, that a 10/day cap feels like progress instead of a chore, and that in-app donation booking can actually be delivered. Simulated user Rachel, 34, Lyon, already half-using Vinted and Marie Kondo videos, pushes back hard on the photo friction and the wear-tracking magic. 6/10 answered, 2 partial, 2 unanswered, with photo friction sitting in the danger zone.

**Dangerous assumptions:**
- Users will photograph every single item in their closet before getting any value. If photo friction kills onboarding, the whole loop never starts. Cheap test: paper prototype with 5 stuck declutterers, ask them to photograph 30 items before the first decision and measure drop-off.
- A 10-decisions-per-day cap feels like progress, not artificial slowness. If users perceive it as the app gatekeeping their motivation on a Sunday afternoon, they'll uninstall or batch-cheat. Cheap test: Wizard-of-Oz with two cohorts (capped vs uncapped) over 2 weeks, measure 30-day decisions decided and churn.
- Pare can actually deliver booked pickup/postage-paid bags at launch in target geographies. H3 targets 60% within 14d but the spec has zero partner named and product_log lists it as an open question. Cheap test: call 3 charities (Goodwill, Emmaüs, ThredUp) and confirm a postage-paid API or pickup booking is available before building anything.
