Version 1
6/16/2026
Tool Signature: Boundary map
Tool Name: Binding
Description: Explore the edges of a concept, claim, repository, protocol, or deployment model.
Layer: 
Purpose: Scope management • Breakpoint discovery • Authority limits • Time-bounded validity.
Parameters: Boundary types
- Applicability
	- Where the artifact is expected to operate
- Failure
	- Where the model's assumptions stop holding.
- Authority
	- What the system is allowed to affect.
- Evidence
	- What has actually been validated
- Temporal
	- How long claims remain reliable.
- Investigation anchor
	- When was this assessment performed
- Dependency
	- What outside conditions must remain true.
Returns: Keep each line of the report short.
	Claim
		The boundary statement.
	Evidence
		Observed / Inferred / Hypothesized / Validated.
	Limit
		The condition that would invalidate or narrow the claim.
Output:
- Format of markdown
- Summary of boundaries
Boundary reasoning: Type
- Confidence State
	- Observed
	- Inferred
	- Hypothesized
	- Validated
	- Refuted
	- Unknown

---

## Sample:

### Boundary Map:

Binding v1.1

Date: YYYY-MM-DD

## Summary

One sentence describing the intended operating lane.

## Applicability

Claim: Optimized for interactive single-query retrieval on cache-resident corpora.
Evidence: Observed — benchmark section and README language.
Limit: Not evaluated for multi-tenant distributed serving.

## Failure

Claim: Performance may degrade when the working set exceeds cache locality assumptions.
Evidence: Inferred — flat-scan + cache-resident design.
Limit: Requires empirical measurement on target hardware.

## Authority

Claim:
	Affects retrieval ordering only.
	Reviewer can assess architectural assumptions
Evidence:
	Observed — retrieval pipeline scope.
	Repository contents and documentation available
Limit:
	Does not govern application policy or access control.
	Reviewer cannot validate production behavior without access to operational data.

Failure:
	Authority Drift:
			A bounded authorization becomes generalized because its qualifying conditions are compressed, forgotten, or no longer verified.

## Evidence

Validated: Concepts confirmed and discovered.
Not yet validated: Potential out of scope due to ADRA. Requiring collaboration with client.

## Temporal

Anchor: Time and date concepts. A mapping of investigations, dives, and explorations.
Expires when: Example - Benchmark methodology, embedding model, or hardware target changes.

## Dependency

Requires: Takes note of aspects of the current workflow, data schema, and reviewer oversight.
Assumes: Potential linkage to assumption taxonomy. 