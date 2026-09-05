# Lead Follow-Up - Planned Example

**Status: design outline only. No importable workflow or build video is available.**
`workflow.json.PLACEHOLDER` marks where a future sanitized export would go.

## Intended flow

1. Receive a new lead from a website form.
2. Prepare an acknowledgement for the selected contact channels.
3. Log the lead and delivery outcome in a sheet or CRM.
4. Follow up only when the configured conditions permit it and no reply has arrived.

Proposed integrations: n8n, an AI provider, Twilio or email, and a sheet or CRM.
The exact credential and configuration requirements will be documented with the export.

## Required before release

Validate a clean import, a synthetic lead, reply detection, duplicate submissions,
provider failures, and retry behavior. Measure actual delivery time before publishing
a latency claim. The current repository does not implement or verify these behaviors.

See the [repository status](../README.md). Installation instructions will be added when
`workflow.json` is published; there is currently nothing to import or activate.
