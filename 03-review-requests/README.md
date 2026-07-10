# 03 — Review Request Automation

After a job is marked complete, automatically waits a day, then **texts the customer a friendly Google review link** — so you get more reviews without ever remembering to ask.

▶️ **Watch the build:** _video coming soon_ · (Covered as task #3 in the "5 tasks to automate first" video.)

## What it does
1. **Trigger** — a job/appointment is marked complete (Webhook, CRM status, or calendar event ended).
2. **Wait** — a set delay (e.g. 1 day) so the ask feels natural.
3. **Sends** a short, friendly review request with your Google review link (SMS and/or email).
4. **(Optional)** logs who was asked so you don't double-ask.

## Prerequisites
- An [n8n](https://n8n.io) instance (cloud or self-hosted)
- A send channel (Twilio for SMS, or email)
- Your Google review link (from your Google Business Profile)
- Optional: AI provider key if you want the message personalized

## Setup
1. In n8n: **Workflows → Import from File →** select `workflow.json`.
2. Connect your send-channel credentials.
3. Copy `../.env.example` to `.env` and add your review link + values.
4. Wire the trigger to however you mark jobs complete.
5. **Test on yourself** before sending to real customers.

## Customize
- Change the delay (same day vs. next morning tends to convert best).
- Personalize the message with the customer's name and the service done.
- Add a branch: only ask customers who rated the job positively (protect your rating).

## Notes
- Ships **without credentials** — you add your own.
- No real keys, numbers, review links, or client data are included. Find any? Open an issue.

---
Built by Revenue With AI. Want more 5-star reviews on autopilot? [Free automation audit →](https://revenuewithai.com)
