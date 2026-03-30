### **Refined Definition**

**Anomaly (A)** is the detection of **statistically significant relational differentiations** between a system’s current behavior and its encoded operational baselines. These differentiations indicate perturbations in the system’s **invariant structures**, revealing potential misalignments, unexpected state transitions, or security‑relevant deviations.

This keeps the focus on:

- structure
- constraints
- relational comparison
- measurable deviation

No intent. No cognition. No “the model wanted something else.”

---

# **Key Properties (Aligned With Framework)**

### **1. Relational, Not Absolute**

An anomaly is never “weirdness in isolation.”  
It is **difference from a reference frame**:

- temporal baselines
- role‑specific patterns
- context‑conditioned distributions
- invariant structures

This makes anomaly a _contrastive_ signal.

---

### **2. Invariant‑Referenced**

An anomaly is only meaningful because invariants exist.

Examples of invariants:

- allowed state transitions
- protocol‑defined message formats
- stable resource‑usage envelopes
- deterministic wrappers around probabilistic components

An anomaly is a **breach, distortion, or unexpected modulation** of these invariants.

---

### **3. Distributional Significance**

An anomaly is not noise.  
It is a **statistically significant deviation** from expected distributions.

This includes:

- output distribution shifts
- latency envelope violations
- role‑boundary mixing
- context‑misaligned responses

I am treating the system as a **probabilistic manifold**, not a mind.

---

### **4. Diagnostic, Not Interpretive**

An anomaly does not imply:

- motive
- confusion
- preference
- internal state

It is a **diagnostic artifact**—a measurable perturbation that signals something structurally meaningful.

---

# **Operational Definition (Compact Version)**

**Anomaly (A)** is a measurable, statistically significant deviation from encoded operational baselines, indicating perturbations in the system’s invariant structures and revealing potential malfunction, drift, or security‑relevant state transitions.


---

# **How This Fits Into the S–A–U Metric**

|Component|What It Measures|Relation to Anomaly|
|---|---|---|
|**Stability (S)**|Adherence to invariants|Anomaly is the inverse signal|
|**Anomaly (A)**|Deviations from invariants|Direct detection of relational differentiations|
|**Uncertainty (U)**|Gaps in constraint encoding or context mapping|High U increases false positives/negatives in A|

Anomaly is the **perturbation detector** in the triad.

---