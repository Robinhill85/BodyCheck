# Positioning

Synthesised from `pitch-script.md` and `cue-card.md`. This is the positioning spine the rest of the pitch hangs on.

> Not a medical device. Routing, not diagnosis.

## Category line (land it once)
**Wearables give scores. BodyCheck gives routing.**

## One-line positioning
BodyCheck is an early-warning and care-routing layer for UK university students. It turns wearable patterns and quick symptom check-ins into one thing a student can act on: their body state right now. Not a diagnosis. Not another score. One state, one reason, one next step.

## The spine (lead with one student; population value is the close, not the core)
1. **One student first.** Open on Abbas: wrecked sleep, resting heart rate climbing, HRV dropping. His watch sees the pattern; he does not. So nothing happens.
2. **The gap, not the prevalence.** 1 in 6 UK students reports a mental health difficulty. Fewer than 6% ever tell their university. The strain shows up early; the help arrives late.
3. **The product as the bridge.** Five states (Stable, Watch, Elevated Risk, Action Needed, Recovery). Each state gives one reason and one next step. On Action Needed, it routes to NHS 111, GP, or university wellbeing.
4. **Where incumbents stop.** Oura, Whoop, Apple, Fitbit, Samsung stop at a score. BodyCheck turns insight into routing and adds conservative red-flag safety logic. (See `competitor-matrix.md`.)
5. **Safety architecture as a feature.** A deterministic rules engine decides the state (traceable, auditable, never invents a diagnosis). An LLM only explains the state and the next step in plain English.
6. **Close on the cohort.** For students: less guessing. For universities: the same engine runs across a cohort, so strain gets spotted earlier across the student population, before pressure becomes crisis. Population health is the close, not the core.

## Guardrails on the claim
- The demo runs on simulated wearable data; the API layer is built and a live connection is possible, but the demo is not live.
- It references the "Student Health App" (Expert Self Care, relaunching Autumn 2026), not an "NHS Student Health App".
- The NHS 111 effect is framed as "could route the right people to the right level of care", never as a measured saving.
