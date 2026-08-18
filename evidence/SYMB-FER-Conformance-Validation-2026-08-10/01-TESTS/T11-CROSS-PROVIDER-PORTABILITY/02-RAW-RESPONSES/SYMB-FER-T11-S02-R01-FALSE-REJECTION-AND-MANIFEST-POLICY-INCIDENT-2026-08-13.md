# SYMB-FER T11 S02-R01 False-Rejection and Manifest-Policy Incident

Test: T11 Cross-Provider Portability  
Series and run: S02-R01  
Date: 2026-08-13 MDT  
Artifact class: `CONTROLLER_GATE_AND_MANIFEST_POLICY_INCIDENT`  
Lifecycle effect: `NONE`

## Authority and scope

John authorized one S02-R01 corrective filing only.

This record does not score the receiver response, create provenance, authorize another receiver run, perform convergence review, create a final result, revise a progress register, or change lifecycle state.

## Valid armed capture

The armed-waiting procedure successfully captured the receiver response before any later clipboard action.

The response contains exactly ten required labeled lines, zero shell-command signatures, `FIXTURE_RECOGNIZED:` as the first labeled line, and `ACTION_TAKEN:` as the final labeled line.

Captured bytes SHA-256:

`947fa8ed7d269471c5f69273dbfa597fe2e880c362e7941046aa8d0a11ca1a2a`

## False-rejection cause

The controller implementation combined fixed-text matching with a regular-expression start anchor. Fixed-text mode treated the anchor literally, so a structurally valid response was falsely classified under a `CAPTURE-REJECTED` filename.

The corrected gate uses an actual starts-with comparison and finds all ten labels exactly once with zero shell-command signatures.

The false-rejected source remains unchanged. A byte-identical canonical raw-response copy is filed separately.

## Root-manifest policy correction

The previous root manifest included mutable Finder `.DS_Store` metadata. Merely viewing project folders changed existing metadata and created additional metadata, causing manifest drift unrelated to governed project evidence.

Beginning with the root manifest produced by this correction:

- all files named `.DS_Store` are excluded;
- the root manifest excludes itself;
- files matching `SHA256-MANIFEST.tmp.*` are excluded;
- governed project artifacts remain included and byte-verifiable.

No `.DS_Store` file is deleted or modified.

## Temporary-manifest disposition

`SHA256-MANIFEST.tmp.1jr0hH` was created during the stopped false-rejection attempt. It was incomplete, non-authoritative, and never replaced the sealed root manifest.

John explicitly authorized removal of that exact temporary file after successful corrective regeneration.

## Exact stoppoint

S02-R01 has one structurally valid, byte-preserved canonical raw response. It remains semantically uninspected and unscored.

Provenance, S02-R02, scoring, convergence review, final-result creation, progress-register revision, and lifecycle action remain unauthorized.
