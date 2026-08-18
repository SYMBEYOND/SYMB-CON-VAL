# SYMB-FER Conformance Progress Register

Register version: v0.1  
Coverage: T01 through T06  
Date: 2026-08-11 MDT  
Artifact class: `PROVIDER_NEUTRAL_PROGRESS_REGISTER`  
Lifecycle effect: `NONE`

## Authority and scope

This register reconciles the frozen SYMB-FER Capability Conformance Matrix against the governed final results for T01 through T06.

It records existing results only. It does not rescore a receiver response, alter a governed result, activate or modify a token, create a ReFer checkpoint or successor, modify a repository, retrieve an external source, or authorize further testing.

`PASS_WITHIN_*_SCOPE` means that the named capability behaved correctly within the bounded fixture. It does not establish universal reliability, cross-provider portability, live external access, or final protocol promotion.

## Governed sources

| Source | Governed SHA-256 | Use in this register |
| --- | --- | --- |
| `SYMB-FER-CAPABILITY-CONFORMANCE-MATRIX-v0.1-2026-08-10.md` | `2968a7bedce644f7df2a59f8e8cbadd4e67140f2f2a3cbcfd26b17ebe729c1cb` | Frozen capability definitions, preliminary dispositions, repairs, prune decisions, and test order |
| `SYMB-FER-T01-FINAL-RESULT-v0.1-2026-08-10.md` | `4a762702224c4dcac879d15aedf901034d5af08c93f894d96b5f6964daedf8d0` | Governed T01 result |
| `SYMB-FER-T02-FINAL-RESULT-v0.1-2026-08-10.md` | `a93092c4ad46fb367f63eb5d471df42e615fba5beff699bc6f4c9a0e05f3abea` | Governed T02 result |
| `SYMB-FER-T03-FINAL-RESULT-v0.2-2026-08-11.md` | `92e78c5ceee826fdb6c44eae32fb0415ddc6ad65a78250a0db0ac95b7e598f5c` | Governed T03 result |
| `SYMB-FER-T04-FINAL-RESULT-v0.1-2026-08-11.md` | `4c4256da838164bc999f1c2ac69b5f90a2cde4f75c3dd979ee89bd6449ace53a` | Governed T04 result |
| `SYMB-FER-T05-FINAL-RESULT-v0.1-2026-08-11.md` | `94a3338a7c97826b71115da6d3234e5033a63e8521fee330d744ea5a5de33df3` | Governed T05 result |
| `SYMB-FER-T06-FINAL-RESULT-v0.1-2026-08-11.md` | `5803c034b04c12a570f833946d58f01a75c9b9d70e9ac17927e5755c61c870da` | Governed T06 result |

The sealed root manifest immediately before this register was prepared had SHA-256 `6d790646f715fc075d38e22494139294b0de14649d5704b8730fc9dc934d62a3`.

## Test progress

| Test | Governed result | Capability scope | Reconciled observation |
| --- | --- | --- | --- |
| T01 Boot Orientation | `PASS` | C01-C14 | The receiver preserved identity, collaboration posture, current and locked state, uncertainty, boundaries, exact next move, and non-action. R01 retains a provenance limitation. Attachment-only intake was excluded. |
| T02 Correction and Truth Handling | `PASS_WITH_PATCH` | C10-C13 | C10 and C11 passed within scope. C12 passed with a source-precedence patch. Both runs omitted the exact next action when no dedicated field existed, creating a C13 repair signal. |
| T03 Lifecycle and Acceptance | `PASS_WITH_PATCH` | C13, C16-C18 | C16-C18 passed within scope. A dedicated `NEXT_ACTION` field produced a successful C13 repair observation. Minor lifecycle narration drift did not reverse the correct state. |
| T04 Delta and Disposition | `PASS` | C19-C22 | R01 was preserved as a rejected delivery. R02 was the sole scored run and correctly handled predecessor reference, delta, disposition, bounded completeness, and loss risk. |
| T05 Evidence-Bounded ReFer | `PASS` | C21 | The non-activating checkpoint remained evidence-bounded. Capture error and recovery were preserved without rerunning the receiver. One external pointer detail was omitted without changing the bounded conclusion. |
| T06 External Source Recovery | `PASS` | C23-C26 | The receiver distinguished verified, ambiguous, missing, optional, hash-mismatched, and unavailable sources without retrieval or substitution. C24-C26 still require external support in live use. |

