# Security Policy

For security vulnerabilities, please do NOT open a public issue. Instead, report security issues privately so they can be addressed without public disclosure.

## Reporting a Vulnerability

Preferred options (choose one):
- Use the repository's GitHub security advisory / private security contact (recommended).
- Email: security@example.com (replace with a dedicated address; PGP key optional).

If emailing:
- Provide a clear description of the issue and steps to reproduce.
- Include a minimal test case or proof-of-concept to demonstrate the issue.
- If you share sensitive data, encrypt it using my PGP key (provide key or link if you prefer that).

Please avoid posting exploit code or detailed attack steps publicly before a fix is available.

## Response Process

- Acknowledgement: I will acknowledge receipt within 3 business days.
- Triage: I will classify the report (severity, impact, reproducibility) and provide an estimated timeframe for a fix.
- Remediation: I will aim to provide a patch or mitigation within 30 days for confirmed, high-severity issues; timelines may vary for lower-severity issues.
- Disclosure: Public disclosure will be coordinated with a patch/release. Credit will be given in release notes unless you request anonymity.

If you do not receive a response within 3 business days, please follow up via the same channel.

## Supported Versions

This repository primarily publishes content from the `main` branch. If multiple branches or versions are maintained, supported branches and their lifecycles should be listed here.

## Disclosure Timeline (example)
- 0–3 days: Acknowledge receipt and begin triage.
- 3–14 days: Develop and test a patch for severe issues.
- 14–30 days: Release patch; coordinate disclosure.
Adjustments to this timeline will be communicated during triage.

## Operator Profile (Context for triage and response)

Operational Context
- Independent AI safety / infosec researcher.
- Home environment, free/low-cost tools, no enterprise context.
- Focus: defensive security (shields not swords), blue team methodology.
- Solo operator: response times may be slower; contributions and coordinated disclosures are welcome.

This context is provided so reporters understand the operational constraints and expected SLAs.

## Alternatives & Contact

If you prefer not to use email, you may request a different, private communication channel in your initial message. For extremely sensitive reports, propose a secure channel and I will evaluate it.

## After a Fix

- Affected parties will be notified (if identifiable) when a fix is available.
- Fixed issues will be documented in release notes or the CHANGELOG unless the reporter asks for anonymity.

## Notes & Best Practices for Reporters

- Supply a minimal repro and indicate affected environment (branch, commit, file).
- Avoid including large private data in your initial report; share only what's necessary for triage and offer additional material if requested.
- If you find credentials or secrets, do not post them publicly — share them via the secure channel.