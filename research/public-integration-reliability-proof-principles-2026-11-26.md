# Integration reliability proof principles

26 November 2026. General engineering research and synthetic demonstration methodology. No customer results, internal repositories, contact information, private configuration or production claims.

A successful workflow invocation is not sufficient evidence that a destination record matches its intended source state. A useful integration demonstration can explicitly inject duplicate events, pre-commit failures, uncertain acknowledgements, ambiguous mappings, stale updates and independent destination drift.

## Demonstration boundaries

- Use synthetic inputs and isolated local data stores, with no external credentials or production writes.
- Give each event a stable identity and version, and distinguish an identical replay from a conflicting reuse of an identity.
- Where the destination actually supports it, record a durable receipt and update the destination atomically. A lost acknowledgement then requires receipt reconciliation, not a blind repeat of the write.
- If the destination cannot establish what happened, hold the event for explicit review. Real vendor idempotency, transaction and consistency guarantees vary.
- Bound retries, hold unclear mappings and verify the latest source version before delivery.
- Compare intended source state with actual destination state independently, even when historical delivery receipts are positive. Do not silently overwrite unexplained drift.
- Preserve actual test output and label mock fault injection, local restarts and synthetic records honestly. Local tests do not establish production security, throughput, uptime, vendor compatibility, distributed exactly-once guarantees or commercial savings.

## Evidence-led conversion

Use owned demonstrations or explicitly authorised professional examples to explain the delivery approach. Distinguish implementation evidence, historical release records and current production verification. Do not label prior employment work or prototype data as paying customer results. A bounded assessment can be useful when scope is uncertain; when requirements are clear, agree scope, responsibilities, acceptance, support and ownership directly.

This is a general methodology record, not a public sales offer, deployed integration or release authorisation.
