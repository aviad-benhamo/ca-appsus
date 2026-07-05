# Release Process

## Current Status

`ca-appsus` is currently Experimental / Not Ready.

Do not create a public release, Git tag, GitHub Release, or version milestone until release readiness is explicitly approved.

## Versioning Baseline

- Release version format: `vMAJOR.MINOR.PATCH`
- Versioning model: Semantic Versioning
- Current version source of truth: `CHANGELOG.md`
- Package-manager version file: none currently, because this repository does not use a package manager

Use `0.x.x` versions until the repository is intentionally declared stable.

The recommended first release target remains `v0.1.0`, and it should be considered only after the completed final GRS verification, current documentation alignment, and explicit release approval.

## Baseline Release Preparation

Before any first public release is considered, confirm:

- `LICENSE` exists
- `SECURITY.md` exists
- `CHANGELOG.md` exists and is current
- README links and repository references are current
- GitHub Pages uses `https://aviad-benhamo.github.io/ca-appsus/`
- the manual validation flow in `docs/validation.md` has been completed
- the repository has passed a final GRS-aligned review

## Change Documentation

Before release preparation:

1. Record user-facing and repository-level changes under `## [Unreleased]` in `CHANGELOG.md`.
2. Do not invent historical versions that were never published.
3. Keep release notes grounded in completed issue work.
4. Move `[Unreleased]` entries into a numbered version section only during approved release preparation.

## Release Approval Boundary

This repository follows a local-first workflow.

Do not push, create tags, publish a GitHub Release, or open a release-preparation PR unless Aviad explicitly asks for that step.

## Post-Release Baseline

After an approved release:

- move the relevant `Unreleased` entries into a versioned changelog section
- keep a fresh `## [Unreleased]` section at the top
- re-check the live GitHub Pages deployment
