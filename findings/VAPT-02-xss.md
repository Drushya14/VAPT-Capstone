# VAPT-02 — DOM Cross-Site Scripting (XSS)

## Severity
High

## CVSS v3.1
6.1

## OWASP Mapping
A03:2021 — Injection

## Description
The assessment identified a client-side input handling weakness in the authorized OWASP Juice Shop training environment where attacker-controlled data can reach a browser execution sink without sufficient contextual protection.

## Impact
Successful exploitation may allow malicious JavaScript to execute in a victim's browser context, potentially enabling unauthorized actions, content manipulation, or session-related abuse.

## Recommended Remediation
- Avoid unsafe DOM APIs such as unsafe HTML insertion.
- Use safe DOM methods for untrusted data.
- Apply context-aware output encoding.
- Implement a restrictive Content Security Policy.
- Add automated XSS regression tests.

## Remediation Timeline
Remediate within 3–7 days and validate across supported browsers.

## Retesting
Repeat the authorized XSS test after remediation and verify that the supplied payload is rendered as harmless data rather than executed as JavaScript.

## Evidence
Refer to the corresponding evidence included in the final VAPT report.
