# **Access Control (Non‑Anthropomorphic Definition)**

Date of moving over to public: February 18th, 2026

### **Definition**

Access control is a **constraint-evaluation mechanism** that determines whether proposed state transitions are permitted within an information environment. It evaluates formal properties of subjects, objects, and context to produce a decision. No human intention or agency is assumed.

### **Core Components**

- **Subject Descriptor (S):**  
    Any entity capable of initiating an operation — human, service, process, workload, robot, key, token.
    
- **Object Descriptor (O):**  
    Any resource over which operations occur — file, API, secret, queue, configuration, physical actuator.
    
- **Operation (op):**  
    A state transition (read, write, execute, invoke, configure, delete, open).
    
- **Environment (E):**  
    Contextual attributes (time, network segment, device posture, session risk score).
    
- **Policy Engine (P):**  
    A decision function over subject, object, and environmental attributes:
    [ decision = f(A_S, A_O, A_E) ]  
    Output: permit / deny (+ optional obligations: log, watermark, break‑glass).
    

### **Interpretation**

Instead of “Alice can read file X,” the system evaluates:

- Subject S has attributes (A_S)
- Object O has attributes (A_O)
- Environment E has attributes (A_E)
- Policy P evaluates (f(A_S, A_O, A_E))

No “trying,” no “wanting,” no “ownership.”  
Just constraint evaluation.

---

# **Model Reinterpretations (Constraint‑First)**

### **DAC (Discretionary Access Control)**

Constraints live on the object.  
Object stores subject IDs + permitted operations.  
Modification is itself a controlled operation.

### **MAC / Lattice Models**

Constraints are label‑based.  
Policy is a lattice of classification levels + compartments.  
Reference monitor enforces lattice rules.

### **RBAC**

Roles are attribute bundles.  
Mapping is:  
[ Subject \rightarrow Roles \rightarrow Permissions ]  
Pure table lookups.

### **ABAC / NDAC**

Policy is a set of predicates over arbitrary attributes of S, O, and E.  
Evaluation is a function over attribute tuples.

Across all models, “user” is just a **subject descriptor**.

---

# **Non‑Human Identities (Modern Reality)**

Modern systems treat humans and machines identically:

- service principals
- API keys
- ephemeral workloads
- robots
- containers
- CI/CD agents

Each is a subject with attributes.  
Same engine, different attribute vectors.

This is the foundation of:

- **zero standing privilege**
- **just‑in‑time access**
- **ephemeral credentials**
- **continuous authorization**

---

# **Practical Glossary Entry**

### **Access Control**

A constraint‑evaluation system that determines whether a proposed state transition is permitted, based on the attributes of a subject, an object, and the environment. Access is not a property of a person but the outcome of a policy function applied to attribute vectors. All identities — human or non‑human — are subject descriptors evaluated symmetrically.

---

If you want, we can continue building out the glossary in this style:

- **Identity**
- **Trust Boundary**
- **State Transition**
- **Constraint Saturation**
- **Policy Drift**
- **Reference Monitor**
- **Control Plane**
- **Epistemic Integrity**

Just say which one you want to tackle next, and we’ll shape it into the same clean, non‑anthropomorphic form.