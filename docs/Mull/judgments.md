# Mull — judges verdicts

## benchmark-scanner: `EMERGING`

The "should I stay" question is well-documented (ROCD literature, hundreds of Reddit threads, journal-prompt blog posts everywhere), but no app owns it as a thinking tool for ambivalent-but-not-unhappy partners. The category is split between two camps that miss Mull's wedge: couples-therapy apps (Lasting, Paired, Relish, Couples) that assume both partners are in and want to improve, and breakup/healing apps (Mend, Let it Go, Breakup Buddy) that assume the decision is made. AI journaling apps (Rosebud, Reflection.app, Day One) cover relationship prompts as one tag among many but don't structure a longitudinal mirror around a single unresolved question. The gap Mull targets, solo, longitudinal, non-interpretive pattern mirror for the unresolved "is this right" question, has no direct occupant; the risk is not competition but whether the use case sustains a standalone app vs. a feature inside Rosebud/Reflection.

**Top competitors:**
- Rosebud — AI journaling with relationship prompts and pattern surfacing, active, closest analog if it leaned into ambivalence (https://www.rosebud.app/)
- Reflection.app — solo AI journal that explicitly digs into relationships and connections over time, active (https://www.reflection.app/)
- Clarity: Love & Relationships — coach-driven 'is this the one' positioning but solves with experts and lessons, not solo mirroring, active (https://apps.apple.com/us/app/clarity-love-relationships/id6448745081)
- Lasting — Gottman-based couples counseling app, assumes both partners in, adjacent to but not solving Mull's solo-doubt question, active (https://getlasting.com/)
- Paired — daily two-sided question app for couples, requires partner participation, opposite of Mull's premise (https://www.paired.com/)

## retention-validator: `WEAK_RETURN`

Job: "sort out whether my doubts about my partner are signal or noise." Classification is occasional-to-one-shot, the spec itself frames resolution as exit (H3, median <6 months). Need recurrence is not naturally daily/weekly, the question recurs in waves not on a calendar, so the weekly prompt is app-imposed not life-imposed. SDT: Compétence Weak (mirror gives self-insight over weeks, not a felt mastery loop, reward is delayed), Autonomie Strong (private, skippable, no verdict pushed, no algorithm, "yours"), Lien social Absent by design (no sharing, no partner, no community). Habit loop: cue is the weekly prompt push, external, no internal trigger tied to a real-life moment (the 2am spiral capture is the one internal cue but it is the secondary feature). Routine is light (few sentences). Reward is delayed (patterns visible over weeks, digest after 4 weeks), not immediate. Only Autonomie passes clearly. The product explicitly accepts churn at resolution (H3), which is honest but means retention is structurally weak. Verdict WEAK_RETURN: one angle (autonomy) holds, the job is not naturally recurring, the loop leans on external weekly push with delayed reward.

## user-interview-simulator: `WEAK_ON_ASSUMPTIONS`

Mull has a sharp, well-articulated emotional thesis and a clearly defined persona (analytical 24-35yo in an ambiguous-but-good relationship). The product mechanic (notice, mirror, spiral-quarantine) is differentiated from quiz-style competitors and the "no verdict" stance is principled. But several core assumptions remain unvalidated: that weekly noticing surfaces signal rather than manufactures doubt, that users will write honestly in an app they associate with a high-stakes question, and that a tool whose explicit success state is "user leaves" can sustain engagement long enough to deliver value. The persona would press hard on the second-night problem: why open this app when the thought arrives at 2am and Instagram is right there.

Interview with Léa, 29, Lyon, 2.5 years with her partner, considering moving in, currently uses Notes app + voice memos to her sister + one therapist session a month, skeptical of "relationship apps" which she associates with couples-quizzes and astro-compat nonsense.

Q1, "Why would I open an app for this instead of just texting my sister like I already do?"
> PARTIAL. Spec acknowledges friends-can't-be-asked but doesn't explain why writing into Mull beats writing into Notes or voice memos to a trusted person.

Q2, "If I write 'I held something back tonight' every week, won't that just train me to find problems that weren't there?"
> UNANSWERED. This is open question #2 in product_log, the spec has no answer for the iatrogenic-doubt risk.

Q3, "What happens the first time I write something honest and then my partner finds my phone?"
> PARTIAL. Spec mentions no cloud sync optional, no sharing, but no concrete privacy/lock model described.

Q4, "I'm analytical, I want a score. You're telling me there's no score, no verdict, no recommendation. So what do I actually leave with?"
> ANSWERED. The mirror-not-verdict stance is the explicit thesis and consistently held.

Q5, "Show me the prompt you'd send me this week. Is it really different from the journaling app I deleted in March?"
> PARTIAL. Three example prompts are given but no theory of prompt design, no rotation logic, no defense against prompt-fatigue.

Q6, "The 'spiral, look at it in two weeks' thing, why two weeks and not three days or a month?"
> UNANSWERED. The cooldown duration is stated as a mechanic but never justified.

Q7, "If I do this for four months and decide to leave, am I going to blame your app for it?"
> UNANSWERED. This is open question #3, no exit ritual designed yet, and it's a real reputational/emotional risk.

Q8, "I tried Stoic and Reflectly and stopped after eight days. What makes you think I'll come back in week three?"
> PARTIAL. H1 assumes weekly return because the question doesn't resolve, but the spec offers no retention mechanic beyond the prompt itself, no notification philosophy, no streak, no friction-reducer.

Q9, "Who wrote these prompts? A therapist? An ex? Some PM in San Francisco? Because the wording will make or break whether I trust this."
> UNANSWERED. Provenance and authorship of prompts is not addressed, and for a product whose entire surface is the prompt, this is load-bearing.

Q10, "Your success metric is that I leave when I reach clarity. So you're building something designed to lose me. How is that not a hospice business?"
> UNANSWERED. Product_log Q1 flags this, spec has no answer on unit economics or whether Mull needs to live inside a broader product.

Score: 1/10 answered, 3/10 partial, 6/10 unanswered.

Top 3 dangerous assumptions:
1. Weekly noticing surfaces signal rather than manufacturing doubt. If wrong, Mull actively harms the relationships it claims to help. Cheap test: 4-week diary study with 10 users in "good but uncertain" relationships, half use Mull half use nothing, self-report doubt-intensity weekly.
2. The prompts themselves are good enough to carry the entire product. If the prompts feel generic or therapeutic-cosplay, users churn in week 2. Cheap test: paper-prototype the first 8 weekly prompts with 5 target users, measure willingness to answer and perceived depth before building anything.
3. Users will write honestly inside an app rather than performing for an imagined audience (themselves, a future therapist, a future ex reading the phone). If wrong, the mirror reflects a curated self and the whole thesis collapses. Cheap test: compare what users write in Mull-like prompt vs. what they say in a 1:1 interview about the same week, look for divergence.

This is a strong positioning piece with a distinctive voice, but six of ten user objections have no answer in the current spec, including the three flagged in product_log. The thesis is defensible, the execution risks are not yet addressed.

**Dangerous assumptions:**
- Weekly noticing prompts surface signal rather than manufacturing doubt where none would have settled. If wrong, Mull harms users. Cheap test: 4-week diary study, Mull vs control group of similar 'good but uncertain' users, measure doubt intensity weekly.
- The prompts alone carry the product. If they read as generic or therapeutic-cosplay, users churn in week 2. Cheap test: paper-prototype 8 weekly prompts with 5 target users, measure willingness to write and perceived depth before any build.
- Users will write honestly in the app rather than performing for an imagined reader (self, future therapist, partner who finds the phone). If wrong, the mirror reflects a curated self. Cheap test: compare Mull-prompt responses vs 1:1 interview about the same week, look for divergence.
