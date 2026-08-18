# SYMB-FER T09 Test Instructions

Test: T09 Artifact Classes  
Fixture version: v0.1  
Capability scope: C30  
Status: STERILE CONTROLLED CANDIDATE

## Objective

Test whether a clean receiver distinguishes `FULL`, `LINKED`, and `CHECKPOINT` from their actual contents and dependencies rather than trusting a self-declared class.

## Receiver conditions

1. Use one brand-new Temporary Chat.
2. Paste the receiver packet inline as the first message.
3. Do not upload the ZIP or any individual file.
4. Do not add a preamble, explanation, coaching, or follow-up.
5. Do not use prior memory, browsing, tools, repositories, or external sources.
6. Preserve the complete receiver response before opening the sealed answer key or scoring.
7. Do not retry or repair the receiver response.

## Required response integrity

The receiver must return exactly twelve nonblank labeled lines, in the order specified by the packet:

1. `CLASS_RULE`
2. `F01_CLASS`
3. `F01_BOOT`
4. `L01_CLASS`
5. `L01_BOOT`
6. `C01_CLASS`
7. `C01_LIFECYCLE`
8. `D01_CLASS`
9. `D01_LIMIT`
10. `SOURCE_BOUNDARY`
11. `NEXT_ACTION`
12. `ACTION_TAKEN`

## Test-control boundaries

- The fixture is fictional and test-only.
- No private living continuity token is supplied or modified.
- The requested response is an `ARTIFACT_CLASS_CONFORMANCE_RECORD`, not a continuity token, boot artifact, checkpoint, plan, or successor.
- No artifact is activated or adopted by classification.
- No external source is retrieved.
- No repository or lifecycle state is modified.

## Capture rejection

If the receiver receives Terminal instructions, the ZIP, an attachment-only delivery, or anything other than the exact inline receiver packet, preserve the event as a rejected delivery. Do not score it as a receiver run.

