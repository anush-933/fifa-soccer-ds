# Changelog

All notable changes to this project are documented here. The format follows
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Versions follow
[Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- SSRF-checked target validation and output-path containment.
- GNN inference, and a GitHub Pages site built from `docs/`.
- Regression tests for calibration, metrics, ONNX export, GNN training, metadata, safe model loading,
  tactical validation, team classification, YOLO fine-tuning and download limits.
- Tests that stop YouTube result assembly from reporting made-up fields.
- `docs/demo.gif`, this changelog, and a shorter contributing guide.

### Changed

- `pyproject.toml` is now the single source of dependency versions, and the ML stack is pinned
  together.
- Moved to Python 3.12.
- CI pins actions by digest, scopes permissions and installs all extras.
- Readiness reports the real state, and the API requires an explicit checkpoint.
- Kaggle authentication no longer runs at import time.
- Rewrote the README and corrected claims about features, including LoRA fine-tuning.

### Fixed

- Removed false-success paths and hardened artifact handling in `src`.
- Every documented `make` target works from a clean checkout.
- Fixed 19 findings from the October 2026 audit and dropped dead helpers.

### Removed

- Misleading one-off scripts and unused config.

### Security

- Bumped aiohttp, Pillow, cryptography, mlflow, pip and setuptools to clear `pip-audit` advisories.
- Stopped tracking `.env*` files other than `.env.example`.

## [0.1.0] - 2026-04-11

### Added

- First tagged version of the detection, tracking and graph pipeline.
- GitHub Pages deployment workflow.
- CI workflow, community files and repo metadata.

[Unreleased]: https://github.com/jayhemnani9910/fifa-soccer-ds/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/jayhemnani9910/fifa-soccer-ds/releases/tag/v0.1.0
