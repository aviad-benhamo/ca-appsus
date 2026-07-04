# Dependency Policy

## Current Dependency Model

This project does not currently use a package manager, lockfile, or build step.

Frontend libraries are loaded from repository-managed files under `lib/`, and some external assets may be loaded directly from third-party URLs in `index.html`.

## Baseline Rules

- Prefer keeping the current static-app model unless a separate approved issue changes it.
- Do not introduce `npm`, `yarn`, `pnpm`, bundlers, or framework migrations as incidental cleanup.
- Keep dependency changes narrow and reviewable.
- Do not replace vendored library files without documenting what changed and why.

## Updating Existing Dependencies

When updating a dependency that is stored under `lib/`:

1. Confirm the update is necessary.
2. Replace only the specific library files that are in scope.
3. Document the source/version context in the issue or implementation summary.
4. Re-run the manual validation flow in `docs/validation.md`.

## Adding New Dependencies

New dependencies should be added only when they provide clear value that cannot be met by the current static setup.

Every new dependency should have:

- a clear reason for inclusion
- a review of public CDN versus repository-managed files
- a check for licensing compatibility
- a validation pass after integration

## External Asset Caution

If a dependency is loaded from an external URL:

- prefer stable, documented sources
- avoid adding secrets, tokens, or private endpoints
- confirm the app still works if that dependency is blocked or unavailable

