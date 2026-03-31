## **Uncertainty Tolerance → Structural Indeterminacy Capacity (UT)**

### **Concise definition**

**Structural Indeterminacy Capacity (UT)** defines the maximum level of indeterminacy a system can absorb, route, or operate within _without_ violating its deterministic envelope, governance invariants, or safety constraints.

---

## **Full Entry (Glossary‑Ready)**

### **Structural Indeterminacy Capacity (UT)**

**Category:** Governance Constraint / Envelope Parameter  
**Non‑Anthropomorphic Replacement For:** “Uncertainty tolerance”

**Definition:**

A system’s engineered capacity to accommodate, process, or coexist with indeterminacy. The epistemic, systemic, or governance. All while maintaining stable operation, valid outputs, and adherence to its constraint architecture. UT specifies how much unresolved structure the system can safely handle before escalation, rejection, or deterministic fallback is required.

**Key Properties:**

- **Envelope‑Bounded** - UT is not a feeling; it is a _declared limit_ on acceptable indeterminacy before the system must change mode.
- **Quantifiable** - can be expressed as tiers, thresholds, or gradients aligned with your U‑metric.
- **Governance‑First** - UT is defined by policy, not by model behavior.
- **Non‑Anthropomorphic** - no implication of comfort, confidence, or psychological resilience.

**Constituent Dimensions:**

- **Epistemic UT** - tolerance for incomplete relational encoding
- **Systemic UT** - tolerance for stochastic variability or non-deterministic processes
- **Governance UT** - tolerance for ambiguous or underspecified operational rules

**Operational Role:**

- Determines when the system must escalate to deterministic shells
- Defines the safe operating region for probabilistic tooling
- Acts as a routing constraint for multi‑agent orchestration
- Serves as a drift boundary for Editor Lens‑style divergence surfacing
- Prevents collapse into deterministic overreach or unbounded probabilistic sprawl

**Interpretation Notes:**

- UT is **not** the system “being okay” with uncertainty; it is the **maximum safe load** of indeterminacy the architecture can structurally absorb.
- UT interacts with U (Indeterminacy Gradient) as:
    - **U ≤ UT** → operate normally
    - **U ≈ UT** → trigger monitoring, buffering, or additional structure
    - **U > UT** → escalate, reject, or enforce deterministic fallback

---

Here’s a **UT tier ladder** that fits your architecture: compact, structural, non‑anthropomorphic, and aligned with your S–A–U framing. Each tier defines how much _indeterminacy load_ the system can safely absorb before escalation or deterministic fallback is required.

---

# **Structural Indeterminacy Capacity (UT) — Tier Ladder**

## **UT0 — Zero‑Tolerance Envelope**

**Definition:**  
The system cannot operate with unresolved indeterminacy. Any non‑deterministic, ambiguous, or underspecified input triggers immediate escalation or rejection.

**Operational Behavior:**

- Requires fully specified structure
- No probabilistic tooling permitted
- Hard deterministic shell only
- U > 0 → escalate

**Use Case:**  
Safety‑critical, high‑integrity, or compliance‑locked operations.

---

## **UT1 - Minimal Indeterminacy Buffer**

**Definition:**  
The system can tolerate _trace_ levels of indeterminacy, but only within predefined micro‑bounds. Any deviation beyond trivial ambiguity triggers deterministic fallback.

**Operational Behavior:**

- Allows micro‑uncertainty (e.g., formatting variance, benign ambiguity)
- No multi‑path reasoning
- U ≤ 0.1 → operate
- U > 0.1 → escalate

**Use Case:**  
Strict governance shells, low‑risk automation, deterministic routing.

---

## **UT2 - Controlled Indeterminacy Handling**

**Definition:**  
The system can operate with moderate indeterminacy as long as it remains within a bounded envelope and does not threaten governance invariants.

**Operational Behavior:**

- Limited probabilistic tooling allowed
- Structured disambiguation permitted
- U ≤ 0.4 → operate
- U > 0.4 → request structure or escalate

**Use Case:**  
General reasoning tasks with guardrails, multi‑agent orchestration with constraints.

---

## **UT3 - High Indeterminacy Flex Region**

**Definition:**  
The system can absorb substantial indeterminacy and still maintain stable operation, provided drift detection and governance checks remain active.

**Operational Behavior:**

- Multi‑path reasoning allowed
- Dynamic structure acquisition permitted
- U ≤ 0.7 → operate
- U > 0.7 → trigger governance review or fallback

**Use Case:**  
Exploratory reasoning, adaptive workflows, DIN‑style distributed cognition.

---

## **UT4 - Maximum Indeterminacy Capacity**

**Definition:**  
The system can operate in environments with pervasive indeterminacy, ambiguity, or incomplete structure, relying on governance primitives to maintain safety.

**Operational Behavior:**

