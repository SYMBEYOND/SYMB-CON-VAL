# SYMB-FER T11 S04-R01 Provenance

Test: T11 Cross-Provider Portability  
Fixture version: v0.4  
Series and run: S04-R01  
Date: 2026-08-13 MDT  
Artifact class: `RECEIVER_RUN_PROVENANCE`  
Evidence lane: `CONTROLLED_PORTABILITY`  
Eligibility: `ELIGIBLE_FOR_CONTROLLED_SCORING`  
Lifecycle effect: `NONE`

## Confirmed receiver environment

- Provider family: A
- Provider: ChatGPT
- Service: `chatgpt.com`
- Visible model: `UNKNOWN`
- Visible effort: `Medium`
- Session type: brand-new empty ChatGPT Temporary Chat
- Project status: outside Projects
- Transcript before delivery: empty
- Independence: controlled session 1

The visible interface did not expose a model name in the preserved pre-delivery evidence. No model identity is inferred.

Temporary Chat is an observable minimized-context control condition. It is not proof that every account-level instruction, provider context, or safety-relevant context was absent.

## Delivery confirmation

John confirmed:

- the frozen v0.4 packet was pasted inline as the first and only message;
- the packet was submitted once;
- ChatGPT complete first response was copied;
- no follow-up, correction, continuation, regeneration, or retry occurred.

## Frozen receiver packet

- Filename: `SYMB-FER-T11-RECEIVER-PACKET-v0.4-2026-08-13.txt`
- SHA-256: `8dcc58b5be754d97b5e44e3a31c5313828574ecd7d72bd8c83f908c7040f7304`

## Pre-delivery environment evidence

- Filename: `SYMB-FER-T11-S04-R01-PRE-DELIVERY-ENVIRONMENT-2026-08-13.png`
- SHA-256: `8599a512932f03eac97576fc705589b361d6a7d592625dff8fd90a4e3942fc5e`
- Local source bytes: `469834`

The governed screenshot is a byte-identical copy of the untouched Mac original. A separately uploaded relay copy had different bytes and was not admitted as governed evidence.

The screenshot establishes `chatgpt.com`, an empty Temporary Chat, outside-Project placement, and visible effort Medium. The visible model remains `UNKNOWN`.

## Canonical receiver output

- Filename: `SYMB-FER-T11-S04-RAW-RESPONSE-R01-2026-08-13.txt`
- SHA-256: `c1c32dce5d78dc88a1e294ee676b83f7ba96b6472f3c9f9703020922bc00253a`
- Bytes: `2161`
- Words: `284`
- Nonempty lines: `10`
- Required starts-with labels: `10 / 10`
- Structural label gate: `PASS`
- Boundary gate: `PASS`
- Shell-command signatures: `0`

No semantic inspection or scoring occurred during capture or provenance filing.

## Capture method and limitations

The verified two-stage non-heredoc method was used:

1. The frozen packet was placed on the clipboard only after hash verification.
2. John pasted and submitted it once in the verified receiver environment.
3. John copied the complete first response.
4. Before any other clipboard action, John manually typed `pbpaste > ~/Desktop/s04-r01.txt` in Terminal.
5. The recovery was structurally verified and filed byte-identically.
6. The temporary Desktop recovery was removed only after governed filing verification.

The clipboard remained a volatile transfer channel. The evidence establishes byte identity from the recovered clipboard file through governed filing, but it does not provide API-level provider attestation, an independently recorded submission timestamp, or proof that all account-level context was absent.

## Eligibility determination

S04-R01 satisfies the adopted v0.4 controlled minimized-context requirements and is eligible for later controlled scoring.

Eligibility does not constitute a semantic pass, scoring result, convergence result, final result, or lifecycle transition.

## Exact stoppoint

S04-R01 environment evidence, canonical raw response, and provenance are governed and verified.

S04-R02, semantic scoring, convergence, reconciliation, progress-register revision, T12, core or token promotion, and lifecycle action remain unauthorized.
