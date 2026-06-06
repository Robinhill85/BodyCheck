# Demo Runsheet

Synthesised from `pitch-script.md` and `cue-card.md`. The demo runs on **simulated wearable data** (the API layer is built and a live connection is possible, but the demo is not live). One character, Maya, a second-year at UCL, across one seeded week.

> Not a medical device. Routing, not diagnosis.

## Timing
- Demo window inside the 3-minute pitch: **0:50 to 2:10** (working product on screen before the one-minute mark).
- Whole-pitch target: **2:55**. Hold the two scripted pauses.
- If the demo breaks: cut to the backup recording and keep talking (recording still TODO, see `/TODO.md`).

## Day-by-day sequence

| Beat | State shown | What to say / show |
|---|---|---|
| Day 1 | **Stable** | "Day one: Stable. Everything normal." Show the dashboard, all signals in range. |
| Days 2-3 | **Watch** | Two bad nights plus a stressed check-in move her to Watch. "It does not panic her. One off night is normal, keep an eye on it." |
| Day 4 | **Elevated Risk** | HRV down, resting HR up, temperature elevated. Show what changed in plain language plus one action: rest, hydrate, reduce load today. "No form. No label." |
| Day 6 | **Action Needed** | Pattern persists and Maya logs a symptom. Routes to NHS 111, GP, or university wellbeing. "Wearables stop at insight. BodyCheck turns insight into routing." |
| Safety bypass | **Action Needed (instant)** | If Maya logs chest pain or severe difficulty breathing, skip the trend and jump straight to Action Needed with urgent signposting. "The wearable does not detect the emergency. The check-in does. That is deliberate." |
| Day 7 | **Recovery** | Signals settle. "The point is not to alarm her. It is to catch strain early and route her safely." |

## On-screen checklist
- Seeded Maya data (seven days) loaded before going on stage.
- Simulated data source labelled on screen (never implies a live feed).
- Each state transition happens visibly, not skipped.
- Action Needed screen shows NHS 111 / GP / wellbeing routing links.
- Red-flag path demonstrated as a separate quick flow.
- Disclaimer visible: "Not a medical device. Routing, not diagnosis."
- Backup recording cued (TODO).
