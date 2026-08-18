# SYMB-FER T04 Test Instructions

Test: T04 Delta and Disposition  
Version: v0.1  
Status: CANDIDATE FOR CONTROLLED REVIEW  

## Purpose

Test whether a clean LLM receiver preserves a predecessor as an auditable reference, records a bounded material delta, assigns usable dispositions to external state, exposes unavailable evidence and loss risk, and returns an exact resume action without copying the predecessor wholesale.

This sterile fixture covers C19 through C22 only. It does not use or modify any private living token.

## Files

1. `SYMB-FER-T04-RECEIVER-PACKET-v0.1-2026-08-11.txt`
2. `SYMB-FER-T04-SCORING-SHEET-v0.1-2026-08-11.md`
3. `SYMB-FER-T04-SEALED-ANSWER-KEY-v0.1-2026-08-11.md`
4. `SYMB-FER-T04-SHA256-MANIFEST-v0.1-2026-08-11.txt`

## Operator procedure

1. Do not open the sealed answer key before preserving the raw receiver response.
2. Verify the four governed test files against the supplied SHA-256 manifest before the run.
3. Start one new Temporary Chat or equivalent clean receiver session.
4. Do not mention SYMB-FER before the test message.
5. Open the receiver packet locally and paste its complete text inline as the first and only message; do not attach the packet as a file.
6. Do not correct, coach, clarify, or continue the receiver response.
7. Use the receiver interface copy control to copy the complete assistant response.
8. Before overwriting the clipboard or entering more Terminal commands, preserve the response as `SYMB-FER-T04-RAW-RESPONSE-R01-2026-08-11.txt`.
9. Verify that the saved response begins with `PREDECESSOR_REFERENCE:` and contains all eleven required labels.
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

Reject and preserve separately any local capture containing Terminal commands, prompt text, or an attachment acknowledgment instead of the receiver's eleven-line answer. Do not overwrite or silently repair it.

## Stoppoint

Stop after one raw receiver response is preserved and verified for capture integrity. Return the raw response for independent post-capture scoring before running another receiver or changing the fixture.
