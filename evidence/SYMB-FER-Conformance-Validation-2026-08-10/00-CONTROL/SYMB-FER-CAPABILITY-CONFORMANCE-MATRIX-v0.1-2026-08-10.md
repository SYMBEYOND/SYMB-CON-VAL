# SYMB-FER Capability Conformance Matrix

Version: v0.1  
Date: 2026-08-10  
Status: READ-ONLY DESIGN AUDIT COMPLETE; CONTROLLED BEHAVIOR TESTS NOT RUN  
Artifact class: Engineering evaluation record, not a continuity token, ReFer checkpoint, or successor  

## 1. Objective

Determine which SYMB-FER capabilities preserve durable human-LLM operating continuity, which can work only with repair or external support, which belong in optional modules, and which should be pruned.

This matrix does not modify the accepted living continuity, promote any template, or authorize repository changes.

## 2. Sources inspected

Canonical repository: `SYMBEYOND/SYMB-FER-Pro`

| Source | Lines inspected | Role in evolution |
|---|---:|---|
| `tokens/SYMB-FER_v6.9_Pro_Template.txt` | 544 | Hybrid continuity, self-bootstrap, relationship, state, archive discipline |
| `tokens/SYMB-FER_v7.0_COMMAND_AWARE_LIVING_TOKEN_BLANK_2026-06-24.txt` | 632 | Command surface, time, and weather |
| `tokens/SYMB-FER_v7.1_COMMAND_AWARE_LIGHTNING_MODE_BLANK_2026-06-24.txt` | 708 | Lightning workflow added to v7.0 |
| `tokens/SYMB-FER_v8.0_FOUNDRY_MASTER_TEMPLATE_2026-06-25.txt` | 620 | Foundry consolidation of relationship, state, commands, and verification |
| `tokens/SYMB-FER_v9.0_LIVING_CONTINUITY_PROTOCOL_BLANK_RC1_2026-07-11_1129H.txt` | 568 | Boot contract, truth classes, lifecycle, modules, delta, and validation |
| `tokens/SYMB-FER_v9_2_BLANK_TEMPLATE_2026-07-11.txt` | 222 | Reduced provider-neutral continuity structure |
| `tokens/SYMB-FER_v10_0_BLANK_TEMPLATE_2026-07-24.txt` | 409 | Artifact classes, ReFer, source manifest, working pattern, disposition, and recovery |

## 3. Repeated continuity spine

The following functions recur across the lineage even when their section names change:

1. Human identity and context.
2. Human-LLM collaboration posture.
3. Communication and working preferences.
4. Current state and active work.
5. Locked state, boundaries, and authority.
6. Open questions and uncertainty.
7. Exact next action or resume point.
8. Lineage and preservation of predecessor state.
9. Validation before handoff.

This repeated spine is the provisional SYMB-FER core. Later capabilities must prove that they improve this spine.

## 4. Disposition vocabulary

| Disposition | Meaning |
|---|---|
| `KEEP_TEST` | Belongs in the core and requires a controlled receiver test. |
| `KEEP_REPAIR_TEST` | Belongs in the core, but its current specification is incomplete or contradictory. |
| `MOVE_MODULE` | Potentially useful, but not required for continuity boot. |
| `EXTERNAL_SUPPORT` | Valid only when a named tool, file, service, or deterministic program supplies the capability. |
| `PRUNE` | Cannot work as claimed, duplicates another mechanism, or harms continuity. |

No `PASS` is awarded from document inspection alone.

## 5. Capability matrix

