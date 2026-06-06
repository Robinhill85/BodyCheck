# BodyCheck: Q&A Prep and Corrections

VibeHack London 2026 · Track 1 Health Impact · Challenge 3: Prevention and Early Intervention

Place this in `02-research/`. It supersedes the "(verify)" and "draft" placeholders in the build brief. All figures below were checked against current sources during the hackathon. Trace each to its primary source once more before judging, and do not state a number you cannot source live.

---

## 1. YouGov wearable-ownership figure (verified)

The site cites a YouGov 2025 smartwatch-ownership figure. The real source is YouGov's March 2025 UK survey (nationally representative, 2,090 UK adults aged 18+, fieldwork 6-7 March 2025).

- 46% of 18-24-year-olds own a smartwatch.
- 47% of 25-34-year-olds own a smartwatch.
- 19% of those aged 55 and over.

Source: YouGov, "Nearly half of Britons concerned about wearable tech privacy," March 2025.

Defensible line: "roughly 46 to 47% of UK 18-34s own a smartwatch (YouGov, 2025)."

Two cautions:
- It is an age-band figure, not students specifically. Frame it as "the 18-34 band that most students fall into," not "students."
- Confirm the exact number printed on the site matches 46-47%. "Nearly half" is supported. A specific different number is not.

---

## 2. Competitor differentiation matrix (corrected)

The earlier matrix claimed incumbents give no proportionate action and no escalation or red-flag logic. Two of those claims are wrong and would fail in Q&A.

What changed and why:

- "No proportionate action" is false. Oura recommends rest below a readiness of 70. Whoop's Strain Coach recommends a restorative day on low recovery. Fitbit gives plain-language guidance ("plan for some moderate exercise, but don't overdo it"). They all recommend an action. The honest distinction is that the action is fitness and training oriented, not health routing.
- "No escalation, no red-flag logic" is false for Apple. Apple Watch has high and low heart-rate alerts and irregular-rhythm (AFib) notifications that encourage the user to seek medical follow-up, plus ECG, fall detection and Emergency SOS, and Apple tells users to call emergency services for suspected cardiac events. The narrow truth is that this is single-signal, cardiac-only, sensor-triggered, and framed for US emergency services, not a holistic body state or UK care routing.

Sources: Apple Support, "Heart health notifications on your Apple Watch" (2025); Oura Support, "Readiness Score"; VERTU / Whoop Strain Coach (Dec 2025); Tom's Guide, "Fitbit Daily Readiness Score."

Corrected matrix. The three bottom rows are where every product, Apple included, is genuinely "No." That is where the differentiation lives.

| Capability | Oura / Whoop / Fitbit / Samsung | Apple Watch | BodyCheck |
|---|---|---|---|
| Produces a daily state or score | Yes | No native score; cardiac alerts only | Yes |
| Explains why in plain language | Yes (contributors) | Partial (alert plus "see a doctor") | Yes |
| Recommends an action | Yes, but fitness/training oriented | Cardiac-only ("call emergency services") | Yes, health-routing oriented |
| Fuses wearable signals with a symptom check-in | No | No | Yes |
| Routes into UK care (NHS 111 / GP / university wellbeing) | No | No (US emergency framing) | Yes |
| Handles reported red-flag symptoms | No | Cardiac sensor events only | Yes |

Pitch framing that survives Q&A: "Apple can tell you your heart rhythm looks off and say see a doctor. None of them take a symptom you type in, combine it with your wearable trend, and route you to NHS 111, a GP, or your university wellbeing service. That is the gap." Drop the blanket "they just give a score" claim.

---

## 3. GDPR answer (drop-in for Q&A)

Question a clinical or technical judge is likely to ask: "How do you handle GDPR and the health data this collects?"

Answer:

Three points. First, classification: wearable and symptom data are special-category health data under Article 9 of the UK GDPR, so we treat them at the highest sensitivity tier. That needs explicit opt-in consent on top of a lawful basis, and consent can be withdrawn at any time, with a right to erasure.

Second, design: the demo runs on simulated data, so no real personal data is processed yet. By design the deterministic risk engine runs locally where possible, we store the minimum needed and no longer than needed, health data is never sold or used for advertising, and we would complete a Data Protection Impact Assessment before any real deployment, which is required for high-risk processing of special-category data.

Third, routing not records: BodyCheck points a user to NHS 111, a GP, or university wellbeing. It does not create a clinical record or send data to those services automatically. The user decides what to share.

Note: this answer is accurate about the current state (simulated data, not yet deployed). Do not upgrade "we would complete a DPIA" to "we have." The accurate version is stronger with a technical judge.

---

## Still outstanding (not in this file)

- The 5 sourced "hardest judge questions" with citations: requested in the Manus brief (Deliverable 4). Confirm whether the Manus run returned them, and fold them in here if so.
- Re-verifying any remaining competitor specifics beyond the rows above (for example Samsung Energy Score wording) if a judge presses on a brand not detailed here.
