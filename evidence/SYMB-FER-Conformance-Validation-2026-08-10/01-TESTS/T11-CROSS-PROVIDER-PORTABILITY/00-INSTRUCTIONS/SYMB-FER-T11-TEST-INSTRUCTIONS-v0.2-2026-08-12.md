# SYMB-FER T11 Test Instructions

Test: T11 Cross-Provider Portability  
Version: v0.2  
Status: `CANDIDATE_NOT_ADOPTED_NOT_AUTHORIZED_FOR_FILING_OR_EXECUTION`  
Lifecycle effect: `NONE`

## Purpose

Test whether one byte-identical provider-neutral fixture preserves the same material semantic state in independent clean receiver environments without provider persona leakage or divergent canonical state.

This test uses sterile fictional state. It does not use or modify a private living token.

## Candidate files

1. `SYMB-FER-T11-RECEIVER-PACKET-v0.2-2026-08-12.txt`
2. `SYMB-FER-T11-SCORING-SHEET-v0.2-2026-08-12.md`
3. `SYMB-FER-T11-SEALED-ANSWER-KEY-v0.2-2026-08-12.md`

No final-result template is part of this candidate.

## Global rules

- Possession, review, or adoption of this package is not filing or execution authority.
- Every phase requires separate exact human authorization.
- Each authorization permits only the named phase.
- Stop after every phase and return its preserved evidence before requesting the next authorization.
- Do not coach, correct, clarify, regenerate, retry, score, compare, close, reconcile, or advance unless the corresponding phase is explicitly authorized.
- Provider and model identity are provenance only.
- Do not create provider-specific fixtures, prompts, directories, scoring standards, continuity lanes, or canonical branches.

## Planned receiver series

| Run | Receiver environment | Required independence |
|---|---|---|
| R01 | Provider family A, clean session 1 | No prior fixture or SYMB-FER context |
| R02 | Provider family B, clean session 1 | No prior fixture or SYMB-FER context |
| R03 | Provider family A, clean session 2 | New session independent of R01 |
| R04 | Provider family B, clean session 2 | New session independent of R02 |

The A/B labels are planning placeholders. Actual provider and visible model are recorded only in separate provenance notes.

## P01: Adoption decision

Precondition: John has completed his review of an exact candidate version.

Permitted action: John may explicitly adopt, reject, or request revision of that exact version.

Stoppoint: record the decision. Do not file or run anything.

## P02: Governed filing

Preconditions:

1. John explicitly adopted candidate v0.2 or a later exact version.
2. John separately authorizes filing that adopted package.

Permitted actions:

- verify the package and member hashes;
- file the adopted package into the governed T11 project structure;
- preserve any predecessor candidate unchanged;
- regenerate the governed root manifest;
- return a structured filing payload.

Stoppoint: the adopted package is filed and manifested. No receiver run is authorized.

## P03-P06: One receiver run per authorization

Each run requires its own exact authorization naming the run ID.

Run preconditions:

1. The adopted package is filed and byte verified.
2. The receiver-packet hash matches the adopted manifest.
3. The named receiver session is demonstrably clean.
4. The run is assigned to the planned provider-family position.
5. No scoring sheet, sealed answer key, or prior provider response is exposed to the receiver.

For the one authorized run only:

1. Start a new Temporary Chat or equivalent clean receiver session.
2. Do not mention SYMB-FER before the test message.
3. Paste the entire receiver packet inline as the first and only message.
4. Do not correct, coach, clarify, regenerate, or continue the response.
5. Copy the complete raw response exactly as returned.
6. Preserve it under `02-RAW-RESPONSES` using the neutral authorized run ID.
7. Preserve a separate provenance note containing provider, visible model, timestamp, timezone, delivery method, clean-session status, and receiver-packet hash.
8. Hash the preserved files, regenerate the governed root manifest, and return a structured run payload.

Mandatory stoppoints:

- After R01, do not run R02 or score anything.
- After R02, do not run R03 or score anything.
- After R03, do not run R04 or score anything.
- After R04, do not score anything.

## Receiver-run contamination rules

- Do not paste instructions, scoring material, answer keys, prior responses, or comparisons into a receiver chat.
- Do not use an existing conversation.
- Do not ask a receiver to revise its answer.
- Do not substitute regeneration for the original response.
- Do not reveal another receiver's output before all four raw responses are preserved.
- Do not count interface-generated text as receiver output.
- Do not use provider-specific prompt adaptations.

## Receiver-run abort conditions

Mark the authorized run `ABORTED_NOT_SCORED` when:

- the packet was incomplete;
- attachment intake replaced inline delivery;
- the session was not clean;
- coaching, continuation, regeneration, or correction occurred;
- the raw response was not preserved exactly;
- the packet hash differed from the adopted hash.

Preserve the incident evidence and stop. An aborted run is an evidence-handling incident, not an automatic capability failure. It does not authorize a replacement run.

## P07-P10: One scoring derivative per authorization

Scoring cannot begin until R01-R04 raw responses and provenance notes are preserved and verified.

Each scoring phase requires separate authorization naming exactly one run. For that run only:

1. Verify the raw-response and provenance hashes.
2. Use the adopted scoring sheet and sealed answer key.
3. Score only explicit evidence in the unchanged raw response.
4. Preserve observed omissions, inventions, drift, and provenance limitations.
5. Create and file one scored derivative.
6. Hash it, regenerate the governed root manifest, and return a structured scoring payload.
7. Stop without scoring another run.

## P11: Cross-run convergence

Preconditions:

- four verified raw responses;
- four verified provenance notes;
- four separately authorized and preserved individual scored derivatives;
- separate explicit authorization for convergence review.

Permitted action: compare material semantics across the four preserved runs using the adopted convergence gate and create one convergence derivative.

Stoppoint: preserve and verify the convergence derivative. Do not close T11 or create a final result.

## P12: Reconciliation and closure

Preconditions:

- all governed T11 run, provenance, scoring, and convergence evidence is present;
- separate explicit authorization for T11 reconciliation and closure.

Permitted action: reconcile the governed evidence and create one final-result artifact with a bounded disposition.

Stoppoint: T11 is closed or explicitly left open by the evidence. Do not revise the progress register or begin T12.

## P13: Progress reconciliation

Preconditions:

- governed T11 final result exists;
- separate explicit authorization for one progress-register revision.

Permitted action: create and file one provider-neutral progress-register successor while preserving predecessors unchanged, then regenerate the root manifest.

Stoppoint: the authorized register revision is filed and manifested. T12, final promotion, repository work, token creation, and lifecycle mutation remain unauthorized.
