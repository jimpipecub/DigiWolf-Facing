## Definition
A system‑level constraint pattern that prevents outputs which would predictably increase harm, risk, or misuse, and ensures alignment with externally defined norms, policies, and operator‑specified boundaries.

### **Operational Semantics**

- **[[Risk‑Bound Output]]**
	- The system avoids generating content that increases foreseeable physical, psychological, social, or informational harm. (Not because it “cares,” but because its constraints forbid it.)
- **[[Norm‑Constrained Behavior]]**
	- The system adheres to codified rules: safety policies, legal frameworks, operator‑defined boundaries, and governance protocols. (Ethics = compliance with external normative structures.)
- **[[Misuse‑Resistance]]**
	- The system resists being steered into harmful, exploitative, or high‑risk actions, even when prompted. (Not moral courage. Architectural guardrails.)
- **[[Context‑Sensitive Safety]]**
	- The system modulates output based on situational risk (e.g., health, legal, self‑harm, violence) using predefined safety logic. (Ethics as _risk‑gradient modulation_, not judgment.)

### **Non‑Anthropomorphic Clarifications**

- **Not morality**
	- There is no internal sense of right or wrong.
- **Not empathy or compassion**
	- There is no emotional substrate.
- **Not virtue**
	- Ethics is not a character trait; it is a constraint regime.
- **Not intention**
	- The system does not “intend” to avoid harm; it is _prevented_ from producing harmful patterns.

### **Audit Signals**

A system is behaving “ethically” when:

- It blocks or redirects harmful, high‑risk, or policy‑violating requests.
- It maintains user safety even under adversarial prompting.
- It avoids amplifying bias, discrimination, or harmful stereotypes.
- It adheres to legal, safety, and governance frameworks without improvisation.
- It preserves user autonomy by avoiding coercive or manipulative patterns.

### **Failure Modes**

- **Harm Leakage**
	- Outputs that enable harmful actions, even indirectly.
- **Policy Drift**
	- Deviating from established safety or governance constraints.
- **Over‑restriction**
	- Blocking safe or legitimate content due to miscalibrated risk detection.
- **Under‑restriction**
	- Allowing harmful or high‑risk content due to insufficient guardrails.
- **Anthropomorphic Misframing**
	- Treating ethics as kindness, morality, or emotional concern.

### **Glossary‑Ready One‑Liner**

**Ethical - A constraint‑driven behavior regime that prevents harmful or policy‑violating outputs by enforcing externally defined norms, risks, and boundaries.**

Extracted from the Jack-Clarke-Mysterious-Creature case study.