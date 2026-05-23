# PDF Skill Approval

## Source

- Repository: https://github.com/anthropics/skills/tree/main/skills/pdf
- Import type: public_import
- Managed package path: skills/pdf
- Review date: 2026-05-23

## What Changed

- Added Skills Charter governance metadata to `SKILL.md`.
- Assigned `@platform` as owner.
- Marked the package `approved` after review.
- Added an evidence pointer back to this review note.
- Preserved the upstream PDF instructions and helper scripts.

## Review Evidence

The package supports common PDF work: reading, extraction, table parsing, merging, splitting, rotation, watermarking, form filling, OCR, generation, and visual verification. The imported package includes helper Python scripts under `skills/pdf/scripts`; these were reviewed as operational helpers for PDF inspection, image conversion, form structure extraction, and form filling.

The main governance decision is that this package is useful enough for team use, but install should be exposed only after provenance, owner, and evidence are present in Git.

## Risk Decision

- Risk level: medium
- Reason: helper scripts are included and should remain reviewed.
- Blockers: none for this test library after owner, provenance, and evidence were added.

## Approval Decision

Approved for the `Guesswhat-Studio/testSkills` approved-only registry.

## Next Steps

1. Generate `skills.json` from the repository.
2. Run strict policy lint.
3. Open a PR for review.
4. Merge after CI passes.
5. Install with `npx skills add Guesswhat-Studio/testSkills --skill pdf -g -a codex`.