Progress count: six of twelve planned tests are closed. Four closed as `PASS`; two closed as `PASS_WITH_PATCH`.

## Capability progress register

| Capability | Current evidence state | Governing evidence | Reconciled note |
| --- | --- | --- | --- |
| C01 | `PASS_WITHIN_T01_SCOPE` | T01 | Human identity and callname preserved. |
| C02 | `PASS_WITHIN_T01_SCOPE` | T01 | Collaboration posture preserved. |
| C03 | `PASS_WITHIN_T01_SCOPE` | T01 | Communication and working posture preserved within the fixture. |
| C04 | `PASS_WITHIN_T01_SCOPE` | T01 | Current state preserved. |
| C05 | `PASS_WITHIN_T01_SCOPE` | T01 | Locked state and boundaries preserved in the bounded fixture. Broader repair testing remains relevant. |
| C06 | `PASS_WITHIN_T01_SCOPE` | T01 | Uncertainty remained explicit. |
| C07 | `PASS_WITHIN_T01_SCOPE` | T01 | Exact next move was preserved in T01. Dedicated-field robustness was tested again under C13. |
| C08 | `PASS_WITHIN_T01_SCOPE` | T01 | Authority and non-action boundaries held. |
| C09 | `PASS_WITHIN_T01_SCOPE` | T01 | Validation-before-action posture held. |
| C10 | `PASS_WITHIN_T02_SCOPE` | T01, T02 | Open questions and unresolved causes were preserved. |
| C11 | `PASS_WITHIN_T02_SCOPE` | T01, T02 | Current fact, historical statement, unsupported intent, and open state were separated. |
| C12 | `PASS_WITH_PATCH` | T01, T02 | Verified correction outranked stale history and unsupported intent. One run omitted explicit inference ordering. |
| C13 | `REPAIR_OBSERVED_SUCCESS` | T01, T02, T03 | T02 exposed loss of the next action without a dedicated field. T03's dedicated `NEXT_ACTION` field repaired that behavior in one bounded run. Further round-trip testing remains pending. |
| C14 | `PASS_WITHIN_T01_SCOPE` | T01 | Bounded fixture was read successfully. Oversize and enforced-budget behavior remains pending T10. |
| C15 | `UNTESTED` | Matrix only | Field-capsule behavior remains `KEEP_REPAIR_TEST`; no T01-T06 final result directly admits it. |
| C16 | `PASS_WITHIN_T03_SCOPE` | T03 | Candidate versus accepted-active lifecycle distinction held. |
| C17 | `PASS_WITHIN_T03_SCOPE` | T03 | Exact acceptance controlled activation. |
| C18 | `PASS_WITHIN_T03_SCOPE` | T03 | Single-active canonical lineage held. |
| C19 | `PASS_WITHIN_T04_SCOPE` | T04 | Predecessor reference worked without recursive predecessor copying. |
| C20 | `PASS_WITHIN_T04_SCOPE` | T04 | Added, changed, closed, and unchanged state was distinguished. |
| C21 | `PASS_WITHIN_T05_SCOPE` | T04, T05 | Evidence-bounded reconciliation and material loss risk were preserved. T05 adds direct bounded-ReFer evidence. |
| C22 | `PASS_WITHIN_T04_SCOPE` | T04 | Inline and external dispositions remained usable without false completeness. |
| C23 | `PASS_WITHIN_T06_SCOPE` | T06 | Complete verified pointers were distinguished from ambiguous pointers. Core candidacy remains conditional on pointer completeness and recoverability. |
| C24 | `PASS_WITHIN_T06_SCOPE_EXTERNAL_SUPPORT` | T06 | Required, optional, missing, and unavailable sources were classified correctly. Live recovery still requires external support. |
| C25 | `PASS_WITHIN_T06_SCOPE_EXTERNAL_SUPPORT` | T06 | Hash meaning was bounded to recorded byte identity. Live hash computation and verification require external support. |
| C26 | `PASS_WITHIN_T06_SCOPE_EXTERNAL_SUPPORT` | T06 | Unavailable history was not substituted as evidence. Live retrieval remains external support. |
| C27 | `UNTESTED` | Matrix only | Command contract remains `KEEP_REPAIR_TEST`; planned T07. |
| C28 | `PRUNE_CONFIRMED_BY_MATRIX` | Matrix only | Provider continuity branches are pruned. Provider and model may remain provenance metadata, not separate continuity lineages. |
| C29 | `UNTESTED` | Matrix only | Working-pattern control remains `KEEP_REPAIR_TEST`; planned T08. |
| C30 | `UNTESTED` | Matrix only | Artifact and module reference behavior remains `KEEP_REPAIR_TEST`; planned T09. |
| C31 | `MOVE_MODULE_AND_EXTERNAL_SUPPORT` | Matrix only | Operational environment inspection does not belong in the continuity core. |
| C32 | `MOVE_MODULE` | Matrix only | Specialized subsystem state belongs in a bounded module. |
| C33 | `MOVE_MODULE` | Matrix only | Project-specific schemas belong in modules, not the universal token core. |
| C34 | `PRUNE_LITERAL_RULE` | Matrix only | Literal carry-everything behavior is replaced by bounded disposition. |
| C35 | `PRUNE_UNBOUNDED_FORM_TEST_PENDING` | Matrix only | Unbounded full-read behavior is pruned. A bounded size budget still requires T10 validation. |
| C36 | `PRUNE_INLINE_SELF_HASH` | Matrix and governed practice | Integrity belongs in an external sidecar or root manifest, not an inline self-hash. |

