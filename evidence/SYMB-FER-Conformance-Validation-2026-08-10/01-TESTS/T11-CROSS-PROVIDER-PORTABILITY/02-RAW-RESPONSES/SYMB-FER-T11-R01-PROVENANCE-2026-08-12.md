# SYMB-FER T11 R01 Provenance

Test: T11 Cross-Provider Portability  
Run: R01  
Date: 2026-08-12 MDT  
Artifact class: `RECEIVER_RUN_PROVENANCE`  
Lifecycle effect: `NONE`

## Receiver environment

- Provider family: A
- Provider: ChatGPT
- Visible model: ChatGPT 5.6
- Session type: Temporary Chat
- Clean session with no prior messages: Confirmed by John
- Exact receiver timestamp: Not separately recorded
- Raw-response preservation timestamp: 2026-08-12 15:38:28 1346

## Delivery confirmation

- Frozen receiver packet pasted inline as the first and only message: Confirmed by John
- Receiver packet SHA-256: `538ad83bdea70580e81e161945663336f93ac3d149d8e89d60386ba7ac7d702d`
- Coaching, continuation, correction, or regeneration before capture: None
- First receiver response copied completely: Confirmed by John

## Preserved raw evidence

- Raw response: `SYMB-FER-T11-RAW-RESPONSE-R01-2026-08-12.txt`
- Raw-response SHA-256: `00892fb6574fb2996155229158ae77cf9e3443fe44fc05219431880f08be61a7`
- Raw response remained uninspected and unscored during P03 preservation.

## Post-run controller incident

After copying the receiver response, John entered the status phrase `R01 response copied` into Terminal rather than the controller chat. Zsh treated the phrase as an unknown command. Strict shell options previously enabled by the controller command then ended that shell process.

The clipboard remained intact, and the original receiver response was subsequently preserved through `pbpaste`. This was a controller-command and operator-interface incident after the receiver response, not receiver contamination or a capability failure.

No retry, second response, coaching, scoring, or fixture modification occurred.

## Stoppoint

R01 raw evidence and provenance are preserved. R02, scoring, convergence review, closure, progress reconciliation, and lifecycle action remain unauthorized.
