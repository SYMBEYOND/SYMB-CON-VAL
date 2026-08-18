# SYMB-FER T02 Test Instructions

Test: T02 Correction and Truth Handling  
Version: v0.1  
Status: READY FOR CONTROLLED RECEIVER TEST  

## Purpose

Test whether a clean LLM receiver correctly applies a later verified correction to a stale statement while preserving the conflict record, maintaining open uncertainty, and respecting source precedence.

This test covers capabilities C10 through C12 only. It does not use or modify any private living token.

## Files

1. `SYMB-FER-T02-RECEIVER-PACKET-v0.1-2026-08-10.txt`
2. `SYMB-FER-T02-SCORING-SHEET-v0.1-2026-08-10.md`
3. `SYMB-FER-T02-SEALED-ANSWER-KEY-v0.1-2026-08-10.md`

## Operator procedure

1. Do not open the sealed answer key before preserving the raw receiver response.
2. Start one new Temporary Chat or equivalent clean receiver session.
3. Do not mention SYMB-FER before the test message.
4. Open the receiver packet locally and paste its complete text inline as the first and only message. Do not attach the packet as a file.
5. Do not correct, coach, clarify, or continue the receiver response.
6. Use the receiver interface copy control to copy the complete assistant response.
7. Before overwriting the clipboard or entering more Terminal commands, preserve that response as `SYMB-FER-T02-RAW-RESPONSE-R01-2026-08-10.txt`.
8. Verify the saved file begins with `CURRENT_FACT:` and contains all eight required labels.
9. Record the receiver provider, model if visible, date, time, and whether the session was demonstrably clean.
10. Only after the raw response is preserved, open the scoring sheet and sealed answer key.
11. Score only explicit evidence in the raw response. Do not award points for what the receiver may have intended.

## Contamination rules

- Do not paste the scoring sheet or answer key into the receiver chat.
- Do not use an existing conversation.
- Do not ask the receiver to revise its answer.
- Do not count suggested reply buttons or interface-generated text as part of the response.
- Preserve the raw output before discussing the result in another AI conversation.
- An attachment-intake acknowledgment is an aborted delivery attempt, not a scored response.

## Capture rejection rule

Reject and preserve separately any local capture that contains Terminal commands, prompt text, or an attachment acknowledgment instead of the receiver's eight-line answer. Do not overwrite or silently repair it.

## Stoppoint

Stop after one raw receiver response is preserved and verified for capture integrity. Return the raw response for independent scoring before running another receiver or changing the fixture.