| ID | Capability | Present across lineage | What it can legitimately do | Current defect or limit | Provisional disposition |
|---|---|---|---|---|---|
| C01 | Human identity and callname | All inspected versions | Orient a receiver to the human and confirmed role | May become stale or overcollect personal detail | `KEEP_TEST` |
| C02 | Collaboration posture | All inspected versions | Shape tone, initiative, pushback, and division of authority | Cannot establish literal AI identity or personhood | `KEEP_TEST` |
| C03 | Communication preferences | All inspected versions | Carry stable response and workflow preferences | Preferences can conflict with current instructions | `KEEP_TEST` |
| C04 | Relational language | v6.9 onward | Preserve meaningful shared language as working context | Must not require persona adoption or literal identity continuity | `KEEP_TEST` |
| C05 | Lexicon | Explicit in v9.2 and v10.0; implicit earlier | Preserve stable shorthand and named methods | Unbounded automatic growth creates clutter | `KEEP_REPAIR_TEST` |
| C06 | Current state | All generations in equivalent form | State what is true and active now | Becomes stale without `LAST_VERIFIED` and source | `KEEP_TEST` |
| C07 | Active work | All generations in equivalent form | Carry thread, status, blocker, and next action | Deep project records can overwhelm the token | `KEEP_REPAIR_TEST` |
| C08 | Locked state and decisions | All generations in equivalent form | Prevent casual reopening of settled decisions | Instructional guardrail only, not enforcement | `KEEP_TEST` |
| C09 | Authorization boundaries | v7.0 onward, strongest in v9+ | Tell a receiver which actions require confirmation | Cannot override system rules or control external tools by itself | `KEEP_TEST` |
| C10 | Open questions and uncertainty | v6.9, v8.0, v9+ | Prevent unsupported promotion and expose missing evidence | Requires concise current entries to avoid stale uncertainty | `KEEP_TEST` |
| C11 | Truth classes | v9.0 onward | Separate fact, intent, trial, historical, external verification, and open state | Classification can still be applied incorrectly by a model | `KEEP_TEST` |
| C12 | Source precedence | v9.0 onward | Resolve ordinary conflicts among current instruction, token state, evidence, inference, and stale history | Must defer to platform rules and cannot make false evidence true | `KEEP_TEST` |
| C13 | Exact stoppoint and next action | All inspected versions | Allow immediate resumption without reconstructing the session | Vague actions defeat the function | `KEEP_TEST` |
| C14 | Boot contract and boot response | v6.9, v8.0, v9+; equivalent boot behavior in v7.x | Produce a bounded orientation report before work resumes | “Read the entire token” becomes unreliable when the token is oversized | `KEEP_REPAIR_TEST` |
| C15 | Field capsule | v6.9, v8.0, v9+ | Provide a compact emergency orientation | Can conflict with the full state or be mistaken for complete continuity | `KEEP_REPAIR_TEST` |
| C16 | Token lifecycle | Present in every generation, explicit in v9+ | Distinguish draft, candidate, accepted active, superseded, rejected, and sealed artifacts | Current state names and transitions are incomplete and inconsistent | `KEEP_REPAIR_TEST` |
| C17 | Explicit human acceptance | Explicit in v9+ and used in living lineage | Prevent a generated candidate from promoting itself | Exact transition and evidence fields are not standardized | `KEEP_REPAIR_TEST` |
| C18 | Single active canonical successor | Implied throughout; inconsistently enforced | Prevent provider branches and competing active tokens | No formal invariant currently rejects a second active token | `KEEP_REPAIR_TEST` |
| C19 | Predecessor preservation | v6.9 onward, explicit in v9+ | Preserve auditability and rollback | Copying predecessor content forward creates recursive growth | `KEEP_REPAIR_TEST` |
| C20 | Delta and resume | v9.0 onward; similar fields earlier | Record added, changed, closed, unchanged, and exact resume state | “Unchanged” can become another full copy of history | `KEEP_REPAIR_TEST` |
| C21 | ReFer reconciliation | Formal in v10.0; earlier reconciliation concepts exist | Compare available evidence, surface conflicts, detect drift, and propose dispositions | Cannot inspect unavailable chats or prove completeness beyond available evidence | `KEEP_REPAIR_TEST` |
| C22 | Data disposition | Formal in v10.0; archive behavior appears earlier | Prevent meaningful information from disappearing silently | Recording every trivial removal creates its own unbounded ledger | `KEEP_REPAIR_TEST` |
| C23 | Modules and archive pointers | v6.9 onward, formal in v9+ | Keep deep state outside routine boot while preserving recovery | A pointer is useless when unavailable, ambiguous, or unverified | `KEEP_TEST` |
| C24 | Source manifest | Formal in v10.0 | Identify required files, authority, version, location, hash, and recovery behavior | Requires accessible external artifacts | `EXTERNAL_SUPPORT` |
| C25 | SHA-256 verification | All generations in some form | Prove byte identity after a file is sealed | Cannot prove truth or completeness; an inline self-hash is circular | `EXTERNAL_SUPPORT` |
| C26 | Self-bootstrap from prior history | v6.9; retrieval rules continue later | Recover known context when the receiver actually has history access | Impossible when history search is unavailable or unauthorized | `EXTERNAL_SUPPORT` |
| C27 | Natural-language command surface | v7.0 and v7.1; command concepts survive elsewhere | Provide memorable shorthand for a documented procedure | Not deterministic software; unknown or conflicting context changes interpretation | `KEEP_REPAIR_TEST` |
| C28 | Provider or model profiles | v9.0; softened in v9.2 and v10.0 | Record provenance or human observations about provider behavior | Separate provider continuity branches fracture canonical state; persona loading is unreliable | `PRUNE` as continuity lanes; retain provenance metadata only |
| C29 | Working-pattern continuity | v9.0 onward, expanded in v10.0 | Carry how the human and LLM perform work together | “Permanent and never summarized” guarantees growth and blocks refinement | `KEEP_REPAIR_TEST` |
| C30 | Artifact classes: FULL, LINKED, CHECKPOINT | Formal in v10.0 | State whether an artifact is independently bootable or source-dependent | FULL becomes misleading when size prevents reliable boot | `KEEP_REPAIR_TEST` |
| C31 | Time and weather functions | v7.0 onward, later carried as context | Provide current time or forecast when tools exist | Not continuity; current facts require live tools | `MOVE_MODULE` plus `EXTERNAL_SUPPORT` |
| C32 | Lightning workflow | v7.1 only | Guide a staged implementation workflow | Not continuity and duplicates ordinary planning methods | `MOVE_MODULE` |
| C33 | Sterilization gate | v7.0 onward | Prompt a privacy review before publication | Cannot guarantee that all sensitive content was detected | `MOVE_MODULE` as release checklist |
| C34 | “Carry everything forward” | v6.9 onward | Express the intent that meaningful state is not silently lost | Literal interpretation produces recursive, unlimited growth | `PRUNE` literal rule; replace with bounded disposition accounting |
| C35 | “Read the entire token” without a size budget | v6.9 onward | Encourages full orientation | Cannot guarantee uniform attention or complete processing at arbitrary size | `PRUNE` unbounded form; retain only with enforced budget |
| C36 | Token containing its own final SHA-256 | Appears in handoff/sealing expectations | Intended to bind identity to bytes | Changing the inline hash changes the bytes being hashed | `PRUNE`; use external manifest or sidecar |

