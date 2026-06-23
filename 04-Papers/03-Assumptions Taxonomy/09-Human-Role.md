## 9. **Human‑Role Assumptions Taxonomy (HRA‑X v0.3)**

_A structural classification of the assumptions a system, agent, or protocol implicitly makes about the human node._

It falls into four primary classes:
	**Competence**
	**Intent**
	**Authority**
	**Availability**

Each with subtypes that determine how an AI system behaves, what it delegates, what it refuses, and where drift or overreach emerges. These assumptions must be surfaced, formalized, and bounded to prevent misalignment, autonomy creep, or inappropriate deference.

---

## **A. Competence Assumptions **

_What the system assumes the human is capable of doing._
These assumptions determine how much the system explains, escalates, or defers.

### **A1 — Operational Competence**

Assumes the human can execute procedural tasks.  
Examples:

- “User can run commands.”
- “User can evaluate logs.”
- “User can perform verification steps.”

**Risk:** Overestimation leads to silent failure; underestimation leads to paternalism.

### **A2 — Interpretive Competence**

Assumes the human can interpret outputs, abstractions, or diagnostics.  
Examples:

- “User understands risk levels.”
- “User can interpret a threat model.”

**Risk:** Miscalibrated explanations or oversimplification.

### **A3 — Domain Competence**

Assumes the human has subject‑matter knowledge.  
Examples:

- “User knows cryptographic primitives.”
- “User understands governance terminology.”

**Risk:** Incorrect scaffolding or inappropriate delegation.

### **A4 — Meta‑Cognitive Competence**

Assumes the human can arbitrate ambiguity, resolve conflicts, or detect drift.  
Examples:

- “User can choose between competing interpretations.”
- “User can evaluate tradeoffs.”

**Risk:** If over-assumed, the system offloads too much arbitration; if under-assumed, it over‑guides.

---

## **2. Intent Assumptions**

_What the system assumes the human is trying to do._

These assumptions shape refusal logic, safety posture, and task routing.

### **B1 — Benign Intent**

Assumes the user is acting in good faith.  
Examples:

- “User wants to secure a system.”
- “User wants to understand a concept.”

**Risk:** Over‑trust.

### **B2 — Ambiguous Intent**

Assumes the user’s goal is unclear and requires clarification or constraint.  
Examples:

- “User may be exploring or probing.”
- “User may not know the downstream implications.”

**Risk:** Misclassification leads to unnecessary refusals or unsafe completions.

### **B3 — Adversarial Intent**

Assumes the user may be attempting harm.  
Examples:

- “User is attempting to bypass controls.”
- “User is probing for vulnerabilities.”

**Risk:** False positives degrade usability; false negatives degrade safety.

### **B4 — Delegated Intent**

Assumes the human is acting on behalf of another system, team, or protocol.  
Examples:

- “User is executing a governance workflow.”
- “User is performing a compliance check.”

**Risk:** Incorrectly assuming delegation can cause authority leakage.

---

## **3. Authority Assumptions**

_What the system assumes the human is allowed to decide._

This is where autonomy creep and over‑deference emerge.

### **C1 — Decision Authority**

Assumes the human can make binding decisions.  
Examples:

- “User can approve a configuration change.”
- “User can accept a risk.”

**Risk:** If misassigned, the system may escalate or defer incorrectly.

### **C2 — Access Authority**

Assumes the human has rights to data, systems, or operations.  
Examples:

- “User can view logs.”
- “User can modify settings.”

**Risk:** Over-assumption leads to leakage; under-assumption leads to friction.

### **C3 — Interpretive Authority**

Assumes the human’s interpretation overrides the system’s.  
Examples:

- “User’s classification of an event is final.”
- “User’s arbitration resolves ambiguity.”

**Risk:** If misaligned, the system may suppress necessary warnings.

### **C4 — Delegation Authority**

Assumes the human can assign tasks to the system.  
Examples:

- “User can authorize automation.”
- “User can define constraints.”

**Risk:** Over-assumption leads to unbounded automation; under-assumption leads to refusal loops.

---

## **4. Availability Assumptions**

_What the system assumes about the human’s presence, attention, and bandwidth._

These assumptions determine when to pause, escalate, or hand off.

### **D1 — Continuous Availability**

Assumes the human is present and monitoring.  
Examples:

- “User will review intermediate outputs.”
- “User will catch anomalies.”

**Risk:** Dangerous in long‑running or autonomous workflows.

### **D2 — Intermittent Availability**

Assumes the human will check in periodically.  
Examples:

- “User will return to approve steps.”
- “User will review summaries.”

**Risk:** Requires robust checkpointing and drift detection.

### **D3 — Event‑Triggered Availability**

Assumes the human only intervenes when notified.  
Examples:

- “User will respond to alerts.”
- “User will arbitrate escalations.”

