# Review Requests - Planned Example

**Status: design outline only. No importable workflow or build video is available.**
`workflow.json.PLACEHOLDER` marks where a future sanitized export would go.

## Intended flow

1. Receive a completed-service event.
2. Apply a configured delay and check whether a request has already been sent.
3. Send a neutral review request through an eligible contact channel.
4. Log the delivery outcome to prevent repeat requests.

Proposed integrations: n8n, a completion-event source, and SMS or email.
The exact credential and configuration requirements will be documented with the export.
Review eligibility should not depend on whether the customer gave positive feedback.

## Required before release

Validate a clean import, synthetic completed jobs, duplicate events, contact preferences,
delayed execution, and provider failures. No automated requests or delivery guarantees
are implemented in this repository yet.

See the [repository status](../README.md). Installation instructions will be added when
`workflow.json` is published; there is currently nothing to import or activate.
