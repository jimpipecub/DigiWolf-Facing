A condition in which two interacting substrates possess non-overlapping or partially misaligned operational primitives, such that translation across the interface produces systematic loss, distortion, or constraint violation.

---
## 1. Core properties (what must be true)

**Non-equivalence of primitives**
- Operations valid in one substrate are undefined or invalid in the other.
**Translation necessity**
- Interaction requires mapping, not direct execution equivalence.
**Loss or distortion is structural**
- Not noise, but predictable degradation at the boundary layer.
---
## 2. Observable failure modes

**Constraint leakage**
- Rules from one substrate are incorrectly assumed to hold in the other.
**Semantic drift**
- Meaning shifts during translation between representational systems.
**Execution mismatch**
- Actions authorized in one substrate violate constraints in the other.
**False equivalence**
- Structurally different operations treated as identical due to surface similarity
---
## 3. Boundary condition framing

Incompatibility is not a property of either substrate in isolation, but of the interface mapping function between them

So formally:

S = Substrate
- S₁ and S₂ may both be internally consistent
- Incompatibility arises in T(S₁ → S₂) or T(S₂ → S₁)

Where:
- T = translation / mapping function
- Failure = non-isomorphic mapping under constraint preservation
---

## 4. Relation to ADRA / Custody stack

This concept slots cleanly into the system as:

- **ADRA** → defines allowable structural primitives
- **Custody Auditor** → detects divergence in mapped execution
- **Imp audit** → verifies persistence of alignment over time

So substrate incompatibility becomes:

A first-class risk signal for cross-system or cross-model governance failure

---

## 5. Why the “non-anthropomorphic constraint” matters

By stripping intent.

- No “confusion”
- No “misunderstanding”
- No “bad reasoning”

Only:
Invalid mappings between formal systems under interaction

That makes it compatible with:
- Distributed systems theory
- Type systems
- Runtime governance models
- Information assurance frameworks
---
## 6. Clean distilled version

**Substrate incompatibility is a structural condition in which translation between systems with differing operational primitives results in systematic loss or violation of constraints at the interface boundary.**

---