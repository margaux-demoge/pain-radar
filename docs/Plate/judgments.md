# Plate — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

Photo-based calorie logging is now the default battleground in nutrition tracking, not a wedge. Cal AI was just acquired by MyFitnessPal (rumored north of $100M) in early 2026, MFP shipped an upgraded Meal Scan in the 2025 Summer Release, and at least 7 other apps (SnapCalorie, Foodvisor, Bite AI, Lose It Snap It, Calorie Mama, Nutrola, PlateLens) offer the exact same "point camera, get calories" loop. The "imprecise but consistent" pitch is undifferentiated, every player above sells the same friction reduction. Independent benchmarks show food ID at 68-86% and portion accuracy as low as 39%, so Plate's accuracy bet is not a moat either.

**Top competitors:**
- Cal AI — point-and-snap calorie tracker, acquired by MyFitnessPal in early 2026 for a rumored $100M+, now the category reference (https://www.calai.app/)
- SnapCalorie — ex-Google AI team, 3D volume estimation with LIDAR, ~16% error rate, free tier with micronutrients (https://www.snapcalorie.com/)
- MyFitnessPal Meal Scan — built-in to the incumbent (200M+ users), upgraded AI in 2025 Summer Release, now bundled with Cal AI tech (https://blog.myfitnesspal.com/meal-scan/)
- Foodvisor — long-running photo logger, strong on European cuisine, freemium + dietitian add-on (https://nutriscan.app/blog/posts/foodvisor-worth-it-2026-review-73e3363135)
- Lose It! Snap It — photo recognition feature inside Lose It, 68.7% food ID benchmark, mass-market distribution (https://ai-food-tracker.com/reviews/lose-it/)

## retention-validator: `STRUCTURAL_RETURN`

The job (logging meals to hit a weight/fitness goal) is naturally recurring multiple times per day, driven by eating itself as a strong internal cue with an immediate reward (instant calorie/macro readout vs target). Competence is Strong via dashboard progress against target and 7-day average; autonomy is Strong via easy corrections, one-tap usuals, and no gamified pressure; relatedness is Absent by design. Two of three angles clearly pass: recurring need and a closed habit loop with internal cue, so verdict is STRUCTURAL_RETURN with relatedness as the noted weakness.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Plate has a sharp problem statement and a credible target persona, but it enters a crowded category (Cal AI, SnapCalorie, MFP meal scan) without articulating its wedge. The "precision-vs-consistency" bet is elegantly stated but rests on three unvalidated leaps: that photo accuracy is good enough to trust, that users will accept ±10-15% error after quitting MFP for being annoying (not inaccurate), and that the absence of motivation features is a feature not a gap. Persona Sarah, 32, Lyon, ex-MFP user now drifting on Yuka + mental notes, would answer 5/10 questions credibly from the spec, leaving the wedge and trust questions exposed.

**Dangerous assumptions:**
- Plate has a defensible wedge against Cal AI / SnapCalorie / MFP's own photo scan. Spec never names a competitor or a difference. Cheap test: spend 30 minutes logging the same 5 meals in Cal AI and a Plate mock, then ask 5 ex-MFP users which output they'd trust and why, the answer reveals if the wedge is UX, accuracy, pricing, or nothing.
- Users will trust a ±10-15% photo estimate enough to keep logging. The people who quit MFP quit because it was tedious, not inaccurate; once they see the photo estimate say 'rice 150g' when they know it's 250g, the trust may collapse faster than with manual entry. Cheap test: show 10 target users a photo + Plate-style estimate for 5 meals they cooked, ask 'would you accept this number or correct it?', count corrections per meal as a friction proxy.
- The no-motivation, no-streaks dashboard is what this segment wants. Spec asserts 'the app's job is not to motivate you' as a virtue, but the same users who quit MFP often cite losing motivation, not just friction. Cheap test: in 5 user interviews, ask 'when you stopped logging in MFP, was it because it was too much work, or because you stopped caring?', if 3+ say the latter, the no-motivation stance is wrong.
