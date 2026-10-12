# Тестирование мобильных приложений Android

Портфолио по ручному тестированию Android-приложений.

В репозитории собраны практические QA-артефакты: чек-листы, тест-кейсы, баг-репорты, отчёты о тестировании, описание окружения и технические evidence, полученные с помощью Android-инструментов.

## Проекты

| Проект | Что проверялось | Основной артефакт |
|---|---|---|
| [Тестирование Android-игры](android-game/README.md) | функциональность, gameplay, реклама, настройки, Android lifecycle, UI, базовый анализ Logcat | [Excel QA report](android-game/artifacts/android-game-test-report.xlsx) |
| [Тестирование Skillcinema](skillcinema/README.md) | functional, UI/UX, negative, network и performance testing | [Excel QA report](skillcinema/artifacts/skillcinema-mobile-testing-report.xlsx) |

## Навыки, показанные в проекте

- ручное функциональное и исследовательское тестирование;
- тестирование Android-приложений;
- smoke и regression checks;
- проверка application lifecycle;
- тестирование рекламы и monetization flow;
- создание чек-листов и тест-кейсов;
- оформление баг-репортов с Severity и Priority;
- фиксация Expected / Actual Result;
- Android Studio Emulator;
- ADB;
- Logcat;
- сбор и анализ технических evidence.

## Структура репозитория

```text
mobile-app-testing/
├── android-game/
│   ├── artifacts/
│   │   └── android-game-test-report.xlsx
│   ├── evidence/
│   │   └── README.md
│   └── README.md
├── skillcinema/
│   ├── artifacts/
│   │   └── skillcinema-mobile-testing-report.xlsx
│   ├── evidence/
│   │   └── README.md
│   └── README.md
├── .gitignore
└── README.md
```

## Примечание

Тестируемые приложения являются сторонними продуктами и использовались только в учебных и портфолио-целях.

Репозиторий не содержит APK-файлы, proprietary source code, пользовательские credentials или конфиденциальные данные компаний.

## Автор

**Екатерина Пешкун**
Junior QA Engineer