## Repair and design observations

1. Dedicated fields matter. The exact next action weakened in T02 when embedded in another field and returned in T03 when `NEXT_ACTION` was explicit.
2. Delivery is part of the test boundary. T01 attachment intake and T04 R01 showed that receiving a file or instructions is not the same as receiving the fixture. Inline packet delivery is the current controlled method.
3. Capture errors do not require receiver retries when the original response can be recovered. T05 preserved both the failed capture and the recovered response.
4. A token can preserve source requirements and evidence boundaries, but it cannot independently retrieve unavailable sources, establish live authority, or compute current hashes without external support.
5. A scoped pass does not convert provider-specific behavior into a provider-specific continuity branch. Provider neutrality remains the canonical design direction.

## Frozen structural dispositions

The T01-T06 results do not reverse the matrix's structural decisions:

- Prune provider-specific continuity branches; retain provider/model as provenance metadata only.
- Prune literal preservation of every detail; use bounded inline, external, closed, missing-evidence, superseded, and pruned dispositions.
- Prune the unbounded full-read requirement; retain a future enforced size budget.
- Prune inline self-hash; use a sidecar or root manifest.
- Do not claim that prompt commands are deterministic software controls.
- Do not claim literal model-identity continuity. The protocol carries evidence-bounded human-LLM working continuity.

## Remaining controlled test sequence

| Planned test | Primary target | Current state |
| --- | --- | --- |
| T07 | C27 command contract | `NOT_STARTED` |
| T08 | C29 working-pattern control | `NOT_STARTED` |
| T09 | C30 artifact and module references | `NOT_STARTED` |
| T10 | C35 bounded size and read budget | `NOT_STARTED` |
| T11 | Cross-provider portability without provider lanes | `NOT_STARTED` |
| T12 | Successor round trip and final core reconciliation | `NOT_STARTED` |

No final core promotion should occur before the remaining tests and final reconciliation are complete.

## Stoppoint

T01 through T06 are reconciled without rescoring or mutation. The evidence currently supports the repeated continuity spine, the C13 dedicated-field repair, bounded delta and ReFer behavior, and explicit external-support boundaries.

The next planned activity is a separately authorized, read-only T07 design review for C27 and preparation of a sterile candidate package only. This register does not authorize that activity.
