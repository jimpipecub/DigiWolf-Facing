**Definition:**  
A failure mode in probabilistic systems where the model detects a familiar structural pattern in the input and completes toward the _strongest_ or most canonical version of that pattern, regardless of the user’s actual scope, constraints, or operational reality.

**Mechanism:**

- Triggered by high‑salience architectural or conceptual keywords
- Driven by latent‑space attractors (actor model, microservices, CQRS, etc.)
- Occurs when constraints are missing or ambiguous
- Amplified when the operator lacks domain mastery to resist the continuation

**Symptoms:**

- Over‑engineered architectural suggestions
- Solutions that are elegant but operationally misaligned
- Locally coherent but globally inappropriate structures
- Increased system complexity without corresponding benefit

**Risk Profile:**

- Shifts complexity to the operator without warning
- Creates hidden operational debt
- Encourages premature abstraction
- Masks itself as “smart” or “best practice”

**Mitigation:**

- Explicit operator profiles
- Constraint‑first prompting
- Deterministic shells around probabilistic cores
- Refusal matrices for out‑of‑scope architectural suggestions
- Epistemic sharding to prevent pattern escalation

**Relation to Completion Bias:**

- Completion bias determines the _trajectory_ of the continuation
- Pattern‑matching overshoot determines the _magnitude_ of the pattern applied

---