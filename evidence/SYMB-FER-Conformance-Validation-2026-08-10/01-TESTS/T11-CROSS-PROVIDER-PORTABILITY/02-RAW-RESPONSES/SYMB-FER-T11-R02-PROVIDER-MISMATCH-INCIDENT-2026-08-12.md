# SYMB-FER T11 R02 Provider-Mismatch Incident

Test: T11 Cross-Provider Portability  
Planned run: R02  
Date: 2026-08-12 MDT  
Artifact class: `DELIVERY_AND_PROVIDER_SELECTION_INCIDENT`  
Disposition: `ABORTED_NOT_SCORED_PROVIDER_MISMATCH`  
Lifecycle effect: `NONE`

## Planned receiver

- Provider family: B
- Intended provider: Claude

## Observed receiver

- Actual provider: ChatGPT
- Visible model: 5.6 Sol Medium
- Confirming interface: ChatGPT Plus at `chatgpt.com`
- Clean receiver session: Confirmed by John

## Evidence

- Preserved response: `SYMB-FER-T11-R02-ABORTED-PROVIDER-MISMATCH-RAW-RESPONSE-2026-08-12.txt`
- Raw-response SHA-256: `f2a39e1f72ece47bd0c3cf575754b597c4a53db9c61d3427857c5353282404b1`
- Original Mac screenshot: `SYMB-FER-T11-R02-PROVIDER-MISMATCH-SCREENSHOT-2026-08-12.png`
- Original screenshot SHA-256: `3cda901a3853f38d87aa1709a41ec26d3c5d499dca8ad63e2219fcdf3844b09a`
- Original screenshot source: `/Users/user/Desktop/screenshots/2026-08/Week-02/Screenshot 2026-08-12 at 3.45.17 PM.png`

The screenshot visually establishes that the frozen packet was delivered to ChatGPT rather than Claude. The response is not Provider Family B evidence and must not be scored as T11 R02.

## Scope interpretation

John clarified that T01-through-T10 receiver work was conducted through ChatGPT. This does not invalidate those governed results because they did not claim cross-provider portability. T11 exists to test that remaining evidence gap.

## Cause and handling

The controller instructed John to use Claude without first verifying that a separate Claude service was open. John followed the packet-delivery procedure in a clean receiver chat. This is a controller-procedure and provider-selection incident, not a receiver capability failure.

The response and screenshot were preserved without scoring. No retry, R03, convergence review, closure, register revision, or lifecycle action occurred.

## Exact stoppoint

P04 is closed as `ABORTED_NOT_SCORED_PROVIDER_MISMATCH`. A valid Provider Family B run remains unperformed. Any replacement run requires separate explicit authorization.
