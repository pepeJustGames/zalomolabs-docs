# Security Policy

Tags: `security` `responsible-disclosure` `secrets` `tokens` `public-docs`

Quick turn:

- [Public Branch Safety](#public-branch-safety)
- [Supported Reporting](#supported-reporting)
- [Responsible Disclosure](#responsible-disclosure)
- [Secret Rotation Notice](#secret-rotation-notice)
- [What Not To Send](#what-not-to-send)
- [Related Docs](#related-docs)

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
- screenshots showing private dashboards, user emails, tokens, database rows, or admin tools

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

Examples of values that should be rotated if exposed:

- Firebase API keys and service account files
- Google AI Studio keys
- OpenRouter keys
- Lemon Squeezy API keys or webhook secrets
- refresh tokens
- admin session files
- database passwords
- storage access tokens

## What Not To Send

Do not send:

- passwords
- raw private tokens
- full database dumps
- private user content not needed to reproduce the issue
- payment card details
- private keys

If a token is necessary to explain a bug, redact it and describe where it appeared.

## Related Docs

- [Terms of Service](TERMS.md)
- [Public API and Config Notes](docs/API_AND_CONFIG.md)
- [Contact](CONTACT.md)
