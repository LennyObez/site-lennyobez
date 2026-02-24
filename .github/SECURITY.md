# Security policy

## Our commitment

Security matters for lennyobez.com. The site handles contact forms, session management, and content delivery, so we prioritize secure defaults, strict input validation, and safe session handling.

## Supported versions

This project is currently in pre-release development. Security fixes are provided for the `main` branch (latest commit). Once the site reaches general availability, we'll publish a more detailed support matrix.

## Reporting a vulnerability

Please use GitHub Private Vulnerability Reporting (Security Advisories) on this repository. If that's unavailable, email us directly.

- **Email:** security@lennyobez.com
- **Subject:** `[SECURITY] <short summary>`
- **Include:**
  - Affected version or commit
  - Impact and attack scenario
  - Reproduction steps or proof of concept (keep it safe and minimal)
  - Any mitigations you're aware of

**Don't include real credentials, API keys, or personal data in reports.** Use synthetic values only.

### What to expect

- **Acknowledgment:** within 48 hours
- **Initial triage:** within 7 days
- **Fix timeline:** depends on severity and complexity

### Severity levels

| Severity | What it means | Examples |
|----------|--------------|----------|
| Critical | Remote code execution, authentication bypass, data exfiltration | SQL injection, deserialization RCE, broken crypto |
| High | Privilege escalation, significant data exposure, CSRF on state-changing actions | IDOR on sensitive resources, session fixation, missing access control |
| Medium | Limited impact, requires specific conditions or user interaction | Stored XSS, SSRF with limited reach, timing side-channels |
| Low | Minor issues, information disclosure with minimal impact | Verbose error messages, missing security headers on non-sensitive routes |

Critical and high issues get patched immediately. Medium and low issues are addressed in the next release unless the risk changes.

### In scope

- Cross-site scripting (XSS)
- Cross-site request forgery (CSRF)
- SQL injection and other injection attacks
- Authentication and session bypass
- Sensitive data exposure
- Server-side request forgery (SSRF)

### Out of scope

- Denial of service (DoS/DDoS)
- Social engineering
- Vulnerabilities in third-party services or dependencies with existing public advisories
- Issues requiring physical access to the server

## Coordinated disclosure

We follow coordinated disclosure. Please don't publish details until a fix is available, unless we agree otherwise.

## For contributors

If you're contributing code, keep these in mind:

- Never commit secrets, private keys, or credentials.
- All network communication must use TLS.
- Security-relevant changes need tests, documentation updates, and threat model notes where applicable.
