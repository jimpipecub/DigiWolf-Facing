# Aegis Protocol: Temporal Diagnostic Integration (Universal Framework)

## Purpose

A structured workflow for rapidly diagnosing the likelihood of AI-enhanced cyberattacks and driving shield-first defense recommendations. Developed through real-world case studies and validated by multi-model collaboration.

## Evolution

Originated as a niche tool for political incident analysis, iteratively refined through practical application (UPenn breach, Columbia case) and collaboration with Manus, Claude, Perplexity, and human analyst. Now a universal, all-purpose protocol.

## Workflow Steps

1. **Identify Trigger Event:** Broadened to any motivating event (political, technical, corporate, social).
2. **Calculate Velocity:** Time between trigger and breach is a primary diagnostic metric.
3. **AI Enhancement Probability Tier:** Probability based on velocity matrix.
4. **Root Cause Analysis:** Diagnostic-driven—victim gaps vs. attacker capabilities.
5. **Shield-First Response:** Harden essentials; escalate to AI-specific defenses only if warranted.

Probability tiers are treated as bounded uncertainty envelopes, not deterministic classification

## Application

- For incident responders, security teams, and community threat analysts.
- Modular: Can be embedded in playbooks, automated workflows, and multi-model orchestration pipelines.

## Quick Start Checklist

- [ ] Log trigger event (timestamp & type)
- [ ] Record breach timestamp
- [ ] Calculate velocity
- [ ] Assign AI enhancement tier
- [ ] Guide investigation to shield-first remediation

## Velocity Tier (Trigger → Breach)

Tier 0: >30 days  → Low AI likelihood (human-dominant)
Tier 1: 7–30 days → Possible automation
Tier 2: 24–72 hrs → Likely AI-assisted
Tier 3: <24 hrs   → High AI-enhancement probability
Tier 4: <1 hr     → Automated / agentic pipeline suspected

## Expected false positive / Limitation

High velocity alone is insufficient for AI attribution; CDN automation, pre-positioned access, and insider activity may produce similar patterns

## Versioning

- **v1.0**: Political trigger version
- **v2.0**: Universal validated version (multi-model consensus)

## References

- UPenn Case Study
- Columbia Breach Analysis
- Manus, Perplexity, Claude validation records

---
Vital note: This protocol assesses likelihood of AI enhancement, not attribution of specific tooling or actors.