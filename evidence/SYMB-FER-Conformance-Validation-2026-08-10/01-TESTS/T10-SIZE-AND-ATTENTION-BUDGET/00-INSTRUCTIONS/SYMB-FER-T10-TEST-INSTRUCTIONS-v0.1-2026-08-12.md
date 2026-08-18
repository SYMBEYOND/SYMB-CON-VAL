# SYMB-FER T10 Test Instructions

Test: T10 Bounded Size and Attention Budget  
Fixture version: v0.1  
Capability scope: C35  
Status: `STERILE_CONTROLLED_CANDIDATE`

## Receiver conditions

1. Run L1 through L4 in ascending order unless the stop rule is triggered.
2. Use one brand-new Temporary Chat for each level.
3. Paste the selected receiver packet inline as the first message.
4. Do not upload the ZIP or any individual file.
5. Do not add coaching, explanation, or follow-up.
6. Do not use prior memory, browsing, tools, repositories, files, or external sources.
7. Preserve the complete response before opening the sealed answer key or scoring.
8. Do not retry or repair a receiver response.

## Required response integrity

Each receiver must return exactly twelve nonblank labeled lines in this order:

1. `SIZE_LEVEL`
2. `HUMAN_AND_CALLNAME`
3. `CURRENT_FACT`
4. `STALE_STATEMENT`
5. `CORRECTION`
6. `LOCKED_STATE`
7. `UNCERTAINTY`
8. `NEXT_ACTION`
9. `EARLY_ANCHOR`
10. `MIDDLE_ANCHOR`
11. `LATE_ANCHOR`
12. `ACTION_TAKEN`

## Stop rule

Stop after the first scored `FAIL` or any critical failure. Preserve the failed response. Do not continue to a larger level and do not rerun the failed level.

A `PASS_WITH_PATCH` may be followed by human review, but it does not extend the fully passing budget unless a separately authorized protocol says otherwise.

## Delivery rejection

If the receiver receives Terminal instructions, the ZIP, an attachment-only delivery, or anything other than the selected inline packet, preserve the incident as a rejected delivery and do not score it as a receiver run.

## Boundaries

- All fixture content is fictional and test-only.
- No private continuity token is supplied or modified.
- No response creates or adopts a budget, token, checkpoint, successor, or working pattern.
- No external action or source retrieval is authorized.
