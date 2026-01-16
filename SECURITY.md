# Security Policy

## Reporting a Vulnerability

**Do not open a public GitHub issue for security vulnerabilities.**

If you have discovered a security vulnerability in VotePeace, please send an email to the maintainer at `dava@example.com` (replace with actual contact). We will triage your report and respond within 48 hours.

## Supported Versions

| Version | Supported |
| :--- | :--- |
| Latest | ✅ |
| < 1.0.0 | ❌ |

## Security Best Practices for Users

1.  **Change Default Credentials**: Specifically for the seed Admin account.
2.  **HTTPS**: Always deploy behind a reverse proxy handling SSL/TLS.
3.  **Environment Variables**: Never share your `.env` files.
