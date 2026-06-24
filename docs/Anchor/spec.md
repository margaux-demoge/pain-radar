# ANCHOR

> **The app that catches the thought before the spiral.** Tell Anchor what's looping in your head about your partner, and it walks you back to ground before you send the text you'll regret.

---

## Status

- Phase 1 Exploration: stub from radar 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You love them, but you also can't stop watching them. A second-too-long like on someone's photo, a name you don't recognise in their phone, a tone shift over text, and your stomach drops. You know, when you're calm, that most of these signals are noise. But in the moment your brain runs the same loop: what if they're losing interest, what if they're with someone else, what if I'm the last to know. By the time you've checked their location and reread the same conversation eight times, you've already half-written the accusatory text. You send it, they get defensive, you feel worse, and the cycle confirms the fear you started with. The problem isn't that you don't trust them. It's that you have no way to interrupt your own spiral before it becomes the relationship's actual problem.

**Target users**

Primary: 19-29 year olds in committed relationships who self-identify as anxious or insecure attachers, who already know the spiral is theirs to manage but lack any tool that intervenes in the 90 seconds between the trigger and the text. They've read the attachment-theory TikToks and follow Jessica Baum or Heidi Priebe; they want a private workspace, not another therapist.

Not for: people in actually unsafe relationships, where the worry is grounded in real betrayal. Anchor is for catching distortions, not validating them. Also not for users seeking couples-counselling features, this is a tool you use alone.

---

## 2. Product experience

Anchor opens to one thing: a text field that asks "what's the thought". You type the loop as it's running in your head, raw, ungrammatical, doesn't matter. "She liked his post and didn't text me back for two hours and now I think she's bored of me." You hit send.

What comes back is not advice. Anchor reflects the thought back to you, structured. It names the trigger (the like, the gap in reply time), the prediction your brain made (she's bored, she's losing interest, she's choosing someone else), and the action you're about to take (send a passive-aggressive screenshot, check her location, accuse). Seeing your own spiral laid out, in the order your brain ran it, breaks the hypnosis. The thought stops being a fact and becomes a sequence.

Then Anchor asks one question, drawn from the texture of what you wrote: "When she's liked posts before, what happened next?" Or "Is there evidence she's pulling away, or is this the gap-in-reply story again?" You answer, or you don't. Either way, the spiral has been slowed down. After a few rounds, Anchor offers you a one-line summary you can keep, the kind of thing you could screenshot for yourself or read again next time the same loop starts.

Over weeks, Anchor learns your specific patterns, the triggers that come up most, the predictions you make most often, the texts you almost sent and didn't. It surfaces them gently: "this is the fifth time this month you've worried she's lost interest after a quiet evening. Each time, she wasn't." It's not therapy. It's a mirror that doesn't flinch and doesn't reassure, just shows you what your brain is doing in time to do something else.

In short: catch the spiral, see it laid out, and let it pass before you make it real.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | ------ |
| H1  | Users open Anchor in the moment of a spiral, not after the fact: the trigger-to-app gap is short enough that the intervention lands before the text is sent. | % of sessions opened within 30 minutes of a self-reported trigger.                      | 50%    |
| H2  | Seeing the spiral structured back reduces the user's urge to act on it: the "almost sent" text doesn't get sent.    | % of sessions ending with user reporting "I didn't send the text" or equivalent.        | 60%    |
| H3  | The pattern recognition over time changes how users perceive their own loops, not just their behaviour in one moment. | % of weekly active users who report fewer spirals in week 4 vs week 1 (in-app survey).  | 40%    |

---
