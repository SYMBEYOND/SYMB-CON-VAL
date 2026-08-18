# SYMB-FER T11 S04-R02 Replacement Provenance

Run: `S04-R02 replacement`  
Date: `2026-08-17 MDT`  
Artifact class: `RECEIVER_RUN_PROVENANCE`  
Evidence lane: `CONTROLLED_PORTABILITY`  
Lifecycle effect: `NONE`

## Receiver environment

- Provider family: B
- Provider: Claude
- Service: `claude.ai`
- Visible model: `Sonnet 5`
- Visible effort: `Medium`
- Session type: brand-new empty Claude Incognito chat
- Project status: outside Projects
- Style state: `DEFAULT_INITIAL_INCOGNITO_STATE`
- Explicit style label displayed: no
- Claude account instructions, memory, style, profile, and configuration changed for this run: no

## Delivery facts

John confirmed that:

- the governed frozen v0.4 packet was delivered inline as the first and only message;
- Claude's complete first response was copied;
- no follow-up, correction, continuation, regeneration, additional submission, or further retry occurred.

## Bound evidence

Receiver packet SHA-256:

`8dcc58b5be754d97b5e44e3a31c5313828574ecd7d72bd8c83f908c7040f7304`

Replacement pre-delivery environment screenshot SHA-256:

`410d145a071983465a0651b09a615ffbc0cbb3959575f2a2d07602295745cfd8`

Canonical replacement raw-response SHA-256:

`336c934701746984e51cbe9f5ffe5bd9f355c4d1d11133f23d73897ba39984f4`

Superseding wrong-input incident SHA-256:

`d75e5979380b7e05f88484eeef3b750c958d2e4b337102d08a8cae65c3e6b67a`

## Replacement lineage

This was the single separately authorized replacement following the preserved `ABORTED_NOT_SCORED_WRONG_INPUT` attempt.

The earlier wrong-input evidence remains unchanged and is not receiver evidence for the frozen v0.4 packet.

## Capture method and structural state

The receiver response was preserved using the verified two-stage clipboard method. The `pbpaste` capture command was positioned in Terminal before Claude's response was copied, and Return was pressed only after the complete response occupied the clipboard.

Capture integrity: `VALID`  
Receiver-output boundary: `ENTIRE_CAPTURE`  
Required starts-with labels: `0 / 10`  
Nonempty lines: `6`  
Shell-command signatures: `0`  
Structural gate: `FAIL`

The structural failure is recorded as observed provider behavior. No semantic score or overall T11 disposition is assigned by this provenance artifact.

## Limitations

- Provider and model identity derive from the visible interface and preserved pre-delivery evidence, not an API-level model identifier.
- The exact submission timestamp was not independently captured.
- Clipboard capture proves the preserved byte sequence but does not independently attest to provider infrastructure.
- No semantic inspection or scoring occurred during provenance filing.

## Exact stoppoint

The S04-R02 replacement response and provenance are governed and hash-bound. No receiver run, further retry, scoring, convergence, reconciliation, register revision, promotion, or lifecycle action is authorized or performed by this filing.
