# Android Game Testing

Independent black-box testing of the Android game **Spider Hero 2 / Spider Fighter 3D**.

The project demonstrates manual testing of gameplay, advertisements, settings, shop functionality, Android lifecycle behaviour and selected technical events in Logcat.

## Application under test

| Parameter | Value |
|---|---|
| Application | Spider Hero 2 / Spider Fighter 3D |
| Build | `game: 0.0.1.1686131318` |
| Package | `com.starplay.spider.fighter3d` |
| Activity | `com.superlevel.fighting.GameActivity` |
| Test date | 2026-06-09 |
| Test approach | Manual black-box testing |

## Test environment

| Parameter | Value |
|---|---|
| Device | Pixel 4 Android Studio Emulator |
| Android | API 36 |
| Emulator | 36.3.10-14472402 |
| CPU / ABI | x86_64 |
| RAM | 2048 MB |
| Screen | 1080 × 2280, density 440 |
| Host OS | macOS 26.4 |
| Network | Wi-Fi / online connection |

## Test scope

The testing covered:

- application installation and launch;
- build version verification;
- pause and resume behaviour;
- repeated pause/resume actions;
- fullscreen advertisement flow;
- restart flow after character death;
- settings and sound controls;
- language selection and persistence;
- graphics quality settings;
- Restore Purchases behaviour;
- Shop navigation;
- gameplay and enemy behaviour;
- map boundaries and character physics;
- Android Back and application lifecycle;
- basic Logcat analysis.

## Test results

| Metric | Result |
|---|---:|
| Total checklist items | 19 |
| Passed | 8 |
| Passed with note | 1 |
| Failed | 9 |
| Need retest | 1 |
| Documented bug reports | 10 |
| Open bugs | 9 |
| Need retest bugs | 1 |

## Main findings

### Blocker

- `BUG-ADS-001` — the user is blocked on a fullscreen advertisement without an available way to return to the game.

### High-priority defects

- `BUG-ADS-002` — advertisement interrupts the restart flow after character death;
- `BUG-SHOP-001` — the Shop button does not open the store;
- `BUG-GAME-002` — armed enemies aim at the player but do not shoot;
- `BUG-UI-001` — the advertisement control opens a feedback menu instead of closing the advertisement.

### Additional findings

- Restore Purchases provides no visible result or feedback;
- selected interface language is not applied;
- Low, Medium and High graphics settings show no visible difference;
- build information is difficult to read;
- the character was observed falling outside the playable area and becoming stuck in empty space.

The map/physics issue is marked **Need retest** because it was observed once and requires additional reproduction attempts and technical logs.

## Tools

- Android Studio Emulator;
- ADB;
- Logcat;
- Android screen recorder;
- screenshots;
- manual test checklist;
- structured bug reports.

## Test artifacts

The complete report is available here:

- [Android game QA report](artifacts/android-game-test-report.xlsx)

The workbook contains:

- project summary;
- 10 bug reports;
- 19 checklist items;
- technical evidence register;
- environment information;
- severity, priority and status legend.

## Evidence

Evidence references and publication rules are documented in:

- [Evidence overview](evidence/README.md)

Large screen recordings are stored externally and are not committed directly to this repository.

## Limitations

- Testing was performed on an Android emulator, not on a physical device.
- Server-side implementation and application source code were unavailable.
- Some monetization behaviour may depend on third-party advertising or billing services.
- The project does not include the tested APK.
- Expected behaviour is based on observable product logic and standard mobile usability expectations where formal requirements were unavailable.

## Disclaimer

This is an independent QA portfolio project.

The tested application, game assets, product names and trademarks belong to their respective owners. This repository does not distribute the application or its proprietary source code.
