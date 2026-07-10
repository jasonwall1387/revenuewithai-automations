# 02 — Appointment Booking Automation

An AI that reads an incoming message, **checks your real calendar for open slots, offers them, and books the appointment itself** — no back-and-forth, no phone tag.

▶️ **Watch the build:** _video coming soon_

## What it does
1. **Trigger** — an inbound message from a lead who wants to book (Webhook: SMS, form, or DM).
2. **AI reads intent** — returns structured data (wants_booking, preferred timeframe, service).
3. **Checks your calendar** — pulls real events from Google Calendar; no double-booking.
4. **Offers times** — AI writes a friendly reply with 2–3 real open slots and sends it.
5. **Books + confirms** — on the lead's reply, creates the calendar event and sends a confirmation.

## Prerequisites
- An [n8n](https://n8n.io) instance (cloud or self-hosted)
- An AI provider key (OpenAI or Anthropic)
- Google Calendar connected in n8n
- A send channel (Twilio for SMS, or email)

## Setup
1. In n8n: **Workflows → Import from File →** select `workflow.json`.
2. Connect your Google Calendar, AI provider, and send-channel credentials.
3. Copy `../.env.example` to `.env` and fill in your values (or set them as n8n credentials).
4. Add a few busy blocks to a test calendar so open-slot logic is visible.
5. **Test with a sample "can I book this week?" message** before going live.

## Customize
- Adjust the slot logic (business hours, buffer time, appointment length).
- Edit the AI prompts for tone and the questions it asks.
- Change the confirmation message and add reminders (a Wait node + second send).

## Notes
- Ships **without credentials** — you add your own.
- No real keys, numbers, calendar IDs, or client data are included. Find any? Open an issue.

---
Built by Revenue With AI. Want this set up on your calendar? [Free automation audit →](https://revenuewithai.com)