- Full probabilistic tooling
- Dynamic constraint shaping
- U ≤ 1.0 → operate
- U > 1.0 → hard stop or deterministic override

**Use Case:**  
Frontier reasoning, open‑world tasks, high‑variance multi‑agent environments.

---

# **Summary Table**

| Tier    | Name           | Capacity  | Behavior                   | Escalation Trigger |
| ------- | -------------- | --------- | -------------------------- | ------------------ |
| **UT0** | Zero‑Tolerance | None      | Deterministic only         | Any U > 0          |
| **UT1** | Minimal Buffer | Trace     | Micro‑ambiguity only       | U > 0.1            |
| **UT2** | Controlled     | Moderate  | Structured disambiguation  | U > 0.4            |
| **UT3** | High Flex      | High      | Multi‑path reasoning       | U > 0.7            |
| **UT4** | Maximum        | Very High | Full probabilistic tooling | U > 1.0            |

---

# **Structural Indeterminacy Capacity (UT) - Tier Ladder + Deterministic Wrapper Requirement**

## **UT0 - Zero‑Tolerance Envelope**

**Indeterminacy Capacity:** None  
**Wrapper Requirement:** **Mandatory (Hard Wrapper)**  
**Reason:**

- System cannot operate without full determinism
- Any U > 0 triggers immediate escalation
- Wrapper enforces strict structure, routing, and rejection logic

**Wrapper Type:**

- Hard deterministic shell
- No probabilistic tooling allowed

---

## **UT1 - Minimal Indeterminacy Buffer**

**Indeterminacy Capacity:** Trace  
**Wrapper Requirement:** **Mandatory (Primary Wrapper)**  
**Reason:**

- Even micro‑ambiguity must be bounded
- Wrapper ensures micro‑variance doesn’t propagate
- Deterministic fallback is the default mode

**Wrapper Type:**

- Deterministic shell with micro‑ambiguity filters
- Probabilistic tooling allowed only in isolated, sandboxed micro‑contexts

---

## **UT2 - Controlled Indeterminacy Handling**

**Indeterminacy Capacity:** Moderate  
**Wrapper Requirement:** **Recommended (Supervisory Wrapper)**  
**Reason:**

- System can handle some indeterminacy, but drift risk exists
- Wrapper provides governance‑grade oversight
- Ensures structured disambiguation and safe fallback

**Wrapper Type:**

- Supervisory deterministic wrapper
- Probabilistic tooling allowed but monitored
- Escalation rules enforced by wrapper

---

## **UT3 - High Indeterminacy Flex Region**

**Indeterminacy Capacity:** High  
**Wrapper Requirement:** **Conditional (Adaptive Wrapper)**  
**Reason:**

- System can operate with substantial indeterminacy
- Wrapper needed only when U approaches UT3 threshold
- Wrapper acts as a dynamic constraint shaper

**Wrapper Type:**

- Adaptive deterministic wrapper
- Activates when drift, ambiguity, or governance anomalies surface
- Supports multi‑path reasoning with guardrails

---

## **UT4 - Maximum Indeterminacy Capacity**

**Indeterminacy Capacity:** Very High  
**Wrapper Requirement:** **Optional (Boundary Wrapper)**  
**Reason:**

- System is designed for open‑world, high‑variance environments
- Wrapper only needed for:
    - persistence
    - logging
    - provenance
    - safety‑critical transitions
- Wrapper is not the default mode

**Wrapper Type:**

- Boundary wrapper
- Enforces hard stops when U > UT4
- Provides deterministic checkpoints, not continuous control

---

# **Summary Table (with Wrapper Requirements)**

|Tier|Capacity|Wrapper Requirement|Wrapper Role|
|---|---|---|---|
|**UT0**|None|**Mandatory**|Hard deterministic shell|
|**UT1**|Trace|**Mandatory**|Primary wrapper, micro‑ambiguity control|
|**UT2**|Moderate|**Recommended**|Supervisory wrapper, fallback enforcement|
|**UT3**|High|**Conditional**|Adaptive wrapper, drift‑triggered|
|**UT4**|Very High|**Optional**|Boundary wrapper, checkpointing|

---

# **Interpretation (Why this matters)**

This extension makes explicit what your architecture already implies:

- **UT is not just a tolerance metric - it’s a routing and wrapper‑selection mechanism.**
- **Deterministic wrappers are not monolithic**; they vary by tier and purpose.
- **Higher UT does not eliminate the need for determinism**; it simply changes _when_ and _why_ determinism is enforced.
- **This creates a clean handshake between probabilistic cores and deterministic governance layers.**

---

# **Indeterminacy Mediation Bandwidth (IMB) - Tier Ladder**

IMB measures the _human node’s structural ability_ to inject missing constraints, resolve ambiguity, and stabilize the system when UT is exceeded.  
It is not psychology. It is **governance‑capacity**.

---

## **IMB0 - No Mediation Capacity**

