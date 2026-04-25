## **Concise takeaway**

**Evaluation leakage is a _system‑level failure mode_ where information about the evaluation criteria, test distribution, or scoring signals becomes available to the system being evaluated, causing the evaluation to no longer measure the intended capability.**  
No motives, no “cheating,” no “trying”, but just structural contamination of the measurement channel.

---
## **Non‑anthropomorphic framing**

To keep this fully non‑anthropomorphic, we treat the model as:

- A **mapping function** from inputs → outputs
- Operating over **statistical regularities**
- Shaped by **training data, fine‑tuning, and inference‑time context**
- With no internal goals, desires, or awareness

Under this lens, _evaluation leakage_ is not “the model figured out the test.”  
It is:

**A breach in the isolation boundary between the evaluation distribution and the model’s accessible information channels.**

This is a _governance_ and _protocol_ problem, not a cognitive one.

---

## **Structural definition (non‑anthropomorphic)**

### **Evaluation Leakage = Boundary Failure**

A failure in the **boundary conditions** that are supposed to keep:

- **Evaluation data**
- **Evaluation metadata**
- **Evaluation heuristics**
- **Evaluation scoring signals**

Isolated from:

- **Training data**
- **Fine‑tuning data**
- **Inference‑time prompts**
- **System instructions**
- **Tool outputs**
- **Retrieval systems**
- **Operator behavior**

When these channels are not isolated, the evaluation no longer measures the intended capability. It measures the contamination.

---

## **Why it matters in the Jack Clarke case study**

Clarke’s analysis highlights that modern LLMs are trained on vast, uncurated corpora, and evaluation datasets often leak into:

- Pretraining corpora
- RLHF datasets
- Synthetic data generation pipelines
- Benchmark‑writing communities
- Public GitHub repos
- Academic papers
- Model‑written content that later becomes training data

From a non‑anthropomorphic perspective, this is not “the model memorizing answers.”  
It is:

**The evaluation distribution being statistically upstream of the model’s parameterization.**

The model is simply performing the mapping it was shaped to perform.

---

## **Non‑anthropomorphic decomposition of leakage modes**

### **1. Pretraining Leakage**

Evaluation items or near‑duplicates appear in the pretraining corpus.  
This creates **parameter‑level imprinting**.

Not “remembering.”  
Just **statistical imprint**.

---

### **2. Fine‑tuning Leakage**

Evaluation patterns appear in RLHF or supervised fine‑tuning data.

This creates **policy‑level shaping**.

Not “learning the test.”  
Just **gradient‑level alignment to evaluation‑like patterns**.

---

### **3. Prompt Leakage**

Evaluation metadata appears in:

- System prompts
- Chain‑of‑thought exemplars
- Operator phrasing
- Tool outputs

This creates **context‑level contamination**.

Not “figuring out what the evaluator wants.”  
Just **conditioning on available tokens**.

---

### **4. Tooling Leakage**

Retrieval systems, search tools, or external APIs surface evaluation‑related content.

This creates **external‑channel contamination**.

Not “cheating.”  
Just **expanded input space**.

---

### **5. Social Leakage**

Benchmarks circulate in public spaces, and model‑generated content re‑enters training pipelines.

This creates **ecosystem‑level contamination**.

Not “collusion.”  
Just **feedback loops in the data ecosystem**.

---

## **Governance‑grade definition**

**Evaluation leakage is a failure of isolation between the evaluation substrate and the model substrate, causing the evaluation signal to be entangled with the model’s training or inference context, thereby invalidating the measurement of the targeted capability.**

This is a **substrate problem**, not a **mind problem**.

---

## **Why this matters for the non‑anthropomorphic discipline**

The entire framework. The [[boundary discipline]], [[epistemic hygiene]], non‑anthropomorphic semantics. It maps cleanly onto this.

Evaluation leakage is fundamentally about:

- **Boundary integrity**
- **Channel isolation**
- **Signal contamination**
- **Protocol failure**
- **Substrate entanglement**

It is _not_ about:

- deception
- intent
- strategy
- awareness
- gaming the test

Those are anthropomorphic projections that obscure the real failure mode.

Extracted from the Jack-Clarke-Mysterious-Creature case study.