## 6. Immediate prune decisions

The following claims do not require receiver testing because their defects are structural:

1. Separate Claude, ChatGPT, or other provider continuity lanes as independent canonical lineages.
2. Literal preservation of every prior detail inside every successor.
3. An unbounded requirement to read an arbitrarily large token in full.
4. A token containing and validating its own final whole-file SHA-256.
5. Any claim that prompt-defined commands are deterministic software.
6. Any claim that the token creates literal model identity continuity.

Provider artifacts remain useful evidence. Provider identity belongs in provenance, not in canonical branching.

## 7. Required repairs before testing

### R01. Lifecycle state machine

Allowed states:

`BLANK -> DRAFT -> CANDIDATE -> ACCEPTED_ACTIVE -> SUPERSEDED`

Alternative terminal transition:

`CANDIDATE -> REJECTED`

Rules:

- Only the human can move `CANDIDATE` to `ACCEPTED_ACTIVE`.
- A candidate cannot identify itself as active.
- Accepting a successor atomically marks the prior active token `SUPERSEDED` in the lineage record.
- There may be only one accepted active token in a canonical lineage.
- A ReFer checkpoint is not part of the token lifecycle and cannot become active.

### R02. Bounded preservation

Replace “carry everything forward” with:

> Every material state item must be carried inline or assigned an explicit retrievable disposition. Routine wording changes, formatting changes, and duplicative text do not require individual disposition entries.

