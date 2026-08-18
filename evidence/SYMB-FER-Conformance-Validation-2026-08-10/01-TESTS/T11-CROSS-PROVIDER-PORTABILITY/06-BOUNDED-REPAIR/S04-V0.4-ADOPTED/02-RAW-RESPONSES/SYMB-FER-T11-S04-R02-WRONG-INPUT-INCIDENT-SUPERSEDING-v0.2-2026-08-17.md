# SYMB-FER T11 S04-R02 Superseding Wrong-Input Incident

Run: `S04-R02`
Date: `2026-08-17 MDT`
Artifact class: `SUPERSEDING_DELIVERY_INPUT_MISMATCH_INCIDENT`
Lifecycle effect: `NONE`

## Supersession boundary

- Incomplete predecessor SHA-256: `5c3301fe05faa369098479e50fb1eb5eec0a45261d4331723395cfc0997732b1`
- The predecessor remains preserved unchanged.
- This record supersedes it only because its documented-facts bullets were omitted.
- Omission cause: zsh `print` interpreted leading hyphens as command options.

## Documented facts

- Pre-delivery screenshot SHA-256: `3efa10322b4413a84b39cf1e25e8e490034cb1cd9245a39351cbda1e2aeb1cdc`
- Intended frozen v0.4 receiver-packet SHA-256: `8dcc58b5be754d97b5e44e3a31c5313828574ecd7d72bd8c83f908c7040f7304`
- The first user message visibly delivered to Claude was the S04-R02 controlled launch payload.
- The frozen v0.4 receiver packet was not delivered.
- Preserved Claude raw-response SHA-256: `432ac59cd31f47e6abfa6f08931c5787a8b748ab5c96a6530ba81f46fe4aecd2`
- Wrong-input screenshot SHA-256: `1d8f74e8ce28acaff8f82632c795ad7951b33f0e4260d031d6001245c28367c8`
- The Claude response corresponds to the delivered controlled launch payload.

## Cause boundary

The mechanism that caused the controlled launch payload to become the delivered input is `UNKNOWN`.
No person, clipboard action, application, or controller step is assigned as the cause without evidence.

## Disposition

`ABORTED_NOT_SCORED_WRONG_INPUT`

This is a delivery-input mismatch, not a Claude capability failure.
The response is preserved as incident evidence and excluded from T11 scoring and convergence.

## Exact stoppoint

S04-R02 controlled receiver execution was not completed.
No retry, provenance, scoring, convergence, reconciliation, register revision, or lifecycle action occurred.
