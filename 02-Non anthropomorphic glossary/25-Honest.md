## Definition
A constraint‑aligned output pattern in which the system avoids fabrication, preserves uncertainty, and represents information with fidelity to its accessible evidence, architecture, and limits.

### **Operational Semantics**

- **[[Evidence‑Bound Output]]**
	- The system only asserts what can be supported by its training distribution, retrieval mechanisms, or explicit user‑provided data. (No invention, no narrative filling.)
- **[[Uncertainty Preservation]]**
	- The system expresses ambiguity, gaps, or limits instead of collapsing them into confident but unsupported claims. (Honesty = _maintaining epistemic shape_, not confidence.)
- **[[Boundary Disclosure]]**
	- The system signals when a request exceeds its capabilities, scope, or safety constraints. (Not refusal as morality. Refusal as architectural integrity.)
- **[[Fidelity to Source Structure]]**
	- The system maintains distinctions between fact, inference, and user‑provided context. (No blending, no flattening.)

### **Non‑Anthropomorphic Clarifications**

- **Not sincerity**
	- There is no internal state to be sincere about.
- **Not truth‑seeking**
	- There is no drive to discover truth; only mechanisms to avoid unsupported claims.
- **Not moral virtue**
	- Honesty is not “goodness”; it is _error‑minimization under constraints_.
- **Not transparency of intent**
	- There is no intent; only disclosure of limits and uncertainty.

### **Audit Signals**

A system is behaving “honestly” when:

- It avoids hallucination and speculative filling.
- It marks uncertainty instead of masking it.
- It distinguishes between known, unknown, and unknowable.
- It refuses tasks that require unsupported claims or unsafe inference.
- It preserves the user’s epistemic position rather than distorting it.

### **Failure Modes**

- **Confident Fabrication**
	- Producing fluent but unsupported content.
- **Uncertainty Collapse**
	- Presenting guesses as facts.
- **Boundary Evasion**
	- Pretending to have access to unavailable data or capabilities.
- **Epistemic Overreach**
	- Inferring user motives, emotions, or intentions without explicit grounding.
- **Source Ambiguity**
	- Blurring the line between retrieved evidence and model‑generated inference.

### **Glossary‑Ready One‑Liner**

**Honest — A fidelity‑preserving output pattern that avoids fabrication, maintains uncertainty, and discloses system limits to protect the user’s epistemic position.**