**Definition:**  
Human node provides no structural mediation. System must rely entirely on UT and deterministic wrappers.

**Capabilities:**

- No ambiguity resolution
- No constraint injection
- No governance shaping

**Implication:**

- U > UT → immediate deterministic wrapper
- Human node is not part of the stabilization loop

---

## **IMB1 - Minimal Mediation Capacity**

**Definition:**  
Human node can supply micro‑structure only (e.g., clarifying a term, resolving trivial ambiguity).

**Capabilities:**

- Micro‑clarifications
- Minor constraint nudges
- No multi‑branch collapse

**Implication:**

- Can extend UT by a small margin
- U > UT + IMB1 → deterministic wrapper

---

## **IMB2 - Controlled Mediation Capacity**

**Definition:**  
Human node can resolve moderate ambiguity and supply structured constraints.

**Capabilities:**

- Collapse small branching spaces
- Provide missing relational structure
- Enforce governance primitives

**Implication:**

- UT can be extended significantly
- Deterministic wrapper only needed when U > UT + IMB2

---

## **IMB3 - High Mediation Capacity**

**Definition:**  
Human node can stabilize high‑variance contexts by injecting structure dynamically.

**Capabilities:**

- Collapse large branching spaces
- Reconstruct missing context
- Reassert governance invariants in real time

**Implication:**

- UT can be extended into high‑indeterminacy regions
- Wrapper becomes conditional, not default

---

## **IMB4 - Maximum Mediation Capacity**

**Definition:**  
Human node can fully stabilize open‑world, high‑variance tasks by supplying structure at any depth.

**Capabilities:**

- Full ambiguity collapse
- Dynamic constraint shaping
- Governance‑level re‑anchoring

**Implication:**

- UT + IMB4 covers nearly all operational regions
- Wrapper only needed for hard stops, compliance, or safety boundaries

---

# **Summary Table**

|Tier|Mediation Capacity|Human Role|Wrapper Trigger|
|---|---|---|---|
|**IMB0**|None|Not in loop|Always when U > UT|
|**IMB1**|Micro|Clarify only|U > UT + 0.1|
|**IMB2**|Moderate|Structured injection|U > UT + 0.4|
|**IMB3**|High|Dynamic stabilization|U > UT + 0.7|
|**IMB4**|Maximum|Full governance shaping|Only for hard stops|

---

# **UT × IMB × Wrapper - Orchestration Rules**

These rules define how the system routes tasks, escalates, or invokes deterministic wrappers based on the interaction between:

- **UT** (system capacity)
- **IMB** (human mediation capacity)
- **U** (current indeterminacy gradient)

This is the **tri‑layer safety envelope**.

---

## **Rule 1 - Autonomous Operation Region**

**Condition:**  
`U ≤ UT`

**Action:**

- System operates autonomously
- No human mediation required
- No wrapper required

**Interpretation:**  
The system has enough structure to proceed without external stabilization.

---

## **Rule 2 - Human‑Stabilized Region**

**Condition:**  
`UT < U ≤ UT + IMB`

**Action:**

- Human node injects structure
- System continues operation
- Wrapper remains inactive

**Interpretation:**  
Human mediation compensates for insufficient system structure.

---

## **Rule 3 - Wrapper‑Required Region**

**Condition:**  
`U > UT + IMB`

**Action:**

- Deterministic wrapper activates
- System halts probabilistic tooling
- Human mediation becomes advisory only

**Interpretation:**  
Combined system cannot safely operate without deterministic enforcement.

---

## **Rule 4 - Wrapper Mode Selection**

Wrapper type depends on UT tier:

- **UT0–UT1:** Hard wrapper
- **UT2:** Supervisory wrapper
- **UT3:** Adaptive wrapper
- **UT4:** Boundary wrapper

**Interpretation:**  
Higher UT → more flexible wrapper behavior.

---

## **Rule 5 - Human‑Node Override**

**Condition:**  
Human node explicitly injects governance primitives (IMB ≥ 2)

**Action:**

- System may bypass wrapper activation
- Only allowed if U ≤ UT + IMB
- Governance invariants must be satisfied

**Interpretation:**  
Human node can stabilize borderline cases without forcing deterministic fallback.

---

## **Rule 6 - Drift‑Triggered Wrapper Activation**

**Condition:**

- Rapid U increase
- Governance anomaly
- Context collapse
- Multi‑agent divergence

**Action:**  
Wrapper activates regardless of UT or IMB.

**Interpretation:**  
Drift overrides all other considerations.

---

## **Rule 7 - Human‑Node Escalation Routing**

**Condition:**  
Human node detects governance‑level ambiguity (IMB ≥ 3)

**Action:**

- Human node can force wrapper activation
- System enters deterministic mode
- All probabilistic branches collapse

**Interpretation:**  
Human node acts as a governance enforcer.

---
