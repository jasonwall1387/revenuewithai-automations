# Revenue With AI - Planned Automation Templates

This repository contains plans for three n8n automations for small and local businesses.
**No importable workflows have been published yet.** Each folder contains a design outline
and a `workflow.json.PLACEHOLDER` notice. There is no `workflow.json` to import or run.

| Planned example | Intended workflow | Status |
|---|---|---|
| [Lead follow-up](./01-lead-follow-up) | Acknowledge a new lead, log it, and follow up if appropriate | Planned; export and video unavailable |
| [Appointment booking](./02-appointment-booking) | Check availability, offer times, and confirm a selected slot | Planned; export and video unavailable |
| [Review requests](./03-review-requests) | Request a review after a completed service | Planned; export and video unavailable |

## What is available now

- Design outlines and proposed prerequisites in each folder's README.
- `.env.example` with illustrative placeholders, for planning only. No workflow reads it.
- A sanitization checklist in each placeholder file for the eventual export.

Please do not connect production accounts or submit customer data to these examples.
They have no executable implementation yet. There is no release date or publishing cadence promised.

## Before an example becomes ready to use

The maintainer must publish a sanitized `workflow.json`, replace its placeholder notice,
and document the tested n8n version and credential setup. Release verification must include:

1. Import into a clean n8n instance.
2. Execute the intended flow with synthetic inputs and test destinations.
3. Verify duplicate triggers, retries, and provider failures do not cause unintended repeat actions.
4. Document remaining limitations and actual outputs before claiming response times or booking guarantees.

Each example's README will contain installation instructions once its export is available.

## License

[MIT](./LICENSE). Use it, change it, ship it under the included license.

Built by Jason at [Revenue With AI](https://revenuewithai.com).
