# Skillcinema Test Evidence

This directory is intended for sanitized evidence supporting the Skillcinema mobile testing report.

## Evidence types

The project may include:

- screenshots of reproduced defects;
- Android Network Inspector screenshots;
- emulator environment screenshots;
- design comparison images;
- short Logcat excerpts;
- screen recordings demonstrating reproducible behaviour.

## Recommended naming convention

- `SK-BUG-001-onboarding-not-displayed.png`
- `SK-BUG-002-search-request-per-character.png`
- `SK-BUG-003-loader-after-network-error.png`
- `SK-BUG-004-related-movies-missing.png`
- `SK-BUG-005-gallery-categories-missing.png`
- `SK-BUG-006-filter-label-mismatch.png`
- `SK-BUG-007-button-radius-mismatch.png`

## Publication checks

Before evidence is committed, it must be checked for:

- email addresses and passwords;
- authentication tokens;
- API keys;
- device identifiers;
- personal information;
- unrelated applications or browser tabs;
- private URLs;
- confidential company or course data.

## Repository rules

- Third-party APK files are not published.
- Large recordings are stored externally.
- Screenshots should be cropped to the relevant application area.
- Sensitive values must be hidden or replaced with placeholders.
- Each evidence file should reference the related Bug ID.

## Current status

The structured test cases and bug reports are included in the Excel report.

Additional sanitized screenshots may be added after their contents and relevance are verified.
