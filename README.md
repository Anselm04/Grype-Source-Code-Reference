# Grype — TrillionAI Engineering Reference

**Research-only source code archive for TrillionAI Audit. Not a running Grype service or a production TrillionAI Audit integration.**

## Original source and licence

- Official upstream: https://github.com/anchore/grype
- Pinned upstream commit: `6b58d49475713089136ce884a103a867c487bca9`
- Original Git tree: `2c2d2370071bdf9eb857e1aabb9e23adfcc3d6c7`
- Original tracked tree inventory: 2,278 entries, including 1,596 file blobs (7,883,759 bytes).
- Root upstream licence: Apache License 2.0. Preserve `LICENSE`, `COPYRIGHT` and all applicable original notices.
- Source destination: actual original project files **directly on `main`**.
- Verification: **PENDING** until remote Git import and independent source-object comparison have succeeded.

## Why this exists

Grype's publicly available code is useful for studying software-component vulnerability detection, matching installed package versions against advisories, scanning SBOMs (including Syft output), representing findings with provenance, handling database availability and freshness, and building deterministic security decision gates.

This public research repository is NOT a grant to ignore upstream licence obligations. TrillionAI Audit must use independently engineered Node.js/TypeScript orchestration and Flutter UIs, with licensing reviewed before copying individual upstream files. Never put private TrillionAI code into this public source archive.

## Safe source-import contract

The `import-grype-source.yml` GitHub Actions workflow fetches precisely the pinned upstream commit, checks the original Git tree hash, imports its tracked source to the root of `main`, preserves this research document as `TRILLIONAI_REFERENCE.md`, disables imported `.github/workflows/` and verifies all remaining file hashes and the final pushed Git tree.

Original `README.md` and source layout remain as upstream designed. GitHub workflows are deliberately omitted to avoid executing unrelated upstream CI; the destination root Git tree will therefore not have the same SHA as the unmodified upstream tree. Other Git files must match by object SHA and mode.

If GitHub push protection blocks any content, the import must fail rather than bypass safeguards. Exclusions must be explicit and verified before describing the snapshot as complete.

This tracked-source archive is not full Git history, built executables, application test results, vulnerability database downloads, paid integrations or a hosted service.
