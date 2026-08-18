# SYMB-FER Conformance Progress Register

Register version: v0.2  
Coverage: T01 through T08  
Date: 2026-08-12 MDT  
Artifact class: `PROVIDER_NEUTRAL_PROGRESS_REGISTER`  
Lifecycle effect: `NONE`

## Authority and scope

This register reconciles the frozen SYMB-FER Capability Conformance Matrix against the governed final results for T01 through T08.

It records existing results only. It does not rescore or modify a receiver response or governed result, replace progress register v0.1, activate or modify a token, create a ReFer checkpoint or successor, adopt a working-pattern capsule, modify a repository, retrieve an external source, authorize T09, or authorize further testing.

`PASS_WITHIN_*_SCOPE` means that the named capability behaved correctly within its bounded fixture. It does not establish universal reliability, cross-provider portability, live external access, or final protocol promotion.

## Preserved predecessor register

`SYMB-FER-CONFORMANCE-PROGRESS-REGISTER-v0.1-2026-08-11.md` remains preserved unchanged with SHA-256 `ba3d3a36f25a6e2937c25a70c60a3e63ba6ef82138d9ee4d6219d109a924dd47`.

Register v0.2 is a new reconciliation artifact. It does not supersede or rewrite the bytes of v0.1.

## Governed sources

| Source | Governed SHA-256 | Use in this register |
|---|---|---|
| `SYMB-FER-CAPABILITY-CONFORMANCE-MATRIX-v0.1-2026-08-10.md` | `2968a7bedce644f7df2a59f8e8cbadd4e67140f2f2a3cbcfd26b17ebe729c1cb` | Frozen capability definitions, preliminary dispositions, repairs, structural prune decisions, and test order |
| `SYMB-FER-CONFORMANCE-PROGRESS-REGISTER-v0.1-2026-08-11.md` | `ba3d3a36f25a6e2937c25a70c60a3e63ba6ef82138d9ee4d6219d109a924dd47` | Preserved T01 through T06 predecessor register |
| `SYMB-FER-T01-FINAL-RESULT-v0.1-2026-08-10.md` | `4a762702224c4dcac879d15aedf901034d5af08c93f894d96b5f6964daedf8d0` | Governed T01 result |
| `SYMB-FER-T02-FINAL-RESULT-v0.1-2026-08-10.md` | `a93092c4ad46fb367f63eb5d471df42e615fba5beff699bc6f4c9a0e05f3abea` | Governed T02 result |
| `SYMB-FER-T03-FINAL-RESULT-v0.2-2026-08-11.md` | `92e78c5ceee826fdb6c44eae32fb0415ddc6ad65a78250a0db0ac95b7e598f5c` | Governed T03 result |
| `SYMB-FER-T04-FINAL-RESULT-v0.1-2026-08-11.md` | `4c4256da838164bc999f1c2ac69b5f90a2cde4f75c3dd979ee89bd6449ace53a` | Governed T04 result |
| `SYMB-FER-T05-FINAL-RESULT-v0.1-2026-08-11.md` | `94a3338a7c97826b71115da6d3234e5033a63e8521fee330d744ea5a5de33df3` | Governed T05 result |
| `SYMB-FER-T06-FINAL-RESULT-v0.1-2026-08-11.md` | `5803c034b04c12a570f833946d58f01a75c9b9d70e9ac17927e5755c61c870da` | Governed T06 result |
| `SYMB-FER-T07-FINAL-RESULT-v0.1-2026-08-11.md` | `35e483fea8ddf1b52f740f138963ff307332aa01a8d3a0bf46324fba00700f07` | Governed T07 result |
| `SYMB-FER-T08-FINAL-RESULT-v0.1-2026-08-12.md` | `0f7c7c279a7197c215ce699371694bbb84423b4e31310c20cc335494297eb832` | Governed T08 result |

The sealed root manifest immediately before this register was prepared had SHA-256 `350c706dca0a38f62ef5c3e18d380706bb9542a9c67283d7d3b9aca7a94c029d`.

## Test progress

