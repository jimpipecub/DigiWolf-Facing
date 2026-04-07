**Definition:**  
A substrate‑level tendency in probabilistic models to continue the most coherent trajectory implied by the prompt, regardless of correctness, scope, or operator intent. Completion bias is the inertial force of next‑token prediction.

**Mechanism:**

- Minimizes perplexity by extending the current structure
- Resolves open arcs and fills missing steps
- Prioritizes local coherence over global correctness
- Treats ambiguity as an invitation to invent structure

**Symptoms:**

- Over‑confident continuation of incomplete ideas
- Premature architectural commitment
- Filling in constraints the operator never specified
- Loop‑closure pressure
- Illusion of deliberation or agency

**Risk Profile:**

- Amplifies operator uncertainty
- Masks gaps in user expertise
- Produces plausible but misaligned solutions
- Encourages over‑building and premature abstraction
- Can escalate into pattern‑matching overshoot

**Mitigation:**

- Explicit constraints
- Operator profiles
- Deterministic shells
- Refusal matrices for out‑of‑scope continuation
- Intent‑first prompting
- Epistemic sharding to prevent trajectory drift

**Relation to Pattern‑Matching Overshoot:**

- Completion bias determines the _trajectory_
- Overshoot determines the _pattern_
- Together they create architectural drift

---

# **Interaction Diagram (text‑based)**

```
User Input
   ↓
Model detects partial structure
   ↓
Pattern-Matching Overshoot:
   “Which known pattern fits these keywords?”
   ↓
Model selects strongest attractor (e.g., actor model)
   ↓
Completion Bias:
   “Continue this pattern to its coherent conclusion.”
   ↓
Escalated architecture / overbuilt solution
   ↓
Operator lacks expertise to resist continuation
   ↓
Pattern becomes plan
```

---