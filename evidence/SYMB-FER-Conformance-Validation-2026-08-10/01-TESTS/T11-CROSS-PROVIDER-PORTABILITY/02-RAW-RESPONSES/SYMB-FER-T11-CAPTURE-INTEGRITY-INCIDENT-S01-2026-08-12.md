# SYMB-FER T11 S01 Capture-Integrity Incident

Test: T11 Cross-Provider Portability  
Series: S01  
Date: 2026-08-12 MDT  
Artifact class: `SUPERSEDING_EVIDENCE_INTEGRITY_RECORD`  
Disposition: `CAPTURE_INTEGRITY_FAILURE`  
Lifecycle effect: `NONE`

## Authority and scope

John authorized one capture-integrity corrective filing only.

This record preserves and supersedes the evidentiary interpretation of the S01 clipboard captures. It does not delete, overwrite, rescore, repair, or activate any predecessor artifact. It does not authorize a receiver run, scoring, convergence review, final result, progress-register revision, or lifecycle transition.

## Verified failure mechanism

The operator copied each receiver response. The controller then supplied a Terminal preservation block. Copying that block replaced the receiver response on the clipboard before the block invoked `pbpaste`.

The resulting files contain the Terminal preservation blocks rather than receiver responses.

All five captures independently showed:

- `0 / 10` expected response labels;
- seven shell-command signatures;
- first nonempty line `zsh -f <<'ZSH'`;
- last nonempty line `ZSH`.

This is a controller-designed capture failure, not a receiver capability failure and not an operator failure.

## Affected captures

| Claimed evidence role | SHA-256 | Correct disposition |
|---|---|---|
| R01 raw response | `00892fb6574fb2996155229158ae77cf9e3443fe44fc05219431880f08be61a7` | `CAPTURE_INTEGRITY_UNTRUSTED_NOT_SCORABLE` |
| Aborted R02 provider-mismatch raw response | `f2a39e1f72ece47bd0c3cf575754b597c4a53db9c61d3427857c5353282404b1` | `CAPTURE_INTEGRITY_UNTRUSTED_NOT_SCORABLE` |
| R02 Claude raw response | `d026a83ad303984dec537096fa454dcbc5e25e7081a40abd161a6bb3c2340ebb` | `CAPTURE_INTEGRITY_UNTRUSTED_NOT_SCORABLE` |
| R03 raw response | `bdd514da546e88659d79c319a6c66dea906edb58d162be78a48713b4a456d65a` | `CAPTURE_INTEGRITY_UNTRUSTED_NOT_SCORABLE` |
| R04 Claude raw response | `6242dd167fb518d93f1ead1e60da9d4df2f64941864af1667f6b3bfde46be423` | `CAPTURE_INTEGRITY_UNTRUSTED_NOT_SCORABLE` |

## Provenance correction

The preserved R01, R02, and R03 provenance artifacts correctly record their intended receiver environments but incorrectly state that receiver responses were successfully preserved.

Those claims are materially superseded by this incident record. The provenance files remain unchanged for auditability.

No R04 provenance artifact was created.

## Provider-mismatch evidence

The preserved provider-mismatch screenshot remains valid visual evidence that one attempted R02 delivery occurred in ChatGPT rather than Claude.

The associated clipboard capture is not a receiver response and is not scorable. The existing provider-mismatch incident remains valid regarding provider selection but is superseded regarding successful raw-response preservation.

## Current T11 receiver-evidence state

`ZERO_VALID_SCOREABLE_RAW_RESPONSES_PRESERVED`

The frozen v0.2 fixture, candidate package, design boundaries, provider assignments, and T01-through-T10 governed results are unaffected.

## Corrective disposition

A collision-safe replacement series named `S02` is required.

S02 must use an armed waiting capture prepared before packet delivery. No second command may be copied between copying the receiver response and capturing it.

Every S02 run requires separate explicit authorization.

## Exact stoppoint

S01 is preserved as capture-integrity evidence and is not scorable.

No S02 receiver run has occurred. No scoring, final result, progress-register revision, or lifecycle transition occurred.
