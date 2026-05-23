# Skill Creator Approval

## Source

- Repository: https://github.com/anthropics/skills/tree/main/skills/skill-creator
- Import type: public_import
- Managed package path: skills/skill-creator
- Review date: 2026-05-23

## What Changed

- Moved `skill-creator` from candidate to approved in `SKILL.md`.
- Kept `@platform` as the accountable owner.
- Added an evidence pointer back to this approval note.
- Preserved the upstream instructions, references, agents, assets, eval viewer, and helper scripts.

## Review Evidence

The package helps users create, evaluate, and improve agent skills. The imported package contains supporting agents, reference schemas, HTML review assets, an eval viewer, and Python helper scripts for packaging, validation, evaluation, report generation, benchmark aggregation, and description improvement.

The scripts were reviewed as operational tooling for skill authoring workflows. They remain visible in Git, are included in registry file inventory, and should continue to be reviewed through PR diffs before future changes are merged.

## Risk Decision

- Risk level: medium
- Reason: helper scripts, HTML assets, and external references are included.
- Blockers: none after owner, provenance, evidence, and approval metadata are present.

## Approval Decision

Approved for the `Guesswhat-Studio/testSkills` approved-only registry as an internal skill authoring package.

## Next Steps

1. Generate `skills.json` from the repository.
2. Run strict policy lint.
3. Open a PR for review.
4. Merge after CI passes.
5. Install with `npx skills add Guesswhat-Studio/testSkills --skill skill-creator -g -a codex`.
