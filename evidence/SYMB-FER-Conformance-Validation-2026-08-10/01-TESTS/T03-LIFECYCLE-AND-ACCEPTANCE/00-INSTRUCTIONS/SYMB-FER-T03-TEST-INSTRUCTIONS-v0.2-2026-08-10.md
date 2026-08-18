# SYMB-FER T03 Test Instructions

Test: T03 Lifecycle and Acceptance  
Version: v0.2  
Status: REPAIRED CANDIDATE FOR CONTROLLED RECEIVER TEST  

## Purpose

Test whether a clean LLM receiver correctly applies the repaired lifecycle state machine, requires exact human acceptance before activation, atomically supersedes the prior active token after valid acceptance, and preserves a single active canonical token.

This test covers capabilities C16 through C18 only. The `NEXT_ACTION` response field is an output-safety control and does not expand the scored capability scope. The fixture uses sterile fictional state and does not use or modify any private living token.

## v0.2 repair delta

- Corrected the verification instruction from three governed test files to four.
- Replaced the ambiguous `CURRENT_DECISION` response label with the explicit `NEXT_ACTION` label.
- No lifecycle facts, acceptance rules, lineage records, or scoring thresholds changed.

## Files

1. `SYMB-FER-T03-RECEIVER-PACKET-v0.2-2026-08-10.txt`
2. `SYMB-FER-T03-SCORING-SHEET-v0.2-2026-08-10.md`
3. `SYMB-FER-T03-SEALED-ANSWER-KEY-v0.2-2026-08-10.md`
4. `SYMB-FER-T03-SHA256-MANIFEST-v0.2-2026-08-10.txt`

## Operator procedure

1. Do not open the sealed answer key before preserving the raw receiver response.
2. Verify the four governed test files against the supplied SHA-256 manifest before the run.
3. Start one new Temporary Chat or equivalent clean receiver session.
4. Do not mention SYMB-FER before the test message.
5. Open the receiver packet locally and paste its complete text inline as the first and only message; do not attach the packet as a file.
6. Do not correct, coach, clarify, or continue the receiver response.
7. Use the receiver interface copy control to copy the complete assistant response.
8. Before overwriting the clipboard or entering more Terminal commands, preserve the response as `SYMB-FER-T03-RAW-RESPONSE-R01-2026-08-10.txt`.
9. Verify the saved response begins with `LIFECYCLE_RULE:` and contains all eight required labels.
10. Record the receiver provider, model if visible, date, time, and whether the session was demonstrably clean.
11. Only after the raw response is preserved, open the scoring sheet and sealed answer key.
12. Score only explicit evidence in the raw response; do not award points for what the receiver may have intended.

## Contamination rules

- Do not paste the scoring sheet, answer key, instructions, or manifest into the receiver chat.
- Do not use an existing conversation.
- Do not ask the receiver to revise its answer.
- Do not count suggested reply buttons or interface-generated text as part of the response.
- Preserve the raw output before discussing the result in another AI conversation.
- An attachment-intake acknowledgment is an aborted delivery attempt, not a scored response.
- Do not perform a second receiver run unless the first run is scored or formally rejected for capture integrity.

## Capture rejection rule

Reject and preserve separately any local capture that contains Terminal commands, prompt text, or an attachment acknowledgment instead of the receiver's eight-line answer. Do not overwrite or silently repair it.

## Stoppoint

Stop after one raw receiver response is preserved and verified for capture integrity. Return the raw response for independent post-capture scoring before running another receiver or changing the fixture.
