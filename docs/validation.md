# Validation Guide

## Purpose

This repository does not currently use an automated test runner or build pipeline.

Validation is therefore manual and should confirm that the static app still loads correctly in both a local static server and the published GitHub Pages deployment.

## Local Validation

1. Start a local static server from the repository root.
2. Open `index.html` through that server, not as a direct `file://` path.
3. Confirm the home page renders without console-blocking script errors.
4. Confirm the main navigation works for:
   - `#/`
   - `#/about`
   - `#/mail`
5. Confirm the mail area renders its list view.
6. Open at least one mail details route and confirm it loads without breaking the app shell.
7. Check that the shared header remains visible while navigating.
8. Confirm the layout remains usable on both desktop and a narrow mobile-sized viewport.

## GitHub Pages Validation

Production validation should use the canonical Pages URL:

`https://aviad-benhamo.github.io/ca-appsus/`

Confirm:

- the site returns a successful page load
- the home page renders expected assets
- hash-based navigation still works
- the old `/Appsus/` Pages path is not referenced in public documentation

## When to Re-Validate

Run the manual validation flow after:

- routing changes
- asset-path changes
- README or documentation changes that affect public URLs
- dependency updates under `lib/`
- GitHub Pages or repository metadata changes

## Validation Reporting

When completing issue work, document:

- what was changed
- which validation steps were run
- whether GitHub Pages was checked
- any validation steps that were not possible

