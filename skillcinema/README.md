# Тестирование мобильного приложения Skillcinema

Ручное black-box тестирование **Android-приложения Skillcinema**, выполненное как учебный QA-проект.

Проект охватывает функциональное тестирование, UI/UX, негативные сценарии, network behaviour, performance observations и сравнение с требованиями дизайна.

## Объект тестирования

| Параметр | Значение |
|---|---|
| Приложение | Skillcinema |
| Платформа | Android |
| Подход | Ручное black-box тестирование |
| Окружение | Android Studio Emulator |
| Физическое устройство | Не использовалось |
| Версия приложения | Не зафиксирована в исходных артефактах |

## Тестовые окружения

| Окружение | Device | Android | Область проверки |
|---|---|---|---|
| `ENV-01` | Medium Phone Emulator | API 36.1 | UX и проверка дизайна |
| `ENV-02` | Pixel 4 Emulator | API 36 | Functional, UI, network и performance checks |

## Область тестирования

Проверялись:

- запуск приложения и splash screen;
- onboarding;
- Home screen и подборки фильмов;
- карточки фильмов и сериалов;
- Search и filters;
- Favorites и viewing status;
- пользовательские коллекции;
- Profile и история просмотров;
- галерея изображений;
- обработка network errors;
- loading indicators;
- поворот устройства;
- базовые performance observations;
- сравнение UI с design requirements.

## Тестовая документация

| Метрика | Результат |
|---|---:|
| UI / Functional test cases | 63 |
| UX test cases | 12 |
| Всего исходных кейсов | 75 |
| Уникальных объединённых сценариев | 41 |
| Passed | 34 |
| Failed | 6 |
| Needs clarification | 1 |
| Задокументированных дефектов | 7 |

Повторяющиеся исходные сценарии объединены с сохранением первоначальных Test Case ID для трассировки.

## Основные дефекты

### Functional

- onboarding не отображался в одном из зафиксированных прогонов;
- отсутствовал блок Related Movies на странице сериала;
- отображались не все требуемые категории галереи;
- loading indicator оставался видимым после network error.

### Search и performance

- API request отправлялся после каждого введённого символа вместо ожидания паузы во вводе.

### UI

- label фильтра не соответствовал design requirements;
- corner radius кнопки Select отличался от макета.

## Уточнение по onboarding

В исходной документации есть противоречивые результаты:

- часть тест-кейсов фиксирует onboarding как Passed;
- в другом прогоне onboarding не отображался.

Поэтому объединённый сценарий отмечен **Needs clarification**.

Для итогового статуса нужен контролируемый retest на зафиксированной версии приложения.

## Инструменты и техники

- Android Studio Emulator;
- Android Network Inspector;
- ручное functional testing;
- exploratory testing;
- positive / negative testing;
- UI / UX validation;
- сравнение с design mockup;
- тест-кейсы и баг-репорты;
- Severity / Priority assessment;
- трассировка между тест-кейсами и дефектами.

## Тестовый артефакт

Полный отчёт:

- [Skillcinema Mobile Testing Report](artifacts/skillcinema-mobile-testing-report.xlsx)

Workbook содержит:

- сводку проекта;
- объединённые тестовые сценарии;
- 63 исходных UI/Functional case;
- 12 UX case;
- 7 структурированных баг-репортов;
- сведения об окружении;
- ограничения и data-quality notes.

## Evidence

Правила публикации evidence:

- [Описание evidence](evidence/README.md)

## Ограничения

- Тестирование проводилось на Android Emulator, а не на физических устройствах.
- Точная версия приложения и даты отдельных прогонов не зафиксированы в исходных документах.
- Source code и server-side implementation недоступны.
- Формальная API documentation отсутствовала.
- Часть Expected Result основана на требованиях курса и design mockups.
- APK приложения в репозитории не распространяется.

## Дисклеймер

Это независимый учебный QA portfolio project.

Название приложения, design materials и связанные assets принадлежат соответствующим владельцам. Репозиторий не содержит proprietary source code или сторонние application binaries.
