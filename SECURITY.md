# Security Policy

## Reporting a Vulnerability

Please do not disclose security vulnerabilities publicly before they have been reviewed.

For security issues, contact:

`YOUR_SECURITY_EMAIL@example.com`

Include:

- A description of the issue
- Steps to reproduce
- Affected version
- Potential impact
- Any suggested mitigation

Do not include confidential customer documents or credentials in a report.

## Secret Management

Never commit:

- API keys
- Passwords
- Private keys
- Signing certificates
- License-generation secrets
- Production authentication secrets
- Internal infrastructure credentials

If a secret is accidentally committed, rotate/revoke it immediately and remove it from future revisions.
