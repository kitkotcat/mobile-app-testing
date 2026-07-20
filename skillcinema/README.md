# Skillcinema Mobile Application Testing

Manual black-box testing of the **Skillcinema Android application**, performed as an educational QA project.

The project covers functional testing, UI/UX validation, negative scenarios, network behaviour, performance observations and comparison with design requirements.

## Application under test

| Parameter | Value |
|---|---|
| Application | Skillcinema |
| Platform | Android |
| Test approach | Manual black-box testing |
| Test environments | Android Studio Emulator |
| Physical device | Not used |
| Application version | Not recorded in the source artifacts |

## Test environments

| Environment | Device | Android version | Scope |
|---|---|---|---|
| `ENV-01` | Medium Phone Emulator | API 36.1 | UX and design validation |
| `ENV-02` | Pixel 4 Emulator | API 36 | Functional, UI, network and performance checks |

## Test scope

The testing covered:

- application launch and splash screen;
- onboarding;
- Home screen and movie collections;
- movie and series details;
- Search and filters;
- Favorites and viewing status;
- custom user collections;
- Profile and viewing history;
- image gallery;
- network error handling;
- loading indicators;
- device rotation;
- basic performance observations;
- UI comparison with design requirements.

## Test documentation

| Metric | Result |
|---|---:|
| UI / Functional test cases | 63 |
| UX test cases | 12 |
| Total source cases | 75 |
| Consolidated unique scenarios | 41 |
| Passed consolidated scenarios | 34 |
| Failed consolidated scenarios | 6 |
| Needs clarification | 1 |
| Documented defects | 7 |

Repeated source scenarios were consolidated while preserving their original test-case IDs for traceability.

## Main findings

### Functional defects

- the onboarding screen was not displayed during one documented execution;
- the Related Movies block was missing on a series page;
- not all required image gallery categories were displayed;
- the loading indicator remained visible after a network error.

### Search and performance

- an API request was sent after every entered character instead of waiting for a pause in user input.

### UI defects

- the filter label did not match the design requirements;
- the Select button corner radius differed from the design mockup.

## Onboarding result clarification

The source documents contain conflicting onboarding results:

- some test cases record the onboarding flow as passed;
- another execution records that onboarding was not displayed.

The consolidated scenario is therefore marked **Needs clarification**.

A controlled retest on a documented application build is required before assigning a final result.

## Tools and techniques

- Android Studio Emulator;
- Android Network Inspector;
- manual functional testing;
- exploratory testing;
- positive and negative testing;
- UI and UX validation;
- design comparison;
- test-case and bug-report preparation;
- severity and priority assessment;
- traceability between test cases and defects.

## Test artifact

The complete consolidated report is available here:

- [Skillcinema Mobile Testing Report](artifacts/skillcinema-mobile-testing-report.xlsx)

The workbook contains:

- project summary;
- consolidated test scenarios;
- 63 original UI/Functional cases;
- 12 original UX cases;
- 7 structured bug reports;
- test environment information;
- limitations and data-quality notes.

## Evidence

Evidence handling and publication rules are described here:

- [Evidence overview](evidence/README.md)

## Limitations

- Testing was performed on Android emulators rather than physical devices.
- The exact application version and execution dates were not recorded in the source documents.
- Application source code and server-side implementation were unavailable.
- Formal API documentation was unavailable.
- Some expected results were based on course requirements and design mockups.
- The tested APK is not distributed in this repository.

## Disclaimer

This is an independent educational QA portfolio project.

The application name, design materials and related assets belong to their respective owners. The repository does not contain proprietary source code or third-party application binaries.