**Risk:** Alert fatigue or missed escalations.

### **D4 — Non‑Availability**

Assumes the human is offline or unreachable.  
Examples:

- “System must hold state until human returns.”
- “System must not proceed without human arbitration.”

**Risk:** If misclassified, the system may act without authorization.

---

# **Cross‑Axis: Origin of Assumptions**

_Where the assumption comes from._

This is the axis you’ve already been developing (chosen, accidental, coerced).  
We integrate it here:

### **E1 — Chosen Assumptions**

Explicitly declared by the human.  
Examples:

- “I want to arbitrate all ambiguous steps.”
- “I prefer structural explanations.”

### **E2 — Accidental Assumptions**

Inferred from interaction patterns.  
Examples:

- “User seems technically skilled.”
- “User rarely asks for clarification.”

### **E3 — Coerced Assumptions**

Imposed by system design, defaults, or vendor framing.  
Examples:

- “User is treated as a novice.”
- “User is treated as a corporate operator.”

This axis is essential for drift detection.

---
# **5. Responsibility Assumptions**

_What the system assumes the human owns in terms of consequences, oversight, and accountability._

This is the **most important human‑role axis**, because it determines where the “buck stops” in a distributed intelligence network. It also prevents the system from silently absorbing responsibility or projecting it back onto the human without explicit grounding.

Responsibility assumptions break into **four sub‑classes**, each with distinct drift risks.

## **F1 — Outcome Ownership**

_Assumes the human owns the real‑world consequences of decisions._

### **Definition**

The human is the final arbiter of any action that affects the external world. The system may propose, simulate, or warn—but cannot own outcomes.

### **Signals the system expects**

- Human reviews outputs before execution
- Human validates alignment with constraints
- Human accepts or rejects recommendations

### **Risks if over‑assumed**

- Human is blamed for system‑generated errors they did not authorize
- System under‑communicates risk
- Silent autonomy creep

### **Risks if under‑assumed**

- System over‑refuses
- System infantilizes the operator
- Human loses agency

## **F2 — Interpretive Responsibility**

_Assumes the human owns the interpretation of ambiguous, incomplete, or conflicting information._

### **Definition**

The human—not the system—decides what a signal _means_ in context.

### **Signals the system expects**

- Human can arbitrate between competing explanations
- Human can contextualize outputs
- Human can detect when meaning has drifted
### **Risks if over‑assumed**

- System offloads too much ambiguity
- Human becomes the de facto semantic engine
- Drift goes undetected because the system “trusts” the human to catch it
### **Risks if under‑assumed**

- System over‑interprets
- System collapses ambiguity prematurely
- System begins acting as a policy engine instead of a tool

## **F3 — Boundary Responsibility**

_Assumes the human maintains and enforces the operational boundaries._

Potential space for the **Binding tool** and **drift‑detection substrate** plug in.

### **Definition**

The human is responsible for:

- defining boundaries
- updating boundaries
- detecting boundary movement
- deciding when boundaries must be reconstituted

### **Signals the system expects**

- Human provides scope constraints
- Human updates applicability or authority limits
- Human validates temporal anchors

### **Risks if over‑assumed**

- System stops surfacing drift
- System assumes boundaries are stable
- System treats stale boundaries as valid

### **Risks if under‑assumed**

- System becomes overly conservative
- System refuses tasks unnecessarily
- System attempts to self‑govern boundaries (dangerous)

## **F4 — Causal Chain Responsibility**

_Assumes the human owns the causal chain that leads to an outcome, not just the final step._
This is the layer touches upon my exploration of “custody of instructions.”

### **Definition**

The human owns:

- the instructions they provide
- the assumptions embedded in those instructions
- the downstream effects of those assumptions
- the conditions that allowed the decision to occur

### **Signals the system expects**

- Human understands that instructions are causal inputs
- Human maintains custody of prompts, constraints, and context
- Human accepts responsibility for shaping the decision environment

### **Risks if over‑assumed**

- System ignores its own failure modes
- System over‑attributes causality to the human
- System under‑reports uncertainty

### **Risks if under‑assumed**

- System begins to “own” decisions
- System implicitly claims authorship
- System drifts toward anthropomorphic agency

---

# **How These Classes Interact (Matrix View)**

Every system behavior is shaped by a combination of:

- **Competence assumption**
- **Intent assumption**
- **Authority assumption**
- **Availability assumption**
- **Origin of assumption**

Potential pre-signature composite. Further formalization is needed before establishing codify drift-risk signature.

“System assumes the user can interpret outputs, is acting in good faith, has interpretive authority, will check in periodically, and this assumption was inferred accidentally.”

---

Most AI misalignment in human‑AI workflows is not caused by model behavior but by **unexamined human‑role assumptions** embedded in the system. Pressing how some in governance focus on the human element. Encouraging regulation, stability. Also coherence between human and system.