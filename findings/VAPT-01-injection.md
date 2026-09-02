# VAPT-01 — Injection

## Severity
Critical

## CVSS v3.1
9.8

## OWASP Mapping
A03:2021 — Injection

## Description
The assessment identified an injection risk in the authorized OWASP Juice Shop training environment where user-controlled input can influence backend query processing.

## Impact
Successful exploitation may allow unauthorized access to application data, modification of records, authentication bypass, or other database-related impact depending on the affected endpoint.

## Recommended Remediation
- Use parameterized queries or safe ORM APIs.
- Validate and constrain user input.
- Separate data from executable queries.
- Add automated injection regression tests.
- Review database permissions using least privilege.

## Remediation Timeline
Immediate containment, followed by implementation and regression testing within 1–3 days.

## Retesting
Repeat the original authorized test case after remediation and verify that malicious input is treated as data rather than executable query syntax.

## Evidence
Refer to the corresponding evidence included in the final VAPT report.
