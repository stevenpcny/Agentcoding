# Security Review and Hardening

## Core rule
Every code change that touches user input, external systems, authentication, or data handling must undergo explicit security review before acceptance. Security is treated as a first-class verification dimension, not an afterthought.

## When to use
- Any code handling user input, files, network requests, or sensitive data
- Authentication, authorization, or session management changes
- Integration with third-party services or APIs
- Deployment or infrastructure modifications

## When not to use
- Purely internal logic with no external surface
- Non-production experimental code

## Decision rules
- Assume all external input is untrusted by default
- Validate and sanitize at the earliest possible layer
- Use established libraries for cryptography, auth, and parsing instead of custom implementations
- Apply the principle of least privilege for any permissions or tokens
- Document security assumptions and threat model for non-obvious decisions

## Verification checklist
- Have all inputs been validated or sanitized?
- Are secrets and credentials handled through secure mechanisms (never hardcoded)?
- Does the change follow least-privilege principles?
- Has the code been checked against common vulnerability classes (injection, auth bypass, data exposure)?
- Is there a clear path to audit or log security-relevant events?

## Anti-patterns
- Trusting client-side validation alone
- Hardcoding secrets or using weak defaults
- Building custom crypto or auth when battle-tested libraries exist
- Ignoring error messages that leak sensitive information
- Adding powerful permissions "just in case"

## Evidence notes
- `knowledge/notes/2026-05-11-2053814471793971582-mindos-lisa.md`
- `knowledge/notes/2026-05-13-2054502229391114435-nainsidwiv50980.md`

## Example prompts
- Read this playbook and perform a security review on the following code change.
- Apply this playbook: identify potential attack surfaces introduced by this feature and propose mitigations.
- Generate a minimal security checklist for this type of integration.