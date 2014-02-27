# Changelog

All notable changes to CorpusCustody are documented here. The format follows
Keep a Changelog, and the project uses semantic versioning.

## [Unreleased]

### Changed

- Obligation matrix wording is under review for the next patch.

## [1.0.3] - 2026-07-14

### Fixed

- Share-alike obligations propagate through nested manifest references
  instead of stopping at the first level.

## [1.0.2] - 2025-11-04

### Added

- Unknown-license fixture and the unknown handling path in the report.

## [1.0.1] - 2024-06-25

### Fixed

- SPDX identifier matching is case insensitive now, per the specification.

## [1.0.0] - 2023-10-17

### Added

- Stable CLI contract for check, explain, and version, exit codes 0/1/2.
- Tests pin the gate decisions on all three bundled fixtures.

## [0.9.5] - 2022-11-29

### Changed

- Maintenance release: documentation pass and fixture refresh.

## [0.9.0] - 2021-09-07

### Added

- Obligation matrix showing which obligations each license class imposes.
- JSON output for pipeline use.

## [0.8.0] - 2020-12-15

### Added

- Compatibility check between two licenses with a verdict per direction.

## [0.7.0] - 2019-08-20

### Added

- Report renderer with stable finding names.
- CLI entry point with subcommands.

## [0.6.0] - 2018-11-06

### Added

- Test suite covering parsing, the gate, and the CLI.

## [0.5.0] - 2017-07-25

### Added

- First gate rules: permissive passes, share-alike warns, unknown blocks.
- Sample manifests for the three classes.

## [0.4.0] - 2016-10-11

### Added

- Provenance fields in the manifest reader: source, revision, and fetch date.

## [0.3.0] - 2015-06-04

### Added
