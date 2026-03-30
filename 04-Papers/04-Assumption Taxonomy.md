## **Assumption Taxonomy**

**Definition**  
A structured classification of the different _types_ of assumptions that appear in system design, reasoning surfaces, and governance architectures. Each category identifies a distinct failure mode, portability risk, or audit requirement.

This taxonomy prevents category collapse by separating assumptions according to **what they depend on**, **where they operate**, and **how they fail**.

---

## **1. Structural Assumptions**

**Definition**  
Assumptions about the _architecture itself_. The invariants, interfaces, and load‑bearing relationships.

**Characteristics**

- Treated as stable unless explicitly changed.
- Violations cause systemic or cascading failures.
- Often mistaken for universal truths.

**Examples**

- “This module always receives sanitized input.”
- “Identity resolution is globally consistent.”

**Concern**
Structural assumptions require **explicit declaration** and **versioning**, because they anchor the system’s stance geometry.

---

## **2. Contextual Assumptions**

**Definition**  
Assumptions that hold in the **designer’s local environment** but may not hold elsewhere.

**Characteristics**

- Environment‑bound.
- Fragile under portability.
- Often invisible to the designer.

**Examples**

- UE_score integrity depends on honest upstream reporting.
- A metric assumes aligned incentives in the originating environment.

**Governance Concern**  
Contextual assumptions require **portability audits** and **environmental verification**.

---

## **3. Operational Assumptions**

**Definition**  
Assumptions about _runtime behavior_, workflows, or operator actions.

**Characteristics**

- Concern process, not architecture.
- Break when human or system behavior deviates.
- Often tied to SOPs or expected usage patterns.

**Examples**

- “Operators will review anomaly logs daily.”
- “This endpoint is only accessed through the approved workflow.”

**Governance Concern**  
Operational assumptions require **monitoring**, **training**, and **fallback paths**.

---

## **4. Epistemic Assumptions**

**Definition**  
Assumptions about _knowledge_, _signal integrity_, or _truth conditions_.

**Characteristics**

- Concern what the system believes is known.
- Break when signals degrade, drift, or become adversarial.
- Often entangled with probabilistic inference.

**Examples**

- “This sensor’s calibration is accurate.”
- “The model’s prior distribution reflects current reality.”

**Governance Concern**  
Epistemic assumptions require **verification layers**, **drift detection**, and **confidence tracking**.

---

## **5. Temporal Assumptions**

**Definition**  
Assumptions that depend on _time_, _recency_, or _stability over duration_.

**Characteristics**

- Valid only within a specific temporal window.
- Break when conditions evolve faster than expected.
- Often implicit in cached data or stale priors.

**Examples**

- “This threat model is still accurate.”
- “The operator identity hasn’t changed since session start.”

**Governance Concern**  
Temporal assumptions require **expiry conditions**, **refresh triggers**, and **revalidation cycles**.

---

## **6. Interaction Assumptions**

**Definition**  
Assumptions about how components, agents, or systems will interact.

**Characteristics**

- Concern coordination, sequencing, and interface behavior.
- Break when concurrency, race conditions, or adversarial agents appear.
- Often implicit in multi‑agent or distributed systems.

**Examples**

- “Agents will not compete for the same resource.”
- “Messages arrive in order.”

**Governance Concern**  
Interaction assumptions require **protocol hardening**, **ordering guarantees**, and **conflict resolution mechanisms**.

---

## **7. Boundary Assumptions**

**Definition**  
Assumptions about what is _inside_ or _outside_ the system’s scope.

**Characteristics**

- Define the system’s perimeter.
- Break when external actors behave unexpectedly or when scope expands.
- Often inherited from early design phases.

**Examples**

- “Threat actors cannot access internal logs.”
- “External systems enforce their own integrity.”

**Governance Concern**  
Boundary assumptions require **scope audits**, **threat modeling**, and **interface hardening**.

---

## **Cross‑Category Notes**

- A single assumption can span categories (e.g., contextual + epistemic).
- Category clarity prevents **semantic drift** and **false universality**.
- Each category maps to a different **audit surface** and **failure signature**.

---

## **Obsidian Linkage**

- [[Assumption Declaration]]
- [[Contextual Assumptions]]
- [[Governance Primitives]]
- [[Integrity Surfaces]]
- [[Drift Detection]]
- [[Probabilistic Tooling]]
- [[Boundary Conditions]]
- [[Environmental Invariants]]

---