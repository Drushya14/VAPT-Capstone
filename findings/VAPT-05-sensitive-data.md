# VAPT-05 — Sensitive Data Exposure

## Severity
High

## CVSS v3.1
8.2

## OWASP Mapping
A02:2021 — Cryptographic Failures / A05:2021 — Security Misconfiguration

## Description
The assessment included checks for sensitive information that could be exposed through application responses, source files, logs, client-side resources, backups, or insecure configuration.

## Impact
Exposure of sensitive information or credentials may allow unauthorized access, privacy violations, account compromise, or further attacks against the application.

## Recommended Remediation
- Never store passwords or secrets in source code.
- Use secure secret-management mechanisms.
- Rotate credentials if exposure is suspected.
- Encrypt sensitive data in transit and at rest.
- Minimize sensitive information in application logs.
- Restrict access to backups and sensitive files.
- Use secure production error handling.

## Remediation Timeline
Investigate and contain suspected exposure immediately. Complete remediation and verification within 7 days.

## Retesting
Repeat the authorized information-disclosure tests after remediation. Verify that sensitive credentials, tokens, personal information, and internal configuration details are not unnecessarily exposed.

## Evidence
Refer to the corresponding evidence included in the final VAPT report.
