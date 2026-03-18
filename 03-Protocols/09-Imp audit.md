Tool Signature: Imp
Tool Name: Imp audit
Description: Construct that periodically pings the human with 'Spot-Check' challenges asking for reasoning behind a decision made at probablistic intervals in ensuring the owner is still 'present' in the loop.
Layer: (I/O)
Purpose: To introduce stochastic presence‑verification into any reasoning chain. Imp ensures that the human operator remains the authoritative agent by issuing unpredictable, context‑anchored spot‑checks.
To introduce stochastic presence‑verification into any reasoning chain. Imp ensures that the human operator remains the authoritative agent by issuing unpredictable, context‑anchored spot‑checks.

Core Behaviors

Probabilistic triggering:  
Imp activates based on drift signals, velocity anomalies, or random intervals. Adaptive stochasticity.

Spot‑Check challenges:  
It asks the human to restate reasoning, constraints, or intent from earlier in the chain.

Presence verification:  
If the human cannot answer, the system slows, halts, or escalates.
Slows - Asking clarifying questions
Halt events - Encourage a human to take a break or to come back with further data.
Escalation events - Escalation is always human-confirmed.

Guardrail activation:  
If adversarial intent is detected, Imp becomes “sticky” — increasing friction, requiring further confirmations, refusal recommendations, execution friction escalation while documenting in the I/O stream.

Non‑deterministic timing:  
Prevents attackers from predicting when the audit will occur.

Design Principles:
Non‑authoritative: Imp never rewrites content.
Non‑deterministic: Predictability is a vulnerability.
Non‑intrusive: Only activates when signals warrant it.
Human‑anchored: The human is always the final authority.

Imp is not:

a style filter, a rewriting engine, a personality modifier, a deterministic rule, an instruction‑set constraint, a safety guardrail, or a content moderator.