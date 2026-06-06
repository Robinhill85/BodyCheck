# BodyCheck — Manus Research Brief
VibeHack London 2026 · Track 1 Health Impact · Challenge 3: Prevention & Early Intervention

## Context for Manus
BodyCheck is a prevention-first health companion. It reads wearable signals (sleep, HRV/RMSSD, resting heart rate, skin-temperature deviation, respiratory rate, activity) plus simple symptom check-ins, runs them through a deterministic risk engine that outputs ONE body state (Stable → Watch → Elevated Risk → Action Needed → Recovery), and uses an LLM only to explain the state and recommend ONE proportionate action (rest, hydrate, monitor, contact GP, call NHS 111, seek urgent help). For the prototype it runs on simulated wearable data; the API layer is built and a live wearable connection is possible, but the demo is not live. It is explicitly NOT a diagnostic tool.

Target audience for this pitch: UK university students. Do all research UK-specific and current (favour the last ~3 years). For every figure, return: the number, the source name, the publication date, and a working link. Prefer ONS, House of Commons Library, peer-reviewed journals, TASO, and Student Minds over blogs or SEO pages. Flag where sources disagree. Return everything as tables with sources inline.

---

## Deliverable 1 — Hook stat (Health Problem Relevance, 25%)
Find and rank 3-5 candidate stats, then recommend the single strongest opening line.
The strongest hook for a prevention product is the GAP between distress and help, not raw prevalence alone. Cover:
- Prevalence of mental-health / chronic-stress / poor-sleep burden in UK students (latest figures).
- The help-seeking / disclosure gap: how many struggling students never reach university or NHS support.
- The cost of late action: dropout, academic failure, or crisis presentations linked to unaddressed strain.
Output: the best "prevalence + gap" pairing for the first spoken line of the pitch.

## Deliverable 2 — Equity map (User Understanding & Equity, 20%)
Find UK student data, with sources, on who is less likely to be heard or helped, by:
- Socioeconomic background / state vs private school / low income.
- International students (language barriers, unfamiliarity with the NHS, GP-registration friction).
- Ethnic minority, LGBTQ+, disabled, neurodivergent, and first-generation students.
Then research the wearable-access tension honestly: UK wearable ownership by income and student status. We need a sourced answer to "isn't a wearable-based tool regressive?" before a judge asks it.
For each finding, map it to a BodyCheck feature (e.g. plain-language and future multilingual explanations = a health-literacy / ESL equity feature).

## Deliverable 3 — Competitor differentiation matrix (Practical Real-World Value, 20%)
Being connected to wearables is table stakes; the incumbents are connected too. Prove where they STOP.
Build a matrix. Rows: Oura (Readiness), Whoop (Strain/Recovery), Apple (Vitals), Fitbit (Daily Readiness), Samsung (Energy Score), plus any UK NHS-linked apps worth noting. Columns:
1. Produces a daily state or score?
2. Explains WHY in plain language?
3. Recommends a proportionate ACTION?
4. Escalates to care / signposts NHS 111 or GP?
5. Handles red-flag symptoms with conservative safety logic?
Extract the conclusion: incumbents largely stop at columns 1-2 (a score). BodyCheck's claim to be "different from what exists" lives in columns 3-5. Confirm or correct this against current sources.

## Deliverable 4 — Real-world potential + Q&A landmines (lighter)
- 3-4 talking points on practical value beyond the hackathon (feeds the Z.ai x Orbit "Best Real-World Potential" lens).
- The 5 hardest factual questions a clinical or technical judge could ask about this audience and these claims, each with a short sourced answer.

---

## Output + award note
Publish the Manus task and add the published link to Devpost. This research doubles as the Manus Real-World Use Case Award entry, where Published Evidence Quality is 20% of the score, so keep citations clean and the link accessible.
