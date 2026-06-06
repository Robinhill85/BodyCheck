# zai-orbit-evidence.md — robin-bodycheck
> Z.ai × Orbit lens · VibeHack London 2026 · Captured by Orbie v2.0.9

---

## D1 — Meaningful use

GLM via Z.ai was chosen as the plain-language explanation layer for BodyCheck's body state output. The stated rationale (visible in the site copy and the "Real-World Potential" card): *"The plain-language explanation layer is powered by GLM via Z.ai. This is not bolted on — it is the core UX differentiator. The model translates deterministic risk signals into human-readable, actionable guidance."* The deterministic rule engine handles the risk classification; GLM handles the communication of that classification to a non-clinical user. The split is deliberate — the engine is conservative and auditable; the LLM is the interface layer only. — **articulated**

## D2 — Workflow clarity

**Product facet:** GLM sits at the output layer of the shipped product — it receives the body state (one of five) and generates the plain-English explanation and single recommended action shown to the user. It does not participate in the risk classification itself.

**Workflow facet:** The build agent (Manus AI) was used throughout the session for scaffolding, full-stack conversion, copy corrections, and image integration. GLM/Z.ai is the product's LLM, not the build agent. The two roles are distinct and non-overlapping. — **articulated**

## D3 — Real-world value

BodyCheck addresses the gap between student distress and help-seeking: 1 in 6 UK students reports a mental health difficulty (TASO); fewer than 6% disclose to their university (House of Commons Library, Apr 2025). The GLM layer is what makes the output actionable for a non-clinical user — it converts a body state label into a plain-English explanation and a single proportionate next step (from "rest today" to "call NHS 111"). Without the explanation layer, the output is a label; with it, it is a routing decision. — **scaffold-ready**

## D4 — Evidence quality

- The Z.ai × GLM integration is referenced in the live site at `bodycheck-mzfvhzqq.manus.space` (Real-World Potential section, "Z.ai × GLM integration" card).
- The footer carries the `Z.ai × Orbit lens active` attribution.
- The LLM integration uses the `invokeLLM` helper from the Manus platform (backed by GLM), called server-side from a tRPC procedure to avoid key exposure.
- No prompt snippets or API call logs were captured in this session — D4 evidence is scaffold-ready, not fully articulated. Robin should add a screenshot of a GLM response or a prompt snippet to `/evidence/` to strengthen this dimension. — **scaffold-ready**

## D5 — Case study

BodyCheck was built in a single continuous session at VibeHack London 2026 (6–7 June, UCL). The build went from a static pitch page to a deployed full-stack application with wearable-signal routing logic, an LLM explanation layer, S3 file storage, and Manus OAuth. A second-pass accuracy audit was run before submission, correcting three overclaims (NHS branding, NHS 111 savings assertion, live-data implication). The live site is publicly accessible at `bodycheck-mzfvhzqq.manus.space`.

**Q6 — Open to a short post-event interview?** Skipped by builder at close.

---

*No evidence invented. Dimensions with thin evidence are marked scaffold-ready. D4 would benefit from a prompt snippet or API screenshot added to `/evidence/` before submission.*
