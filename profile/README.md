# Contact OS

Contact OS is the communications layer of the [Caldrion](https://ventures.caldrion.com) studio: AI agents that answer the phones and the email of every studio company, so no caller or correspondent goes unanswered.

Caldrion Ventures combines venture capital with a hands-on studio that identifies opportunities, validates concepts and incubates businesses through launch and growth. Contact OS is shared infrastructure for those businesses.

**Links:** [Website](https://ventures.caldrion.com) · Portfolio project: TODO(confirm): link the "Caldrion" portfolio project once it exists

## What we build

| Product | What it does | Repository | Live |
|---|---|---|---|
| Telephony OS | Phone system for every studio number: AI receptionists (Twilio ConversationRelay, ElevenLabs voices, Claude), SMS, an MCP server for Claude, an admin dashboard and CRM call logging, on one Cloudflare Worker. | [contact-os/telephony-mcp](https://github.com/contact-os/telephony-mcp) (private) | MCP server and admin dashboard on `telephony-mcp.caldrion.workers.dev` |
| Email OS | AI agents that triage the email reaching every studio domain, draft or send replies within per-domain limits, log correspondence to the CRM, and expose an MCP server, dashboard and daily digest, on one Cloudflare Worker. | [contact-os/email-os](https://github.com/contact-os/email-os) (private) | MCP server and admin dashboard on `email-os.caldrion.workers.dev` |

Both products log activity to the studio CRM (`caldrion-com/crm`).

## How we work

- **Issue forms.** Every repository uses the org's default forms: Bug, Feature, Task, Epic and Initiative. New bugs and feature requests arrive labelled `needs-triage`.
- **Issue hierarchy.** Work is organised as **Initiative** (a portfolio-level outcome, a quarter or more) > **Epic** (a shippable body of work) > **Feature / Task / Bug**, linked with sub-issues. Blocking relationships are recorded as issue dependencies.
- **Labels.** Labels describe state and area, not type: `needs-triage`, `needs-info`, `blocked`, `security`, `documentation`, `dependencies`, plus `platform:*` (worker, mcp, web) and `area:*` labels per repository.
- **Project boards.** Each product has a GitHub Project named "Caldrion · <Product>" with Status (Backlog, Ready, In progress, In review, Done), Priority (P0–P3), Size (XS–XL) and two-week iterations.
- **Pull requests.** PRs use the default template and reference their issue with `Closes #<n>`, so merging closes the issue and moves it to Done.

## Contact

Use the contact options on [ventures.caldrion.com](https://ventures.caldrion.com). Please report security issues privately rather than in a public issue.

<sub>© Caldrion LLC. All rights reserved.</sub>
