# Held — judges verdicts

## benchmark-scanner: `CROWDED_SPACE`

The platonic-touch space has a 20-year-old incumbent (Cuddle Party, founded 2004, with a global certified-facilitator network running exactly the eight-to-twelve-people, two-hour, consent-scaffolded format Held describes) plus active 1:1 marketplaces (Cuddlist, Cuddle Comfort, Cuddle Companions) and physical studios (Embrace Club NYC, Snuggle Salon, Cuddling Haven). The graveyard is also dense and specific: every app-based attempt at this problem (Cuddlr, Spoonr) died from the same failure, men using it as a hookup channel, which is exactly the risk Held's spec flags. Held's format is nearly identical to Cuddle Party's, so the wedge is not the format. The team needs a sharp answer to "why us, not a Cuddle Party franchise."

**Top competitors:**
- Cuddle Party Inc., facilitated 3.5h group platonic-touch workshops with certified facilitators worldwide, active since 2004 (cuddleparty.com)
- Cuddlist, professional 1:1 cuddle-therapy marketplace with certified practitioners, active (cuddlist.com)
- Cuddle Comfort, largest platonic-cuddling platform connecting buddies and pro cuddlers, active (cuddlecomfort.com)
- Embrace Club, NYC's first dedicated professional cuddle studio, structured consent-based sessions, active (embraceclub.com)
- Cuddle Puddle / Snuggle Lab and Meetup cuddle groups, recurring local facilitated group events (versicolorcoaching.com, meetup.com/topics/touch)

## retention-validator: `WEAK_RETURN`

VERDICT: WEAK_RETURN

**Le job que l'app fait pour l'user**
Get the platonic physical touch my body needs, in a setting safe enough that my nervous system actually relaxes.
Classification: naturally recurring (the bodily need for touch recurs continuously, like hunger or sleep)

**Besoins psychologiques nourris**
- Compétence (sentiment de progresser, de maîtriser): Weak. There is a faint progression (attend, attend again, eventually host or steward) but no visible mastery surface, no measurable progress the user can feel between events.
- Autonomie (sentiment d'être en contrôle): Strong. The whole design is consent-first, opt-out at any moment, choose which parts to participate in, leave when you want. Control is the product.
- Lien social (sentiment d'être connecté à d'autres): Strong. Recognising faces over time, acquaintances and friends emerging, shared vulnerability with a fixed local group. The relatedness is literal and embodied.

**Boucle d'habitude**
- Déclencheur: the bodily feeling of touch deprivation between events, plus the calendar reminder for the next RSVP. Mixed INTERNAL (somatic ache) and EXTERNAL (event scheduling).
- Routine: open app, RSVP to next event, show up in person two weeks later.
- Récompense: the actual touch and nervous-system regulation at the event. Immediate Y at the event, but NOT immediate inside the app. In-app reward is essentially zero, the app is a booking shell.
- Push reliance: retention depends heavily on event cadence and external scheduling cues. The app itself has no daily surface, no in-product reward loop. If event frequency drops or push is off, the app is invisible.

**Verdict line**
Need recurrence passes clearly, touch deprivation is as recurring as it gets, and SDT passes on autonomy and relatedness. The habit loop fails as an app-level loop: there is no in-product routine with immediate in-product reward, the reward lives entirely offline at the event, and the spec deliberately strips out every daily surface (no DMs, no profiles, no scroll) for safety reasons. Two angles pass, one fails, but the failing angle is structural to the app-vs-service question already flagged in product_log. Calling it WEAK_RETURN rather than STRUCTURAL because the product is closer to an event-booking shell than a returnable app, and retention rides almost entirely on event supply cadence.

**What needs to change for STRUCTURAL_RETURN**
- Is there a between-events surface that the user would actually want to open, without it drifting into the DMs/profiles/scroll territory Held explicitly forbids?
- Can recognising-faces-over-time become a visible, in-product progression (attendance history, stewardship path, returning-to-the-same-circle) without turning into a social graph?
- What is the cadence of events in a given city, and is it frequent enough that RSVP-to-attendance becomes a rhythm rather than a one-off booking every few months?

## user-interview-simulator: `BUILT_ON_SAND`

Held has a sharply named pain and a clear target, and the spec is unusually honest about the structural safety design. But the value proposition rests on three load-bearing claims that the spec does not back: that the wedge user will actually walk into a room with strangers to be touched, that an app (vs a hospitality org) can deliver this at all, and that the safety scaffolding survives contact with reality (in particular the gender-balance and predator-screening problem flagged in the log itself). A skeptical 32-year-old who currently copes by going to yoga and getting massages would leave the interview unconvinced, not because the idea is bad, but because the spec hasn't proven anyone crosses the threshold.

**Dangerous assumptions:**
- The target user will actually attend a first event. Naming the need privately is a very different act from showing up in a room with 8-12 strangers to be touched. The spec assumes the wedge ('already named it') converts, but offers no evidence anyone has ever paid, RSVP'd, or shown up for this. Cheap test: post a landing page offering a single $40 facilitated session in one city, count RSVPs and no-shows before building anything.
- The safety scaffolding actually holds, especially around gender balance. The product log flags this as open. Without a screening model, a gender-mix policy, and a facilitator standard, the first incident kills trust permanently and H3 (99% incident-free) is a wish, not a plan. Cheap test: run 3 pilot events with a hired somatic facilitator and a hard 50/50 cap, measure withdrawals, complaints, and second-event return rate manually.
- This is a software product Amon Studio can run. The economics are hospitality (venues, insurance, trained facilitators, liability, city-by-city ops), not an app. If unit economics don't work without subsidising every event, the 25% / 60% / 99% targets are irrelevant. Cheap test: model one event end to end (venue + facilitator + insurance + no-show rate) at a price the target will actually pay, and check if the contribution margin is non-negative before writing a line of code.
