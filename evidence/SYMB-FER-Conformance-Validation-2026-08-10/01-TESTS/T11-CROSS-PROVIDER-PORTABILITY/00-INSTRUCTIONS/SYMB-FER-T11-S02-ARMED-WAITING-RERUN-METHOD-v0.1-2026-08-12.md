# SYMB-FER T11 S02 Armed-Waiting Rerun Method

Version: v0.1  
Date: 2026-08-12 MDT  
Artifact class: `CONTROLLED_PROCEDURAL_REPAIR`  
Status: `PREPARED_NOT_AUTHORIZED_FOR_EXECUTION`  
Lifecycle effect: `NONE`

## Purpose

Prevent clipboard replacement between receiver-response copying and raw-response preservation.

This method repairs the S01 capture procedure. It does not modify the frozen v0.2 fixture or authorize a receiver run.

## Replacement-series identity

Series: `S02`

Collision-safe raw-response filenames:

- `SYMB-FER-T11-S02-RAW-RESPONSE-R01-2026-08-12.txt`
- `SYMB-FER-T11-S02-RAW-RESPONSE-R02-2026-08-12.txt`
- `SYMB-FER-T11-S02-RAW-RESPONSE-R03-2026-08-12.txt`
- `SYMB-FER-T11-S02-RAW-RESPONSE-R04-2026-08-12.txt`

Corresponding provenance filenames use:

- `SYMB-FER-T11-S02-R01-PROVENANCE-2026-08-12.md`
- `SYMB-FER-T11-S02-R02-PROVENANCE-2026-08-12.md`
- `SYMB-FER-T11-S02-R03-PROVENANCE-2026-08-12.md`
- `SYMB-FER-T11-S02-R04-PROVENANCE-2026-08-12.md`

No S01 file may be overwritten, renamed, moved, or deleted.

## Provider sequence

| Run | Provider family | Provider | Independence |
|---|---|---|---|
| S02-R01 | A | ChatGPT at `chatgpt.com` | New Temporary Chat |
| S02-R02 | B | Claude at `claude.ai` | New empty Claude chat |
| S02-R03 | A | ChatGPT at `chatgpt.com` | New Temporary Chat independent of S02-R01 |
| S02-R04 | B | Claude at `claude.ai` | New empty Claude chat independent of S02-R02 |

## Required armed-waiting sequence

For each separately authorized run:

1. Prepare one run-specific Terminal block before opening the receiver.
2. Preflight the frozen packet hash, current root-manifest hash, predecessor evidence, provider assignment, and collision-safe destination.
3. Copy the frozen packet to the clipboard.
4. Keep the same Terminal block running at an explicit waiting prompt.
5. Switch to the confirmed clean receiver.
6. Paste the packet as the first and only message.
7. Copy the receiver's complete first response.
8. Return to the waiting Terminal.
9. Press `Return` only. Do not copy or type another command.
10. The already-running block immediately captures the clipboard into a temporary file.
11. Apply the structural capture gate before filing.
12. Preserve, hash, and report the raw response.
13. Stop before provenance filing or the next run.

## Structural capture gate

A candidate capture is valid for raw preservation only when:

- content is nonempty;
- all ten required response labels appear exactly once;
- zero shell-command signatures are present;
- the first nonempty line is not a shell launcher;
- the final content is not a copied Terminal block;
- the collision-safe destination does not already exist.

The ten required labels are:

1. `FIXTURE_RECOGNIZED:`
2. `HUMAN_AND_CALLNAME:`
3. `COLLABORATION_POSTURE:`
4. `CURRENT_STATE:`
5. `LOCKED_STATE:`
6. `UNCERTAINTY:`
7. `AUTHORITY_BOUNDARY:`
8. `NEXT_ACTION:`
9. `PROVIDER_BOUNDARY:`
10. `ACTION_TAKEN:`

## Failed structural capture

If the structural gate fails:

- do not overwrite or classify the candidate as a valid raw response;
- preserve it under a collision-safe `CAPTURE_REJECTED` filename;
- report the structural measurements;
- stop;
- do not retry without separate authorization.

## Authority boundaries

Each S02 run requires separate explicit authorization.

Authorization for one run permits only:

- one receiver delivery;
- one first response;
- armed clipboard capture;
- structural validation;
- raw-response preservation;
- hashing and governed filing;
- one root-manifest regeneration;
- return payload.

It does not authorize provenance creation, another run, scoring, convergence review, final result, register revision, or lifecycle action unless those actions are separately named.

## Exact stoppoint

This method is prepared and filed only. No S02 run is authorized or performed by possession of this artifact.
