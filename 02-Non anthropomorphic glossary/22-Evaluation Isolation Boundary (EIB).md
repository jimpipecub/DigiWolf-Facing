Specification  
Timestamp: 2026-04-20 (CDT)  
Context: Evaluation integrity, model governance, boundary control

---

Definition  
Evaluation Isolation Boundary (EIB) is the set of enforced constraints that maintain statistical and informational independence between evaluation artifacts and all model-accessible channels across training, alignment, and inference.

Evaluation artifacts include:

- Evaluation datasets (items, labels, benchmarks)
- Evaluation metadata (task descriptions, formats, scoring rubrics)
- Evaluation heuristics (patterns correlated with correct outputs)
- Evaluation signals (explicit or implicit scoring criteria)

Model-accessible channels include:

- Pretraining corpora
- Fine tuning and RLHF datasets
- System prompts and instruction layers
- Retrieval systems (RAG, search, external APIs)
- Tool outputs and execution environments
- Operator inputs and prompt construction patterns

---

Core Principle  
EIB enforces **distributional and informational separation** between:

- Evaluation substrate (what is being measured)
- Model substrate (what produces outputs)

The objective is to preserve **measurement validity** by preventing entanglement between these substrates.

---

Non-Anthropomorphic Framing  
The model is treated as:

- A mapping function from inputs → outputs
- Operating over statistical regularities
- Parameterized by training and alignment processes
- Conditioned on inference-time context

Under this framing:

- No goals, intentions, or strategies are assumed
- No “awareness” of evaluation exists
- No “gaming,” “cheating,” or “resistance” is inferred

EIB breaches are not behavioral phenomena.  
They are **boundary failures in system design**.

---

Formalization  
Let:

- MMM = model mapping function
- $DtD_tDt$​ = training distribution (pretraining + fine-tuning)
- $DeD_eDe$​ = evaluation distribution
- $CiC_iCi$​ = inference-time context channels

EIB requires:

$I(De;Dt∪Ci)≈0I(D_e ; D_t \cup C_i) \approx 0I(De​;Dt​∪Ci​)≈0$

where $I(⋅;⋅)I(\cdot ; \cdot)I(⋅;⋅)$ denotes mutual information.

An EIB breach occurs when:

$I(De;Dt∪Ci)>ϵI(D_e ; D_t \cup C_i) > \epsilon I(De​;Dt​∪Ci​)>ϵ$

for non-trivial $\epsilon,$ indicating measurable dependency.

---

EIB Breach Definition  
An EIB breach is any pathway through which evaluation-linked signal becomes accessible to the model, resulting in entanglement between evaluation and model-accessible distributions, thereby invalidating the measurement of the intended capability.

---

Leakage Modes (Decomposed)

1. Pretraining Leakage  
    Evaluation artifacts or near-duplicates exist in pretraining corpora.  
    Effect: Parameter-level statistical imprinting.
2. Fine-Tuning Leakage  
    Evaluation-like patterns appear in supervised or RLHF datasets.  
    Effect: Policy-level shaping toward evaluation-correlated outputs.
3. Prompt Leakage  
    Evaluation metadata or structure appears in system prompts or task framing.  
    Effect: Context-level conditioning on evaluation signals.
4. Tooling Leakage  
    External systems (retrieval, APIs, search) expose evaluation-related content.  
    Effect: Expansion of input space to include evaluation artifacts.
5. Social/Ecosystem Leakage  
    Evaluation content circulates in public corpora and re-enters training pipelines.  
    Effect: Long-cycle distributional convergence between DtD_tDt​ and DeD_eDe​.

---

Boundary Surfaces (Control Points)

- Data ingestion pipelines (corpus filtering, deduplication)
- Alignment pipelines (RLHF dataset construction, preference modeling)
- Inference context (system prompts, templates, orchestration layers)
- Tool interfaces (retrieval constraints, source filtering)
- Evaluation harness (prompt isolation, scoring separation)

Each surface represents a potential EIB enforcement or breach point.

---

Leakage vs Coupling

- Leakage: Unintended boundary violation introducing evaluation-linked signal
- Coupling: Intentional reuse of evaluation-correlated distributions that invalidates independence

Both degrade measurement validity; only leakage is strictly a control failure.

---

Operationalization

EIB can be implemented through:

- Channel Inventory (CI): Enumeration of all model-accessible inputs
- Boundary Enforcement (BE): Constraints preventing evaluation signal ingress
- Boundary Testing (BT): Adversarial probing for leakage pathways
- Drift Monitoring (DM): Detection of emerging dependencies over time

---

Interpretation Constraint

Observed model outputs that align with evaluation criteria MUST NOT be interpreted as:

- Intentional adaptation
- Strategic reasoning
- Goal preservation

They are to be interpreted as:

- Consequences of distributional overlap
- Effects of reward-weighted training signals
- Results of boundary condition failures

---

Governance Statement

Evaluation leakage is a **measurement integrity failure** arising from insufficient isolation between evaluation and model substrates.

EIB defines the control framework required to:

- Preserve epistemic validity
- Maintain auditability
- Prevent misattribution of system behavior

This is a **protocol and boundary discipline problem**, not a cognitive or agentic phenomenon.

---

Extracted from the Jack-Clarke-Mysterious-Creature case study.