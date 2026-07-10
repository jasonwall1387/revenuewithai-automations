# 01 — Lead Follow-Up Automation

Replies to every new lead with a personalized **text and email within ~30 seconds**, logs the lead, and sends an automatic follow-up nudge if they don't reply.

▶️ **Watch the build:** _video coming soon_

## What it does
1. **Trigger** — new lead from your website form (Webhook).
2. **AI** writes a warm, personalized message using the lead's name + requested service.
3. **Sends** the message by SMS (Twilio) and email.
4. **Logs** the lead to a Google Sheet / CRM.
5. **Follow-up** — if no reply in 1 hour, sends one friendly nudge.

## Prerequisites
- An [n8n](https://n8n.io) instance (cloud or self-hosted)
- An AI provider key (OpenAI or Anthropic)
- Twilio account + a phone number (for SMS)
- An email account / SMTP (for email)
- A Google Sheet or CRM to log leads

## Setup
1. In n8n: **Workflows → Import from File →** select `workflow.json`.
2. Open each credential-using node and connect **your** accounts.
3. Copy `../.env.example` to `.env` and fill in your values (or set them as n8n credentials).
4. Point the Webhook at your website form.
5. **Test with a fake lead** (use your own phone) before going live.

## Customize
- Edit the AI prompt to match your brand voice and services.
- Change the follow-up delay (the Wait node) to fit your business.
- Add channels (WhatsApp, Slack) by duplicating the send node.

## Notes
- This template ships **without credentials** — you add your own.
- No real keys, numbers, or client data are included. If you ever find any, open an issue.

---
Built by Revenue With AI. Want this set up for your business? [Free automation audit →](https://revenuewithai.com)
