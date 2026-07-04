# Release Process

## Current Status

`ca-appsus` is currently an experimental, unreleased public repository.

Do not create a public release, tag, or version milestone until release readiness is explicitly approved.

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

## Release Approval Boundary

This repository follows a local-first workflow.

Do not push, tag, publish a release, or open a release-preparation PR unless Aviad explicitly asks for that step.

## Post-Release Baseline

After an approved release:

- move the relevant `Unreleased` entries into a versioned changelog section
- keep a fresh `## [Unreleased]` section at the top
- re-check the live GitHub Pages deployment

