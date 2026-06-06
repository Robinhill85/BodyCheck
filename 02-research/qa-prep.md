# Q&A Prep

Grounded in the prepared Q&A line in `cue-card.md` and the judge landmines in `manus-research-brief.md` (Deliverable 4). Short answers below are the ones already locked in the workspace. Fully sourced answers to the clinical/technical questions are still pending the published Manus research (see `/TODO.md`); do not improvise numbers.

> Not a medical device. Routing, not diagnosis.

## Locked answers (from the cue card)

**Q: Is this running on live wearable data?**
A: No. The demo runs on simulated wearable data. The API layer is built and a live connection is possible, but the demo is not live. We were explicit about this on the site and in the pitch.

**Q: Is the AI making the clinical decision? Is that safe?**
A: No. A deterministic rules engine decides the state, so it is traceable and auditable and never invents a diagnosis. The language model has one job: explain the state and the next step in plain English. AI makes the system understandable; it does not make the clinical decision.

**Q: What happens in a real emergency / crisis?**
A: A logged red-flag symptom (for example chest pain or severe difficulty breathing) bypasses the trend logic and jumps straight to Action Needed with urgent signposting: 999, NHS 111, and Samaritans 116 123.

**Q: What did you actually build, and what tools did you use?**
A: We built the frontend, the deterministic rules engine, the API layer, and the simulated wearable datasets, plus the pitch site, brand kit, and creatives. Tools: GLM in Cursor for build and synthesis, Manus for research and competitor analysis, Fotor for creatives. Links are on Devpost.

## Verified answers (see `qa-and-corrections.md`)

**Q: Isn't a wearable-based tool regressive? Lower-income students are less likely to own a wearable.**
A: Frame on the age band, not "students": roughly 46 to 47% of UK 18-34s own a smartwatch (YouGov, March 2025). Pair with the equity feature: plain-language and future multilingual explanations as a health-literacy lever. The figure is age-band, not student-specific, so "nearly half" is the supported phrasing.

**Q: How do you handle GDPR and the health data this collects?**
A: Three points (full version in `qa-and-corrections.md`): (1) wearable and symptom data are special-category health data under Article 9 UK GDPR, so highest-tier handling with explicit opt-in consent and right to erasure; (2) the demo runs on simulated data, so no real personal data is processed yet, engine runs locally where possible, data minimised, never sold, and a DPIA would be completed before any real deployment; (3) routing not records: BodyCheck points to NHS 111 / GP / wellbeing and does not create a clinical record or auto-share. Do not upgrade "we would complete a DPIA" to "we have."

**Q: Are the competitor claims accurate?**
A: Use the corrected matrix in `competitor-matrix.md`. Apple does have cardiac alerts; incumbents do recommend (fitness) actions. The gap is symptom-fusion plus UK care routing plus red-flag handling.

## Still to compile (TODO)
- The 5 hardest factual questions a clinical or technical judge could ask, each with a short sourced answer (Manus research brief, Deliverable 4). Confirm whether the Manus run returned them; fold into `qa-and-corrections.md` if so.
