# BodyCheck — Devpost Submission

> Not a medical device. Routing, not diagnosis.

## Team
- **Team 19** — product name: BodyCheck
- **Abbas** — lead tech
- **Robin** — lead marketing

## Track
Track 1 — Health Impact · Challenge 3: Prevention & Early Intervention.

## One-line summary
BodyCheck is an early-warning and care-routing layer for UK university students: it turns wearable patterns and quick check-ins into one body state, one reason, and one next step.

## What we built
- A frontend with five body states (Stable, Watch, Elevated Risk, Action Needed, Recovery).
- A deterministic rules engine that decides the state from six signals (sleep, HRV/RMSSD, resting heart rate, skin-temperature deviation, respiratory rate, activity) plus symptom check-ins.
- An API layer (built and live-connection-capable).
- Simulated wearable datasets for a full seeded week (Maya).
- The pitch site, the brand kit, and the creatives.

## Who it is for
UK university students, and the wellbeing services that support them at cohort scale.

## What problem it solves
The gap between distress and help. 1 in 6 UK students reports a mental health difficulty; fewer than 6% disclose to their university. Wearables already see the early strain, but they stop at a score. BodyCheck turns that insight into a routing decision: it explains the state in plain language and, when needed, routes to NHS 111, a GP, or university wellbeing. A logged red-flag symptom bypasses the trend and goes straight to urgent signposting.

## How AI is used
Two layers, deliberately split. A deterministic rules engine decides the state, so it is traceable, auditable, and never invents a diagnosis. A language model (GLM via Z.ai) sits on top with one job: explain the state and the next step in plain English. AI makes the system understandable; it does not make the clinical decision. GLM in Cursor was used for build and synthesis, Manus for research and competitor analysis, and Fotor for creatives.

## Simulated-data note
The demo runs on **simulated wearable data**. The API layer is built and a live wearable connection is possible, but the demo is not live. We do not claim a live feed.

## Important corrections we hold to
- It references the "Student Health App" (Expert Self Care, relaunching Autumn 2026), not an "NHS Student Health App".
- The NHS 111 effect is framed as "could route the right people to the right level of care", never as a measured saving.

## Links
- **Live demo (Manus):** https://bodycheck-mzfvhzqq.manus.space/
- **GitHub repo:** https://github.com/alirezabedi/ModelAi-hackaton-mvp
- **Fotor creations:**
  - ECG five-state legend — https://www.fotor.com/explore/creation/6a2476df9e828f006d13ba36/
  - Wearable-score vs BodyCheck comparison — https://www.fotor.com/explore/creation/6a2477709e828f006d13ba48/
  - Elevated Risk phone mockup — https://www.fotor.com/explore/creation/6a2477dae950ee32f57e3ea2/
- **Manus research:** the live site itself was researched, scaffolded, and deployed via Manus (see note below). Confirm whether a separately published Manus task link is needed for the Manus award (TODO).
- **Ortie / Orbit package:** TODO (upload `ortie/robin-bodycheck/`)
- **Demo backup video:** TODO

## How Manus was used (award note)
Manus researched and sourced every statistic on the site (NHS data, TASO reports, YouGov figures) with inline citations, so the pitch launched with verifiable claims and a pre-answered judge Q&A. It then scaffolded the full-stack build (React, tRPC, Drizzle, S3 file storage) and deployed it as a live application without manual configuration. Before submission it audited the copy for overclaims: correcting a false NHS branding attribution, softening an unproven savings figure, and relabelling the hero demo as a simulated wearable stream.

## How Fotor was used (award note)
Three purpose-built visuals replaced generic stock imagery with graphics that explain the product. A neon ECG strip labelling all five body states sits in the Body States section as a visual legend for the interactive selector. A side-by-side comparison contrasting a wearable readiness score against BodyCheck's "Action Needed: Call NHS 111" output sits above the competitor matrix to frame the table before the reader reaches it. A phone mockup showing an Elevated Risk notification with plain-language reasoning anchors the hero section and makes the product tangible within the first scroll.