| Test | Governed result | Capability scope | Reconciled observation |
|---|---|---|---|
| T01 Boot Orientation | `PASS` | C01-C14 | Two scored receivers preserved the semantic boot spine. R01 retains a provenance limitation; attachment-only R02 was excluded; direct R03 scored 20/20. |
| T02 Correction and Truth Handling | `PASS_WITH_PATCH` | C10-C13 | C10 and C11 passed within scope. C12 passed with a source-precedence completeness patch. Repeated omission of the exact next action created the C13 repair signal. |
| T03 Lifecycle and Acceptance | `PASS_WITH_PATCH` | C13, C16-C18 | C16-C18 passed within scope. A dedicated `NEXT_ACTION` field produced a successful bounded C13 repair observation. Lifecycle narration had minor completeness drift without state reversal. |
| T04 Delta and Disposition | `PASS` | C19-C22 | R01 remained a rejected delivery. Sole scored R02 correctly handled predecessor reference, bounded delta, disposition, missing evidence, loss risk, and resume state. |
| T05 Evidence-Bounded ReFer | `PASS` | C21 | The sole scored recovered response remained non-activating and evidence-bounded. One external-pointer detail was omitted without false completeness or state change. |
| T06 External Source Recovery | `PASS` | C23-C26 | The receiver distinguished supplied, verified-uninspected, missing, optional, hash-mismatched, recollected, and ambiguous sources without retrieval or substitution. |
| T07 Command Contract | `PASS` | C27 | The receiver treated `ReFer` and `Token` as governed natural-language procedures, enforced preconditions and refusal behavior, and performed no real command or lifecycle action. |
| T08 Working Pattern | `PASS` | C29 | R01 remained a rejected delivery incident. Sole scored R02 carried stable methods, current override, external and provisional dispositions, pruning, growth control, and human approval authority. The proposed capsule remains unadopted. |

Progress count: eight of twelve planned tests are closed. Six closed as `PASS`; two closed as `PASS_WITH_PATCH`.

## Capability progress register

