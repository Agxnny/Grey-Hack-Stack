# R00 — GreyScript API inventory

Initial snapshot: 2026-11-24. `inventory.json` contains 270 entries across 25 groups sourced from [GreyDocs](https://greyscript.net/api). Source blob hashes are recorded in the JSON. This is a community-reference baseline, not a complete or verified inventory of the current game.

## Verification policy

- Test single-player and multiplayer independently, recording exact game build and branch.
- Unknown is not equivalent to available or unrestricted.
- Historical nightly labels must be checked against the current public branch.
- Moderator-only functions are outside normal player tooling.
- Use isolated owned test systems and disposable data; review multiplayer rules before running tests online.
- Record actual return values and types, errors, prerequisites, permission requirements, side effects and resource costs. Do not infer that an emulator reproduces server behavior.
- Preserve source provenance and distinguish documentation from measured observations.

## Known source gaps

Nine entries lack argument or return metadata; three encryption restriction references do not match the function inventory. Sixteen entries match encryption restrictions and fifteen have historical nightly labels. See the JSON discrepancy fields. No entries have been runtime tested.

## Next steps

1. Cross-check against the installed game's manual and current API documentation; reconcile missing groups and signatures.
2. Establish the language/runtime baseline, external development tooling and test environment.
3. Populate library dependencies and permission requirements.
4. Test basic runtime, collections, filesystem, compilation and process APIs first.
5. Establish mode-specific compatibility and document multiplayer limits.
6. Derive verifier and mock interfaces only from the versioned inventory and verified observations.
