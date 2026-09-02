# VAPT-04 — Authentication Weakness

## Severity
Critical

## CVSS v3.1
9.1

## OWASP Mapping
A07:2021 — Identification and Authentication Failures

## Description
The assessment identified authentication-related weaknesses in the authorized training environment. Weak credential controls, insufficient protection against repeated login attempts, or insecure authentication flows can increase the likelihood of account compromise.

## Impact
An attacker may be able to compromise user accounts, access protected information, or perform actions using another user's identity.

## Recommended Remediation
- Enforce strong password requirements.
- Block or screen common and compromised passwords.
- Implement authentication rate limiting.
- Use secure password hashing.
- Protect password-reset and account-recovery mechanisms.
- Enable multi-factor authentication for privileged accounts.
- Monitor repeated authentication failures.

## Remediation Timeline
Begin remediation immediately, with critical authentication protections implemented within 1–3 days.

## Retesting
Repeat the authorized authentication tests after remediation. Verify that weak credentials are rejected, repeated attempts are appropriately limited, and protected accounts cannot be accessed without valid authentication.

## Evidence
Refer to the corresponding evidence included in the final VAPT report.
