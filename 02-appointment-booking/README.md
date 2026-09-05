# Appointment Booking - Planned Example

**Status: design outline only. No importable workflow or build video is available.**
`workflow.json.PLACEHOLDER` marks where a future sanitized export would go.

## Intended flow

1. Receive a booking enquiry and identify the requested service and timeframe.
2. Check calendar availability and offer candidate times.
3. Recheck availability when the customer selects a time.
4. Create the appointment and report the confirmed result.

Proposed integrations: n8n, an AI provider, Google Calendar, and a reply channel.
The exact credential and configuration requirements will be documented with the export.

## Required before release

Validate a clean import, synthetic bookings, timezone handling, simultaneous requests
for the same slot, duplicate replies, and calendar/provider failures. The design outline
is not evidence of protection against double-booking; that behavior must be implemented
and tested before it is claimed.

See the [repository status](../README.md). Installation instructions will be added when
`workflow.json` is published; there is currently nothing to import or activate.
