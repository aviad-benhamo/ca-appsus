# Changelog

All notable changes to this repository will be documented in this file.

The project is currently Experimental / Not Ready and unreleased. Historical releases have not been reconstructed retroactively.

This repository follows Semantic Versioning for approved releases and Git tags in the format `vMAJOR.MINOR.PATCH`.

Because this repository does not use a package manager, `CHANGELOG.md` is currently the version source of truth.

## [Unreleased]

The `[Unreleased]` section is the active staging area for work that may become part of a future approved release. Move entries into a numbered version section only during explicit release preparation.

### Added

- Repository documentation baseline files.
- Supporting documentation under `docs/` for validation, release preparation, and dependency management.
- `ROADMAP.md` with the current release-readiness and documentation priorities.

### Changed

- Polished release-readiness wording across the README and supporting release documents after the completed final GRS verification pass.
- Reorganized public media assets into dedicated logo, images, and screenshots folders.
- Replaced the repository's personal profile photo asset with a neutral local placeholder for public safety.
- Documented the release and versioning baseline, including SemVer expectations, approval boundaries, and the recommended first release target of `v0.1.0` after baseline completion.
- Rewrote `README.md` to match the GRS structure with current repository identity, demo links, screenshots, development guidance, and AI notice.
- Removed unused duplicate message/event-bus files, cleaned residual mojibake in the active UI, and trimmed debug-only frontend leftovers without changing the static app architecture.
