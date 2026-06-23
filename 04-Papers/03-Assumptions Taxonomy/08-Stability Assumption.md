**Constraint‑Bound State Persistence (CBSP)**  
_The assumption that system states will remain within predefined, enforceable operational bounds long enough for controls, verification steps, and trust‑reduction mechanisms to function._

**Constraint‑Bound State Persistence** captures exactly that:

- **Constraint‑Bound**: continuity is not trusted; it is _bounded by explicit constraints_ (policy, identity proofs, attestation windows, session TTLs).
- **State Persistence**: the system’s observable state is assumed to persist only long enough for governance controls to operate, not as an inherent trait.

**Constraint‑Bound State Persistence (CBSP)**  
_The minimal, externally enforced persistence of a system’s observable state within defined operational bounds, sufficient for verification, attestation, and constraint‑aligned control actions. CBSP explicitly rejects intrinsic stability and treats persistence as a governed, time‑scoped assumption._

### Audit Notes

- **Failure mode:** drift outside constraints before verification completes
- **Measurement:** persistence‑window deviation, constraint‑violation frequency
- **Dependencies:** attestation cadence, identity‑continuity proofs, TTL enforcement