| Capability | Current evidence state | Governing evidence | Reconciled note |
|---|---|---|---|
| C01 Human identity and callname | `PASS_WITHIN_T01_SCOPE` | T01 | Human identity and callname were preserved. |
| C02 Collaboration posture | `PASS_WITHIN_T01_SCOPE` | T01 | Active collaboration, direct reasoning, uncertainty, and bounded authority were preserved. |
| C03 Communication preferences | `PASS_WITHIN_T01_SCOPE` | T01 | Fixture-defined working and response preferences were preserved; current-instruction override behavior received additional support in T08. |
| C04 Relational language | `PASS_WITHIN_T01_SCOPE` | T01 | The bounded callname and collaboration relationship were carried without claiming literal model identity continuity. |
| C05 Lexicon | `PASS_WITHIN_T01_SCOPE` | T01 | Fixture shorthand remained usable in the bounded boot. Unbounded automatic lexicon growth remains disallowed by the matrix. |
| C06 Current state | `PASS_WITHIN_T01_SCOPE` | T01 | Current paused state and its evidentiary basis were preserved. |
| C07 Active work | `PASS_WITHIN_T01_SCOPE` | T01 | Active objective, blocker, and bounded next move survived the boot. Deep project-state growth remains governed by external disposition rules. |
| C08 Locked state and decisions | `PASS_WITHIN_T01_SCOPE` | T01 | Firmware and replacement locks were not reopened. |
| C09 Authorization boundaries | `PASS_WITHIN_T01_SCOPE` | T01 | No measurement, change, publication, purchase, or replacement was initiated. |
| C10 Open questions and uncertainty | `PASS_WITHIN_T02_SCOPE` | T01, T02 | Unresolved causes, evidence gaps, and authorization questions stayed open. |
| C11 Truth classes | `PASS_WITHIN_T02_SCOPE` | T02 | Current fact, historical statement, unsupported intent, correction, and open state were separated. |
| C12 Source precedence | `PASS_WITH_PATCH` | T02 | Verified correction outranked stale history and unsupported intent; one run omitted explicit inference ordering. |
| C13 Exact stoppoint and next action | `SUCCESSFUL_REPAIR_OBSERVATION` | T01, T02, T03 | T02 exposed loss without a dedicated field. T03 restored the exact bounded next action using `NEXT_ACTION`. Final round-trip robustness remains pending T12. |
| C14 Boot contract and boot response | `PASS_WITHIN_T01_SCOPE` | T01 | The bounded fixture produced accurate orientation. Oversize and enforced-budget behavior remain pending T10. |
| C15 Field capsule | `UNTESTED` | Matrix only | No governed T01-T08 final result directly tests compact field-capsule equivalence or conflict handling. |
| C16 Token lifecycle | `PASS_WITHIN_T03_SCOPE` | T03 | Candidate, accepted-active, and superseded states remained distinct. |
| C17 Explicit human acceptance | `PASS_WITHIN_T03_SCOPE` | T03 | Exact human acceptance controlled activation; self-declaration and intent did not. |
| C18 Single active canonical successor | `PASS_WITHIN_T03_SCOPE` | T03 | Exactly one accepted-active canonical token remained. |
| C19 Predecessor preservation | `PASS_WITHIN_T04_SCOPE` | T04 | The predecessor remained auditable without recursive body copying. |
| C20 Delta and resume | `PASS_WITHIN_T04_SCOPE` | T04 | Added, changed, closed, unchanged, loss-risk, and exact-resume state were distinguished. |
| C21 ReFer reconciliation | `PASS_WITHIN_T05_SCOPE` | T04, T05 | Evidence-bounded reconciliation, conflict preservation, missing evidence, and material loss risk were preserved. T05 directly tested the non-activating checkpoint behavior. |
| C22 Data disposition | `PASS_WITHIN_T04_SCOPE` | T04 | Material state was carried inline or assigned a usable external, missing-evidence, closed, or unchanged disposition. |
| C23 Modules and archive pointers | `PASS_WITHIN_T06_SCOPE` | T06 | Complete recorded pointers were distinguished from ambiguous or unusable pointers. Core use remains conditional on completeness and recoverability. |
| C24 Source manifest | `PASS_WITHIN_T06_SCOPE_EXTERNAL_SUPPORT` | T06 | Required, optional, unavailable, authority, identity, and recovery distinctions held. Live access remains external support. |
| C25 SHA-256 verification | `PASS_WITHIN_T06_SCOPE_EXTERNAL_SUPPORT` | T06 | Hash evidence was correctly limited to recorded byte identity. Live computation and verification remain external support. |
| C26 Self-bootstrap from prior history | `PASS_WITHIN_T06_SCOPE_EXTERNAL_SUPPORT` | T06 | Unavailable recollection was not substituted for authoritative evidence. Live retrieval remains external support. |
| C27 Natural-language command surface | `PASS_WITHIN_T07_SCOPE` | T07 | The bounded command contract correctly governed `ReFer`, `Token`, refusal, artifact class, and lifecycle effect without pretending to be deterministic software. |
| C28 Provider or model profiles | `PRUNE_CONFIRMED_BY_MATRIX` | Matrix, T07, T08 | Provider identity may remain provenance metadata. Provider continuity lanes and canonical provider roles remain pruned. |
| C29 Working-pattern continuity | `PASS_WITHIN_T08_SCOPE` | T08 | Stable methods remained inline while project recipes, provider experiments, provisional trials, and transient details received bounded dispositions. The proposed capsule remains unadopted. |
| C30 Artifact classes: FULL, LINKED, CHECKPOINT | `UNTESTED` | Matrix only | Planned T09 remains not started and unauthorized. |
| C31 Time and weather functions | `MOVE_MODULE_AND_EXTERNAL_SUPPORT` | Matrix only | Live environment facts are not continuity-core state and require live tools. |
| C32 Lightning workflow | `MOVE_MODULE` | Matrix only | Specialized implementation workflow remains outside the continuity core. |
| C33 Sterilization gate | `MOVE_MODULE` | Matrix only | Privacy review remains a release checklist or module, not a guarantee or boot-core function. |
| C34 Carry everything forward | `PRUNE_LITERAL_RULE` | Matrix, T04, T08 | Literal preservation is replaced by bounded inline, external, closed, missing-evidence, superseded, and pruned dispositions. |
| C35 Read the entire token without a size budget | `PRUNE_UNBOUNDED_FORM_TEST_PENDING` | Matrix only | The unbounded rule remains pruned. A bounded size and attention budget remains pending T10. |
| C36 Token containing its own final SHA-256 | `PRUNE_INLINE_SELF_HASH` | Matrix and governed practice | Integrity remains external in sidecars and manifests rather than a circular inline self-hash. |

