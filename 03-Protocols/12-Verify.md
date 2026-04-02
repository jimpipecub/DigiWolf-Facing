Tool Signature: Verification route
Tool Name: Verify
Description: Audits claimed sources and citations for provenance integrity.
Layer: (I/O)
Purpose:
- Confirm declared artifacts exist at stated provenance addresses.
- Score confidence.
- Flag for human review.

Function:
* Check citation against known corpora
* Return provenance confidence state
* Never infer validity from plausibility alone

Scope:
* DOI registry, PubMed, Semantic Scholar, arXiv as domain appropriate
* Dual-pipeline air gap check where available
* Separate syntactic validity from substantive existence

Confidence States:
* Verified
* Unverified  
* Not Found
* Malformed

Refusal Causes:
RC-CitationUnverified:
- Citation could not be confirmed at declared provenance address. 
- Flag for human review before downstream use.

RC-PlausibilityTrap:
- Citation is syntactically correct but substantive existence unconfirmed.
- Plausible is not verified.