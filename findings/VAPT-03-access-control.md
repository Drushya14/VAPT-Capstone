# VAPT-03 — Broken Access Control

## Severity
Medium

## CVSS v3.1
6.3

## OWASP Mapping
A01:2021 — Broken Access Control

## Description
The assessment identified an access-control weakness in the authorized training environment where protected resources may be accessible when object identifiers are trusted without sufficient server-side authorization checks.

## Impact
An authenticated user with limited privileges may potentially access or modify resources belonging to another user, resulting in confidentiality or integrity impact.

## Recommended Remediation
- Enforce authorization on the server for every protected request.
- Verify resource ownership before allowing access.
- Apply deny-by-default authorization policies.
- Do not rely only on client-side access controls.
- Add horizontal and vertical privilege regression tests.

## Remediation Timeline
Remediate within 7–14 days, with priority given to sensitive or administrative resources.

## Retesting
Repeat the authorized access-control test using different user roles and object identifiers. Verify that users can access only resources they are authorized to access.

## Evidence
Refer to the corresponding evidence included in the final VAPT report.
