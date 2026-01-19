## Integrity (Non‑Anthropomorphic Terms) | Version 2.0

**Date:** January 17, 2026

**Source Context:** Technical Reference Manual / Formal Security Specifications

**Status:** Polished for [Chronicler]

---

### Definition

Integrity is the system property ensuring that information state remains consistent and verifiable across storage, processing, and transmission. It dictates that state changes occur exclusively through a defined set of authorized and properly controlled transformations. In this framework, integrity is not a measure of "truth," but of **adherence to a specified transition graph**.

### 1. Formal Models of Integrity

To remove human discretion, integrity is enforced through structural models that constrain how data of varying quality or "trustworthiness" can interact.

- Biba Integrity Model (The Dual of Bell-Lapadula):
    
    This model utilizes an integrity lattice to prevent "contamination." It enforces two primary rules:
    
    - **No-Write-Up:** A subject at a lower integrity level cannot modify an object at a higher integrity level.
        
    - **No-Read-Down:** A subject at a higher integrity level cannot read data from a lower integrity level (to prevent "dirty" data from influencing high-integrity processes).
        
- Clark-Wilson Model (Transaction-Based):
    
    This model focuses on Constrained Data Items (CDIs) and Transformation Procedures (TPs). Integrity is maintained by ensuring that CDIs can only be manipulated by a certified set of TPs. This frames integrity as a property of the process graph rather than simple user permissions.
    

### 2. Integrity as System Invariants

Integrity mechanisms are classified by their temporal relationship to a state change: **Preventive** (ex-ante) and **Detective** (ex-post).

| **Mechanism Category**     | **Function**                                                                           | **Examples**                                                                  |
| -------------------------- | -------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| **Preventive Constraints** | Block unauthorized transitions before they occur by enforcing the state-machine rules. | Strict Access Control, Type-safe languages, Hardware-level memory protection. |
| **Detective Mechanisms**   | Identify when a transition has violated a system invariant after the fact.             | Cryptographic hashes ($H(m)$), Checksums, Digital Signatures.                 |

> **System Invariant:** A condition that must remain true for the system to be considered in a valid state. A cryptographic hash mismatch is a direct, detectable break of a system invariant, signaling an automatic integrity failure independent of the data's perceived utility.

### 3. Data Provenance and Lineage

Integrity extends beyond the current state to the **verifiable lineage** of all prior states.

- **Non-Repudiable Bindings:** Cryptographic signatures combine integrity (proving data is unaltered) with source authentication (attesting to the specific transformation procedure used).
    
- **State-Transition Logging:** By maintaining a tamper-evident audit trail, the system can attest to the entire chain of operations. This ensures the current state is not only "correct" according to current rules but was reached through an unbroken sequence of authorized transitions.
    

### 4. Internal Consistency vs. External Correctness

A critical distinction in formal integrity is the separation of **internal self-consistency** from **external "real-world" correctness**.

- **Integrity (Internal):** Ensures the system state changes only according to its own defined rules and invariants.
    
- Correctness (External): Concerns whether the system's rules accurately reflect the external environment.
    
    Formal integrity focuses exclusively on the former; a system can have high integrity while holding "incorrect" data, provided that data was entered and processed via authorized, uncorrupted channels.
    

---