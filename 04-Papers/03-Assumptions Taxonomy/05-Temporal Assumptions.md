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