# Security Policy

## Public Branch Safety

This branch must not contain:

- real `.env` files
- API keys
- refresh tokens
- admin session JSON files
- database dumps
- private user data
- payment provider secrets
- service account keys
- build artifacts containing secrets

## Supported Reporting

If you find a serious vulnerability, report it privately through the contact listed in [CONTACT.md](CONTACT.md).

Please include:

- affected product or page
- steps to reproduce
- expected impact
- screenshots or logs with private tokens removed

## Responsible Disclosure

Do not exploit, scrape, exfiltrate, or publicly disclose private data. Give the maintainers reasonable time to investigate and fix the issue.

## Secret Rotation Notice

If a token, refresh session, or API key is ever committed to any branch, assume it is compromised and rotate it from the provider dashboard.