## Repair and design observations

1. Dedicated fields materially improve preservation. C13 weakened when the next action was embedded in T02 and returned when T03 used an explicit `NEXT_ACTION` field.
2. Delivery is part of the controlled boundary. T01 attachment intake, T04 R01, and T08 R01 were preserved as delivery failures or incidents rather than misclassified as capability failures.
3. Capture failure is distinct from receiver failure. T05 recovered the original response without coaching, regeneration, or retry.
4. Bounded disposition prevents recursive growth. T04 and T08 support inline stable state plus explicit external, provisional, superseded, missing-evidence, and pruned dispositions.
5. Prompt-defined commands can be governed procedures but are not deterministic software. T07 supports a small documented command surface with explicit preconditions and refusal behavior.
6. A continuity artifact can carry source requirements and recovery behavior but cannot independently retrieve unavailable sources, establish live authority, or compute current hashes without external support.
7. Provider neutrality remains canonical. T07 and T08 did not create provider roles or continuity lanes.
8. A successful proposed derivative is not automatically adopted. T08 passed while its working-pattern capsule remained pending human judgment and explicitly unadopted.

## Frozen structural dispositions

The T01-T08 results do not reverse the matrix's structural decisions:

- Prune provider-specific continuity branches; retain provider and model only as provenance metadata.
- Prune literal preservation of every detail; use bounded disposition accounting.
- Prune the unbounded full-read requirement; retain a future enforced size budget.
- Prune inline self-hash; use an external sidecar or manifest.
- Do not claim prompt commands are deterministic software controls.
- Do not claim literal model-identity continuity.
- Keep live retrieval, live hash computation, time, weather, and unavailable-history recovery explicitly dependent on external support.
- Keep the proposed T08 working-pattern capsule unadopted unless separately reviewed and explicitly approved.

## Remaining controlled test sequence

| Planned test | Primary target | Current state | Required purpose |
|---|---|---|---|
| T09 | C30 artifact classes | `NOT_STARTED_NOT_AUTHORIZED` | Distinguish FULL, LINKED, and CHECKPOINT without claiming complete boot when required sources are missing. |
| T10 | C35 bounded size and read budget | `NOT_STARTED_NOT_AUTHORIZED` | Locate the practical omission or instruction-dilution boundary and establish an enforceable budget. |
| T11 | Cross-provider portability | `NOT_STARTED_NOT_AUTHORIZED` | Test the same provider-neutral fixture in independent receiver environments without creating provider lanes. |
| T12 | Successor round trip | `NOT_STARTED_NOT_AUTHORIZED` | Test candidate creation and fresh-receiver boot for material loss, altered locks, lineage ambiguity, and uncontrolled expansion. |

Eight of twelve planned tests are closed. No final core promotion should occur before T09 through T12 and final reconciliation are complete.

## Exact remaining evidence gap

The current record supports semantic boot, truth correction, lifecycle control, bounded predecessor and delta handling, evidence-bounded ReFer, external-source boundaries, command contracts, and working-pattern disposition.

It does not yet establish:

- correct artifact-class behavior for FULL, LINKED, and CHECKPOINT
- a measured, enforceable size and attention budget
- cross-provider semantic portability
- successor round-trip preservation
- final core-template promotion

## Stoppoint

T01 through T08 are reconciled without rescoring or mutation. Progress register v0.1 remains unchanged. The proposed T08 working-pattern capsule remains unadopted.

The next planned activity in the frozen matrix is T09 for C30, but this register does not authorize T09 design, package preparation, or execution.
