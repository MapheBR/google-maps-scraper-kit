# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- GitHub Actions CI/CD pipeline with automated testing (Python 3.9-3.12)
- Test suite with 81% code coverage (29 tests)
- Comprehensive testing documentation (TESTING.md)
- Architecture decision record for CI/CD (docs/AD-001-test-cicd.md)
- Metrics and baseline documentation (docs/METRICS-001-cicd-baseline.md)
- Test enhancement report (docs/TEST-ENHANCEMENT-REPORT.md)
- Pre-commit hooks for running tests before commits
- Development dependencies (pytest, pytest-cov)
- Testing section in README.md
- CHANGELOG.md for tracking project changes

### Changed
- Updated .gitignore to exclude coverage artifacts
- Updated SECURITY.md with CI/CD security best practices
- Updated requirements-dev.txt to pytest 8.x for Python 3.9 compatibility

### Security
- Pinned all GitHub Actions with absolute SHAs (supply chain security)
- Tightened GITHUB_TOKEN permissions to minimum required
- Documented pinned SHAs policy as mandatory standard in SECURITY.md

### Fixed
- Fixed pytest version to 8.x for Python 3.9 compatibility
- Fixed workflow trigger to include both main and master branches

### CI/CD
- Added pip cache to speed up CI builds
- Added job timeout (10 minutes) to prevent hanging jobs
- Coverage gate enabled (≥80% threshold)