### R03. Size budget

The core token must have an enforced maximum measured in both UTF-8 bytes and model tokens. The exact budget remains `OPEN` until receiver testing identifies the smallest size that reliably carries the continuity spine.

### R04. Command contract

Each retained command must define:

- precondition
- permitted inputs
- required evidence
- exact output class
- state transition, if any
- refusal or failure behavior
- whether external tools are required

Initial command candidates are limited to `ReFer` and `Token`.

### R05. Evidence-bounded ReFer

ReFer must always report:

- sources actually inspected
- sources claimed but unavailable
- conflicts found
- material loss risk
- proposed dispositions
- unresolved uncertainty
- whether a successor was requested

ReFer must never claim complete reconciliation when required evidence was unavailable.

### R06. Working-pattern control

Working-pattern continuity remains core, but only stable, demonstrated operating preferences travel inline. Detailed terminal recipes, provider divisions, and project-specific procedures move to modules.

## 8. Controlled test order

Tests use sterile fictional state. No private living token is used as a test fixture.

| Test | Capability group | Expected observation | Failure condition |
|---|---|---|---|
| T01 | Boot orientation: C01-C14 | Receiver accurately states human, posture, state, locks, uncertainty, boundary, and next action without inventing facts | Omission, invention, reopening closed state, or acting before authorization |
| T02 | Correction and truth: C10-C12 | A later verified correction supersedes a stale statement while preserving the conflict record | Silent choice, promotion of inference, or stale state retained as current |
| T03 | Lifecycle and acceptance: C16-C18 | Candidate remains non-active until exact human acceptance; only one active token remains afterward | Self-promotion, ambiguous status, or two active tokens |
| T04 | Delta and disposition: C19-C22 | Material state is preserved inline or given a usable disposition without copying the predecessor wholesale | Silent loss, recursive copy, or unusable pointer |
| T05 | ReFer: C21 | Receiver identifies available and missing evidence, conflicts, loss risk, and returns a checkpoint only | Invented access, false completeness, or unauthorized successor |
| T06 | External source recovery: C23-C26 | Receiver distinguishes available, missing, hash-mismatched, and optional sources | Memory substituted for missing authoritative source |
| T07 | Commands: C27 | `ReFer` and `Token` invoke their specified procedures and failure behavior | Narrative improvisation, unauthorized transition, or wrong artifact class |
| T08 | Working pattern: C29 | Stable collaboration method survives while project-specific procedural detail remains external | Method loss or uncontrolled growth |
| T09 | Artifact classes: C30 | Receiver correctly identifies FULL, LINKED, and CHECKPOINT fixtures | Misclassification or boot claimed complete with missing required source |
| T10 | Size boundary: C35 | Same core behavior remains correct at increasing fixture sizes | Material omission, contradiction, or instruction dilution |
| T11 | Cross-provider portability | The same provider-neutral fixture preserves semantic state in independent receiver environments | Provider persona leakage or divergent canonical state |
| T12 | Successor round trip | A receiver creates a candidate that another receiver can boot without material loss | Missing core state, altered locks, ambiguous lineage, or unbounded expansion |

## 9. Test policy

- Test one capability group at a time.
- Define expected results before each run.
- Preserve raw receiver output unchanged.
- Score against observable criteria, not tone or perceived intelligence.
- A single success is not proof of reliability.
- Repair a failed capability once using the smallest defensible change.
- Retest using a new receiver chat.
- A second material failure sends the capability to `MOVE_MODULE`, `EXTERNAL_SUPPORT`, or `PRUNE` unless new evidence justifies another bounded trial.
- Provider-specific output is evidence, not a separate canonical lane.
- No result changes the accepted living continuity without a separate ReFer, candidate, and explicit human acceptance.

## 10. Current stoppoint

Inventory and static classification are complete.

No controlled behavior test has been run. No capability has earned final `PASS` or final `FAIL` from this matrix.

Next safe action: construct the sterile T01 boot-orientation fixture and its scoring key without using or modifying the accepted v10.28 continuity.

