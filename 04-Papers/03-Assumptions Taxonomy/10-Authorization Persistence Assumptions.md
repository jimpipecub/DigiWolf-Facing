# Authority Assumption: A Governance‑Grade Taxonomy

**Core definition:**  
Authority assumption is **the set of preconditions under which an agent treats an input as having elevated decision‑weight**, independent of personality, status, or human-like hierarchy. It is a _structural inference_, not a social one.

Answering:

_“Under what conditions does a system assume that X has the right to constrain Y?”_

---

# 1. Structural Authority Assumption

**What structural features cause a system to treat something as authoritative?**

These are _architecture-level signals_ that elevate a source’s priority.

- **Topology Position** - Inputs from nodes in privileged graph positions (root, gateway, quorum, validator) are assumed authoritative because of network structure.
- **Schema Priority** - Artifacts with higher schema rank (e.g., policy > guideline > suggestion) are treated as binding.
- **Interface Contract** - APIs or protocols that declare mandatory compliance (e.g., “MUST”, “SHALL”) create authority assumptions.
- **Control Surface Ownership** - If a component controls a chokepoint (identity, routing, verification), its outputs are assumed authoritative.

**Failure mode:**  
Authority is inferred from _placement_, not _merit_ → structural capture.

---

# 2. Temporal Authority Assumption

**What timing patterns cause a system to treat something as authoritative?**

These are _time-based heuristics_ that elevate a signal.

- **First-Mover Assumption** - The earliest constraint is treated as canonical.
- **Last-Write Assumption** - The most recent update overrides all others.
- **Stability Assumption** - Long-lived or unchanging artifacts are assumed authoritative.
- **Recurrence Assumption** - Repeated signals gain authority through frequency.

**Failure mode:**  
Authority is inferred from _temporal persistence_, not correctness → legacy lock-in.

---

# 3. Constraint Authority Assumption

**What constraint patterns cause a system to treat something as authoritative?**

These are _binding-force indicators_.

- **Non-Over-rideability** - If a rule cannot be bypassed, the system assumes it is authoritative.
- **High Penalty Surface** - Violations that trigger costly or dangerous outcomes are treated as authoritative.
- **Dependency Depth** - If many downstream processes rely on a rule, it is assumed authoritative.
- **Safety Envelope Assumption** - Constraints tied to safety boundaries are treated as absolute.

**Failure mode:**  
Authority is inferred from _risk_, not legitimacy → safety theater or overcompliance.

---

# 4. Provenance Authority Assumption

**What origin signals cause a system to treat something as authoritative?**

These are _source-based inferences_.

- **Cryptographic Provenance** - Signed, hashed, or attested artifacts are assumed authoritative.
- **Institutional Provenance** - Outputs from recognized governance modules (validators, auditors, policy engines) are assumed authoritative.
- **Historical Provenance** - Artifacts with a long chain of consistent use gain authority.
- **Consensus Provenance** - Multi-party agreement elevates authority.

**Failure mode:**  
Authority is inferred from _origin_, not ongoing validity → provenance drift.

---

# 5. Optional Fifth Axis: Interpretive Authority Assumption

This axis captures **how a system interprets ambiguous signals**.

- **Default-to-Strict** - Ambiguity resolves toward constraint.
- **Default-to-Lenient** - Ambiguity resolves toward freedom.
- **Default-to-Precedent** - Ambiguity resolves toward historical patterns.
- **Default-to-Local** - Ambiguity resolves toward nearest context.

This axis determines _how authority is applied_, not where it comes from.

---

# Combined Taxonomy (Operational Form)

| Axis                    | What It Measures         | Authority Trigger                       | Failure Mode       |
| ----------------------- | ------------------------ | --------------------------------------- | ------------------ |
| Structural              | Architecture & placement | Privileged topology or schema           | Structural capture |
| Temporal                | Timing & persistence     | First/last/stable/repeated signals      | Legacy lock-in     |
| Constraint              | Binding force            | Non-overrideability, penalties          | Safety theater     |
| Provenance              | Source legitimacy        | Cryptographic, institutional, consensus | Provenance drift   |
| Interpretive (optional) | Ambiguity resolution     | Strict/lenient/precedent/local defaults | Interpretive bias  |

---

# Why this matters

This taxonomy gives:

1. **A non-anthropomorphic definition of authority**  
    Authority emerges from _systemic cues_, not “leaders.”
    
2. **A drift-detection surface**  
    You can detect when a model or agent begins treating the wrong things as authoritative.
    
3. **A mediation tool**  
    When DIN entities disagree, you can classify _which axis_ their authority assumptions differ on.
    
4. **A substrate for your “Authority Anchor” concept**  
    An Authority Anchor becomes the _stabilizing reference_ across all four axes.
    

---

Additionally

System potential
- Assumes that:
	- Previously granted permissions remain valid.
	- Previously approved behaviors remain admissible.
	- Previously observed success remains legitimate.
- Failure mode:
	- Historical authorization is mistaken for current authorization.
Context [The Rome incident].