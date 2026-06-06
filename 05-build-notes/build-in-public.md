# Build in Public — BodyCheck

VibeHack London 2026 · Track 1 Health Impact · Challenge 3: Prevention & Early Intervention. Honest log of what happened. Feeds the Ortie persona capture and the Z.ai Best Build-in-Public Story award.

> Not a medical device. Routing, not diagnosis.

## What we built
- **Frontend:** a five-state UI (Stable, Watch, Elevated Risk, Action Needed, Recovery) with per-state reason and one next step.
- **Rules engine:** a deterministic, auditable classifier that turns six wearable signals plus symptom check-ins into one body state. The engine decides; it never diagnoses.
- **API layer:** built and capable of a live wearable connection.
- **Simulated wearable datasets:** a full seeded week for the demo character, Maya.
- **Pitch site:** the public site at bodycheck-mzfvhzqq.manus.space.
- **Brand kit and creatives:** teal-on-near-black identity, ECG-waveform motif, logo files, and Fotor backgrounds.

## What changed and why
- **Narrowed to UK university students.** A specific, reachable audience beats "everyone with a wearable", and it let us use UK-specific, sourced stats.
- **Repositioned to an early-warning and routing layer.** We stopped competing on "another score" and claimed the gap incumbents leave: explanation, one action, and routing to care. Population-health value became the close, not the core, so the pitch stays human (one student first).
- **Made the simulated-data point explicit.** The demo runs on simulated wearable data; the API layer is built but the demo is not live. We say so on the site and in the pitch rather than implying a live feed.
- **Corrected the Student Health App label.** It is the "Student Health App" (Expert Self Care, relaunching Autumn 2026), not "NHS Student Health App". No implied NHS endorsement.
- **Softened the NHS 111 claim.** Dropped "measurable"; reframed as "could route the right people to the right level of care" rather than a quantified system saving.
- **Corrected the competitor matrix.** The first matrix claimed incumbents give no action and no safety logic. That was wrong: Oura/Whoop/Fitbit recommend fitness actions, and Apple has cardiac alerts, ECG, and Emergency SOS. We rebuilt the matrix so the differentiation sits where it is genuinely true: symptom-fusion plus UK care routing plus reported-red-flag handling.
- **Verified the YouGov figure.** Reframed wearable ownership as an age band (roughly 46 to 47% of UK 18-34s, YouGov March 2025), not a student-specific number we could not source.

## What failed
- **The UGC video.** The generator kept blocking it on a content-safety filter triggered by health and brand terms. Rather than fight the filter, we moved the message into editing: brand kit, motion motif, and on-canvas copy instead of a generated talking-head.

## What we learned
- **Use AI for visuals and own the text.** Generated backgrounds are fast; the words and the claims have to be ours and have to be defensible.
- **Deterministic engine for safety, LLM for explanation.** Keeping the clinical decision in auditable rules and using the model only to explain is what makes the product safe to demo and easy to defend in Q&A.
- **Validate stats to primary sources.** The hook is the distress-to-help gap; "1 in 6" and "fewer than 6%" carry the pitch, so they have to trace to TASO and the House of Commons Library, not to a blog.
- **Claim discipline is product work.** A second-pass accuracy audit before submission caught three overclaims (NHS branding, NHS 111 saving, live-data implication) and corrected them.

## Which tools did what
- **GLM in Cursor:** build and synthesis (and the product's plain-language explanation layer).
- **Manus:** researched and sourced every site statistic (NHS, TASO, YouGov) with inline citations, scaffolded the full-stack build (React, tRPC, Drizzle, S3 file storage) and deployed it without manual configuration, then audited the copy for overclaims before submission.
- **Fotor:** three purpose-built visuals, each placed to do a job. ECG five-state legend in the Body States section; a wearable-score vs "Action Needed: Call NHS 111" comparison above the competitor matrix; an Elevated Risk phone mockup anchoring the hero.
