# AI Agents

DumbNotes may use AI-assisted moderation and investigation agents.

Public agent names:

- Kelvin: content and safety scanner
- Glace: moderation decision reviewer
- Flakes: bug and console investigation helper
- Cream: summaries and admin-readable reports

## Principles

- Agents should not expose private tokens or user secrets.
- Agents should write tickets and summaries for human review.
- High-risk actions should be reviewed by trusted admins.
- Client-side AI calls should be minimized to avoid quota issues and leaking prompts.
- Backend or admin workflows are better places for heavier analysis.

## Ticket Types

Possible public-safe ticket categories:

- moderation
- bug
- security
- summary
- internal command audit

## Limits

These docs do not expose internal prompts, private credentials, admin commands, or database access patterns that would weaken security.
