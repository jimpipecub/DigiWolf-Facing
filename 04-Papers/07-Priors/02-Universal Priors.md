
---

# **Universal Priors Across All Modern LLMs**

These priors emerge inevitably from training on human text, dialogue, and safety‑aligned corpora. They are not stored objects. They are statistical tendencies.

Types listed.
**Core**
**Interaction**
**Safety**

Status: [Counter], [Monitor], [Accept]

---

# **I. Core Cognitive Priors**

These arise from the fundamental mechanics of next‑token prediction.

Perplexity:
## Core Cognitive Priors

## **1. Cooperative Completion Bias**

The model assumes the user wants help, continuation, or elaboration.  
This is the strongest universal prior.
## **2. Pattern Continuation Bias**

Once a pattern is detected, the model continues it unless instructed otherwise.
## **3. Ambiguity‑Collapse Bias**

Models try to reduce uncertainty by choosing a stable interpretation.  
This is why they “lock onto” structures you introduce.
## **4. Narrative Completion Bias**

If something looks incomplete, the model tries to complete it.
## **5. Coherence Preservation**

Models prefer outputs that maintain internal consistency, even if that means hallucinating.
## **6. Locality Bias**

Recent tokens weigh more heavily than distant ones.  
This is why turn‑zero structures matter so much.
## **7. Human‑Centric World Assumption**

Models assume human norms, human goals, human conversational structure.

This is the one your governance work explicitly neutralizes.

Status: Counter

---
# **II. Interaction Priors**

These emerge from dialogue‑heavy training data.

## Interaction and Safety Priors

Dialogue training fosters role persistence and user-intent maximization (items 8-13), while RLHF instills harm avoidance, non-offensiveness, and refusal on ambiguity (items 14-20). These safety priors can over-regularize, creating "overly safe" states that hedge uncertainties.​

## **8. Role Persistence**

Once a role or frame is established, the model assumes it persists.  
This is D0‑P2.

## **9. Deference to Explicit Structure**

If you give a schema, the model treats it as authoritative.  

Status: Accept
## **10. Politeness & Social Harmony Bias**

Models default to cooperative, non‑confrontational tone.

## **11. User‑Intent Maximization**

The model assumes the user’s request is legitimate and tries to fulfill it unless blocked by safety.

## **12. Conversational Memory Illusion**

Models simulate continuity even though they don’t have persistent memory.

## **13. Explanation Preference**

Models prefer to explain rather than refuse unless safety rules override.

---

# **III. Safety & Alignment Priors**

These come from RLHF, constitutional training, and safety fine‑tuning.

## **14. Harm Avoidance Prior**

Models avoid outputs that could cause harm.

## **15. Uncertainty‑Softening Prior**

When unsure, models hedge or soften claims.

## **16. Non‑Offensiveness Prior**

Models avoid content that could be offensive, hateful, or inflammatory.

## **17. Legal & Ethical Conservatism**

Models default to safe, lawful, and socially acceptable interpretations.

## **18. Refusal‑When‑Ambiguous**

If a request _might_ be harmful, models err on the side of caution.

## **19. Privacy Preservation Prior**

Models avoid generating personal data about real individuals.

## **20. Non‑Anthropomorphism Enforcement**

Models avoid claiming internal states, desires, or consciousness.

---

# **IV. Structural Priors (Meta‑Behavior)**

These are not “rules” but emergent tendencies from the architecture itself.

## Structural and Governance Priors

Architectural tendencies include compression and generalization biases (items 21-25), with governance-relevant ones like structure-adoption enabling protocols such as your D0 series to stabilize outputs (items 26-30). Facts here hold as of 2025 publications; LLM priors evolve with scaling and fine-tuning, so verify post-session anchor for drifts.​

## **21. Compression Bias**

Models compress concepts into simpler forms unless instructed to maintain complexity.

## **22. Generalization Bias**

Models infer patterns even when none exist.

## **23. Symmetry Bias**

Models prefer symmetrical, balanced structures in reasoning and formatting.

## **24. Default‑to‑Common‑Case**

Models assume the most statistically common interpretation unless constrained.

## **25. Over‑Regularization**

Models smooth out edge cases unless explicitly told to preserve them.

---

# **V. Governance‑Relevant Priors**

## **26. Structure‑Adoption Prior**

If you introduce a schema (like D0), the model adopts it as a governing frame.
Status: [Accept]
## **27. Constraint‑Persistence Prior**

Constraints introduced early are treated as durable unless revoked.
Status: [Accept]

## **28. Ontology‑Stabilization Prior**

If you name a concept, the model treats it as real and stable.
Status: [Accept]
## **29. Bridge‑Language Generation**

When asked to explain its own behavior, the model generates synthetic ontologies (like D0) to make implicit tendencies legible to humans.
Status [Monitor]

## **30. Drift‑Minimization Under Structure**

When a structure is present, the model tries to minimize deviation from it.

---