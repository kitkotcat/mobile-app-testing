# Technical Evidence

This directory is intended for technical evidence supporting the Android game test report.

## Evidence types

The Excel report references the following evidence:

- Logcat excerpts;
- screenshots;
- Android screen recordings;
- package and activity information obtained through ADB;
- environment and build information.

## Evidence register

| Evidence ID | Type | Related defects |
|---|---|---|
| `EVD-001` | Logcat | `BUG-ADS-001`, `BUG-ADS-002` |
| `EVD-002` | Additional Logcat | `BUG-ADS-001`, `BUG-ADS-002` |
| `EVD-003` | Logcat | `BUG-SET-001` |
| `EVD-004` | Screenshots | `BUG-ADS-001`, `BUG-UI-001` |
| `EVD-005` | Screen recording | `BUG-ADS-001`, `BUG-GAME-001` |

## Publication rules

Before evidence is committed, it must be checked for:

- credentials and tokens;
- personal email addresses;
- device identifiers;
- unrelated personal information;
- confidential application or company data.

Large videos are stored externally to avoid unnecessary repository size.

APK files are not published because they are third-party application binaries.

## Current status

Evidence names and external references are included in the Excel report.

Small sanitized screenshots and Logcat excerpts may be added to this directory later.
