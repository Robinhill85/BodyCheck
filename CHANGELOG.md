# Changelog

All structural and consistency-pass changes made while tidying the BodyCheck pitch project. No facts, stats, or claims were invented; missing items were moved to `TODO.md`.

## Corrections (post-close)
- **MVP repo link corrected:** replaced the wrong MVP URL with `https://github.com/DrbagherianCode/ModelAIMVP` across `TODO.md`, `04-devpost/devpost-submission.md`, `CHANGELOG.md`, and the Orbit persona files (`SKILL.md`, `manifest.md`). Persona zip repackaged.

## Reorganisation
- Renamed `01-pitch/BodyCheck_Pitch_CueCard.md` to `01-pitch/cue-card.md`.
- Renamed `02-research/bodycheck-manus-research-brief.md` to `02-research/manus-research-brief.md`.
- Renamed `02-research/manus-competitors.md` to `02-research/competitor-matrix.md` and populated it from the site comparison table.
- Renamed Fotor exports: `One state.jpg` to `fotor-one-state.jpg`, `elevated risk.jpg` to `fotor-elevated-risk.jpg`, `wearables.jpg` to `fotor-wearables.jpg`.
- Renamed `03-creatives/images_claude/` to `03-creatives/brand-logos/`.
- Moved `BodyCheck_Build_and_Demo_Brief.docx` to `03-creatives/bodycheck-build-and-demo-brief.docx` (the build pack).
- Moved the live-site snapshot into `03-creatives/pitch-site/` (kept internal `_files` folder name so relative links still resolve).
- Archived the stale duplicate site snapshot from `04-devpost/` to `_archive/devpost-site-snapshot.html` (+ `_files`).
- Archived `03-creatives/images_claude.zip` to `_archive/images_claude.zip` (duplicate of the unzipped `brand-logos/`).
- Removed empty `brand-kit/` folder and stray `.DS_Store` files.

## Consistency pass (canonical facts)
- **Simulated data:** `02-research/manus-research-brief.md` said "It already connects to live wearable data." Replaced with "For the prototype it runs on simulated wearable data; the API layer is built and a live wearable connection is possible, but the demo is not live."
- **Simulated data (clarity):** `01-pitch/pitch-script.md` changed "we simulate live wearable streams" to "we run on simulated wearable streams" to remove the live-data adjacency.
- **Routing, not triage:** changed "triage" to "routing"/"early-warning and routing" in `ortie/robin-bodycheck/manifest.md`, `ortie/robin-bodycheck/SKILL.md` (two places), and `ortie/robin-bodycheck/zai-orbit-evidence.md`.
- **Stat wording:** in `ortie/robin-bodycheck/zai-orbit-evidence.md`, changed "57% of UK students self-report a mental health issue; only 5.8% disclose" to the canonical pairing "1 in 6 UK students reports a mental health difficulty (TASO); fewer than 6% disclose to their university (House of Commons Library, Apr 2025)."
- **Disclaimer:** added "Not a medical device. Routing, not diagnosis." to every new document where a claim is made (README, brand-kit, positioning, competitor-matrix, qa-prep, demo-runsheet, creative-brief, build-in-public, devpost-submission).

## New documents written
- `README.md` — project synthesis and file index.
- `02-research/brand-kit.md` — colours, fonts, wordmark, motif extracted from the site source.
- `01-pitch/demo-runsheet.md` — day-by-day demo beats and checklist (from the script).
- `02-research/positioning.md` — category line and positioning spine.
- `02-research/competitor-matrix.md` — transcribed from the site comparison table.
- `02-research/qa-prep.md` — locked Q&A answers plus pending items.
- `03-creatives/creative-brief.md` — creative direction and asset set.
- `04-devpost/devpost-submission.md` — submission text and link placeholders.
- `05-build-notes/build-in-public.md` — honest build-in-public log.
- `TODO.md` — outstanding items before the deadline.

## Second pass (links, team, and verified corrections)
- **New file integrated:** `02-research/qa-and-corrections.md` (added by Robin) — verified YouGov figure, corrected competitor matrix, GDPR answer.
- **Competitor matrix corrected:** rewrote `02-research/competitor-matrix.md` to match `qa-and-corrections.md`. The earlier "incumbents give no action / no safety" claims were wrong (Oura/Whoop/Fitbit recommend fitness actions; Apple has cardiac alerts, ECG, Emergency SOS). Differentiation now sits on symptom-fusion plus UK care routing plus red-flag handling.
- **Q&A prep updated:** `02-research/qa-prep.md` now carries verified answers (YouGov age-band framing, GDPR, competitor accuracy) and points to `qa-and-corrections.md`.
- **Devpost links filled:** added live demo, GitHub repo (`github.com/DrbagherianCode/ModelAIMVP`), three Fotor creation links, and Manus + Fotor award notes. Team set to Team 19, Abbas (lead tech), Robin (lead marketing).
- **Creative brief updated:** documented the three delivered purpose-built Fotor visuals with placements and links; demoted the abstract Asset 1-3 backgrounds to optional.
- **Build-in-public enriched:** added the competitor-matrix correction and YouGov verification to "what changed"; expanded the Manus and Fotor tool entries with specifics.
- **Orbit manifest:** set `member_role` to "Lead marketing (Robin); Abbas = lead tech; Team 19" (was "assumed — confirm") and `github_repo` to the project repo.
- **README and TODO refreshed** to reflect resolved items.
- **Build pack docx updated:** replaced the stale Section 8.2 competitor table in `03-creatives/bodycheck-build-and-demo-brief.docx` with the corrected 4-column matrix (Oura/Whoop/Fitbit/Samsung, Apple Watch, BodyCheck), matching `competitor-matrix.md`. Arial, no em dashes, same position in the document.

## Not changed (flagged instead)
- The "Student Health App" (not "NHS Student Health App") label and the softened NHS 111 framing were already correct in the pitch script and cue card; no edit needed, and both are restated in the new docs.
- Competitor per-product capability claims are transcribed from the site, not independently verified; re-verification is listed in `TODO.md`.
