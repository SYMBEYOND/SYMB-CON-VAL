# SYMB-FER T01 Evidence Recovery Note

Test: T01 Boot Orientation  
Run: R01  
Date: 2026-08-10  
Status: RECOVERED USER-RELAYED RAW RESPONSE; ORIGINAL RECEIVER SESSION NOT RERUN  

## Reported condition

The local file initially named `SYMB-FER-T01-RAW-RESPONSE-R01-2026-08-10.txt` did not contain the receiver response. It contained the Terminal command block used to create the file because the clipboard held the wrong content when `pbpaste` ran.

Initial incorrect-capture SHA-256 reported by John:

`085cebd95a6ba9f5efb83921bafd6d0d6762ef3726018adea0fd886f37212cbf`

Initial incorrect-capture measurements reported by John:

- 6 lines
- 16 words
- 234 bytes

Read-only inspection confirmed that the file contained the `raw=...`, `pbpaste`, `wc`, and `shasum` Terminal commands rather than the receiver output.

## Recovery source

John pasted the complete nine-line receiver response into the active control conversation immediately after reporting the incorrect local capture. The recovered response file was transcribed from that user-relayed message without rerunning, correcting, or coaching the receiver.

Recovered artifact:

`SYMB-FER-T01-RECOVERED-RAW-RESPONSE-R01-2026-08-10.txt`

Source class:

`USER_RELAYED`

Authority and limitation:

- The recovered file is sufficient for semantic scoring of the nine visible response fields.
- It is not byte-authoritative evidence of the original receiver interface output.
- Formatting details not preserved in John’s pasted message must not be inferred.
- The original incorrect capture must be retained under a clearly labeled filename and must not be overwritten or deleted.

## Required local disposition

Rename the incorrect local capture to:

`SYMB-FER-T01-CAPTURE-ERROR-R01-2026-08-10.txt`

Place this recovery note and the recovered response beside it in the T01 raw-response directory. Update the project SHA-256 manifest afterward.

## Test effect

R01 may be semantically scored with the provenance qualifier `RECOVERED_USER_RELAYED`. It may not be used to validate exact byte preservation, exact line-ending behavior, or receiver-interface formatting.

