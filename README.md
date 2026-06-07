# BodyCheck — Pitch Project

> Not a medical device. Routing, not diagnosis.

## Overview
BodyCheck is an early-warning and care-routing layer for UK university students, built at VibeHack London 2026 (Track 1 Health Impact, Challenge 3: Prevention & Early Intervention). It reads wearable patterns (sleep, HRV/RMSSD, resting heart rate, skin-temperature deviation, respiratory rate, activity) plus quick symptom check-ins, runs them through a deterministic rules engine that outputs one of five body states, and uses an LLM only to explain that state and recommend one proportionate next step, routing to NHS 111, a GP, or university wellbeing when needed. The demo runs on simulated wearable data; the API layer is built and a live connection is possible, but the demo is not live.

## Positioning spine
Wearables give scores. BodyCheck gives routing. Lead with one student (Abbas), frame the gap (1 in 6 report a difficulty, fewer than 6% disclose), show the five states and the routing, explain the safety split (rules engine decides, LLM explains), and close on cohort value for universities. Population health is the close, not the core. Full version in `02-research/positioning.md`.

## 3-minute pitch, in brief
- **0:00 Problem** — Abbas' silent early signals; the distress-to-help gap.
- **0:25 Core idea** — one state, one reason, one next step; simulated streams so a week fits in three minutes.
- **0:50 Demo** — Stable to Watch to Elevated Risk to Action Needed (routes to care) to Recovery, plus a red-flag bypass.
- **2:10 AI + safety** — deterministic engine decides; LLM only explains.
- **2:35 Close** — students get less guessing; universities get earlier routing across a cohort.

## File index
| Path | What it is | Status |
|---|---|---|
| `01-pitch/pitch-script.md` | Full 3-minute spoken script | Done |
| `01-pitch/cue-card.md` | Condensed cue card for stage | Done |
| `01-pitch/demo-runsheet.md` | Day-by-day demo beats, timing, on-screen checklist | Done |
| `02-research/manus-research-brief.md` | Brief sent to Manus (4 deliverables) | Done |
| `02-research/competitor-matrix.md` | Corrected Oura/Whoop/Apple/Fitbit/Samsung vs BodyCheck | Done |
| `02-research/positioning.md` | Category line and positioning spine | Done |
| `02-research/qa-prep.md` | Judge Q&A; verified answers | Done |
| `02-research/qa-and-corrections.md` | Verified YouGov figure, corrected competitor matrix, GDPR answer | Done |
| `02-research/brand-kit.md` | Colours, fonts, wordmark, motif from site source | Done |
| `03-creatives/creative-brief.md` | Creative direction and asset set | Done |
| `03-creatives/brand-logos/` | Icon, primary/inverse wordmarks, ECG motif | Done |
| `03-creatives/fotor-*.jpg` | Exported Fotor state/wearable visuals | Done |
| `03-creatives/bodycheck-build-and-demo-brief.docx` | Builder build pack | Done |
| `03-creatives/pitch-site/` | Saved snapshot of the live pitch site | Done |
| `04-devpost/devpost-submission.md` | Devpost text, team, demo/GitHub/Fotor links + award notes | Done |
| `05-build-notes/build-in-public.md` | Honest build-in-public log | Done |
| `ortie/robin-bodycheck/` | Orbit persona package (SKILL, manifest, evidence, stats) | Done |
| `_archive/` | Stale duplicates kept for reference | n/a |
| `CHANGELOG.md` | Every consistency-pass change | Done |
| `TODO.md` | What is still missing before the deadline | Done |

## Repositories
- **This repo (pitch + docs):** the build-in-public story, brand kit, research, creatives, and Devpost text. Public.
- **Code (MVP application):** [Robinhill85/ModelAI-BodyCheck](https://github.com/Robinhill85/ModelAI-BodyCheck) — the working backend (Node/Express, Postgres) and frontend (React/Vite). Currently private; request access for review.

## Team
Team 19. Abbas (lead tech), Robin (lead marketing). Product: BodyCheck.

## Deliverable status
All deliverables complete:
- **Done:** pitch script, cue card, demo runsheet, brand kit, corrected competitor matrix, positioning, Q&A + corrections (YouGov, GDPR, competitors, and the 5 sourced judge questions verified), build-in-public log, build pack, brand logos, site snapshot, Devpost text with demo/GitHub/Fotor links, Manus award link confirmed, Ortie persona package uploaded to Orbit, demo backup recording captured, final pitch timing locked.
