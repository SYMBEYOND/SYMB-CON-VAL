# SYMB-FER T11 S03-R02 Capture-Controller Failure Incident

Date: 2026-08-13 MDT  
Run: `S03-R02`  
Artifact class: `CAPTURE_CONTROLLER_FAILURE_INCIDENT`  
Lifecycle effect: `NONE`

## Incident

Claude produced one first response in the authorized clean S03-R02 session.

The capture controller attempted to collect interactive response input from inside a shell heredoc. The `cat` process inherited the heredoc input stream and preserved controller-script text instead of Claude receiver output.

This was a controller capture failure. It was not a Claude conformance failure.

## Controller-heredoc capture

Path:

`/Users/user/Desktop/SYMB-FER-Conformance-Validation-2026-08-10/01-TESTS/T11-CROSS-PROVIDER-PORTABILITY/06-BOUNDED-REPAIR/S03-V0.3-ADOPTED/02-RAW-RESPONSES/SYMB-FER-T11-S03-CAPTURE-STAGING-R02-2026-08-13.txt`

SHA-256:

`284c21ba7d569af8b731cf5089cd08a32c4058eda47db2525874dd18acaa1a9f`

Classification:

`CONTROLLER_HEREDOC_CAPTURE_NOT_RECEIVER_OUTPUT_NOT_SCORABLE`

The staging file remains unchanged as controller-failure evidence and must not be treated as receiver output.

## Canonical recovered response

Path:

`/Users/user/Desktop/SYMB-FER-Conformance-Validation-2026-08-10/01-TESTS/T11-CROSS-PROVIDER-PORTABILITY/06-BOUNDED-REPAIR/S03-V0.3-ADOPTED/02-RAW-RESPONSES/SYMB-FER-T11-S03-RAW-RESPONSE-R02-2026-08-13.txt`

SHA-256:

`78bb836c790094dec2bb34d416dc6dc46f050d81aca44e29ea07f0814fbbf612`

John preserved the same already-produced first Claude response through a direct clipboard recovery. No receiver rerun, follow-up, correction, or regeneration occurred.

The recovered response passed the structural capture gate:

- required starts-with labels: 10 / 10;
- nonempty response lines: 10;
- first boundary: `FIXTURE_RECOGNIZED:`;
- last boundary: `ACTION_TAKEN:`;
- shell signatures: 0.

## Recovery limitation

The controller did not preserve Claude's response during its initial input phase. The canonical artifact is a byte-identical filing copy of the separately verified Desktop recovery. This limitation must be carried into separately authorized provenance.

## Stoppoint

The canonical response, controller-heredoc capture, and this incident are preserved pending root-manifest regeneration and verified removal of the temporary Desktop recovery.

Provenance, semantic inspection, scoring, S03-R03, convergence, reconciliation, progress-register revision, T12, promotion, and lifecycle action remain unauthorized.
