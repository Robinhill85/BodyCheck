# Pitch Script

0:00–0:25 · Problem
"Meet Abbas, a second-year at UCL. His sleep is wrecked. His resting heart rate has climbed all week. His HRV is dropping. His smartwatch sees the pattern. Abbas doesn't. So nothing happens.
One in six UK students reports a mental health difficulty. Fewer than 6% ever tell their university. [pause] The strain shows up early. The help arrives late."

0:25–0:50 · Core idea
"BodyCheck is an early-warning and care-routing layer for university students. It turns wearable patterns and quick symptom check-ins into one thing Abbas can act on: his body state right now. Not a diagnosis. Not another score. One state, one reason, one next step.
For this prototype, we run on simulated wearable streams so you can see a full week of progression in three minutes."

0:50–2:10 · Live demo (working product on screen before the one-minute mark)
"Day one: Stable. Everything normal.
Two bad nights and a stressed check-in move her to Watch. It does not panic her. It says one off night is normal, keep an eye on it.
Day four: HRV down, resting heart rate up, temperature elevated. Elevated Risk. It shows what changed, in plain language, and gives one action: rest, hydrate, reduce load today. She never filled in a form. She never had to label herself.
Day six: the pattern persists and Abbas logs a symptom. Action Needed. It routes him to NHS 111, his GP, or university wellbeing. That is the gap. Wearables stop at insight. BodyCheck turns insight into routing.
Now the safety bypass. If Abbas logs chest pain or severe difficulty breathing, it does not wait for a trend. It jumps straight to Action Needed and signposts urgent care. The wearable does not detect the emergency. The check-in does. That is deliberate.
Day seven: signals settle. Recovery. The point is not to alarm her. It is to catch strain early and route her safely."

2:10–2:35 · AI and safety
"Two layers. A deterministic rules engine decides the state. It is traceable, auditable, and never invents a diagnosis. A language model sits on top with one job: explain the state and the next step in plain English. AI makes the system understandable. It does not make the clinical decision."

2:35–3:00 · Close
"For students, BodyCheck means less guessing. For universities, the same engine runs across a cohort, so strain gets spotted earlier across the student population, before pressure becomes crisis.
In this hackathon we built the frontend, the rules engine, the API layer, and the simulated wearable datasets. The next step is clinical review of the red-flag protocol and a pilot with a university wellbeing service.
BodyCheck is not a medical device. It turns silent signals into an earlier route to help."