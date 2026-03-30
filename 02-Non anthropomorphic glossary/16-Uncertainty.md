**Uncertainty (U)** quantifies the degree of _epistemic_, _systemic_, and _governance_ drift within an AI system by measuring gaps, ambiguities, or unencoded differentiations in the system’s operational manifold. It reflects the system’s **information‑encoding capacity** about its own state, predictions, or decisions—without implying subjective confidence or internal belief.

This keeps U grounded in:

- structure
- encoding
- drift
- measurable gaps

No “confidence,”
No “belief,”
No “self‑assessment.”

---

# **Three Components of Uncertainty (U)**

## 1. **Epistemic Uncertainty**

Uncertainty arising from **unencoded relational differentiations**.

Examples:

- missing constraints
- incomplete baselines
- insufficiently specified roles
- ambiguous context signals

This is uncertainty due to _lack of encoded knowledge_, not “the model being unsure.”

---

## 2. **Systemic Uncertainty**

Uncertainty arising from **inherent system variability**.

Examples:

- stochastic sampling
- non‑deterministic execution paths
- multi‑model divergence
- distributional noise

This is the probabilistic interior of the system.

---

## 3. **Governance Uncertainty**

Uncertainty arising from **ambiguous, incomplete, or conflicting operational policies**.

Examples:

- unclear escalation rules
- overlapping role definitions
- missing invariants
- undefined behavior for edge cases

This is uncertainty in the **deterministic exterior**, not the model.

---

# **Structural Properties of U**

### **1. U is a Measure of Encoding Completeness**

High U = the system lacks sufficient encoded structure to map the current situation into a stable operational region.

### **2. U is a Drift Signal**

U increases when:

- baselines degrade
- invariants weaken
- context becomes ambiguous
- role boundaries blur

It’s a _governance‑layer metric_, not a psychological one.

### **3. U is Orthogonal to Anomaly**

- **Anomaly (A)** = deviation from what _is_ encoded
- **Uncertainty (U)** = gaps in what _should be_ encoded

A system can have:

- low A, low U - Stable, well-governed, target operational state.
- high A, low U - clear rules, clear violation
- low A, high U - no rules, nothing to violate, silent failure
- high A, high U - violations detected but resolution ambiguous, noisy, hard to triage

This distinction is crucial in the architecture.

### **4. U is Non‑Anthropomorphic by Design**

U never means:

- confidence
- belief
- doubt
- hesitation

It is strictly about **information encoding and structural completeness**.

---

# **Operational Definition (Compact Version)**

**Uncertainty (U)** measures the degree to which an AI system lacks sufficient encoded structure—epistemic, systemic, or governance—to deterministically map its current state, inputs, or tasks into stable operational behavior.

Note: High governance uncertainty means the uncertainty score itself is less reliable.