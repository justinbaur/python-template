# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.1.0] - 2026-04-18

### Added

- GitHub Actions CI workflow
- `lint-ci` tox env for CI-safe linting without auto-fix
- Filled in INSTALL.md with setup and workflow instructions

### Changed

- Bumped pytest `^8.3` → `^9.0`
- Bumped pytest-cov `^6.0` → `^7.0`
- Bumped pytest-mock `^3.14` → `^3.15`
- Bumped mypy `^1.14` → `^1.15`
- Widened ruff constraint `^0.6` → `>=0.6` to allow current releases
- Simplified mypy config to `strict = true`; added `RUF` and `SIM` lint rule sets
- Fixed tox 4 deprecation: replaced `skipsdist = True` with `package = skip` per-env
- Updated README to remove flake8/yapf/isort references, update all doc links to stable URLs, and add ruff reference section
- Regenerated poetry.lock against updated constraints

### Removed

- Orphaned `.flake8` config (flake8 replaced by ruff; config was never called by tox)

## [1.1.0] - 2023-10-06

### Changed

- Dependency updates [@justinbaur](https://github.com/justinbaur).
- Remove unused dependencies [@justinbaur](https://github.com/justinbaur).

## [1.0.0] - 2022-11-09

### Added

- Project template [@justinbaur](https://github.com/justinbaur).
