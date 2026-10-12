# Технические evidence

Папка предназначена для технических доказательств, связанных с отчётом по тестированию Android-игры.

## Типы evidence

В Excel-отчёте используются ссылки на:

- фрагменты Logcat;
- screenshots;
- Android screen recordings;
- package и activity information, полученные через ADB;
- сведения об окружении и build.

## Реестр evidence

| Evidence ID | Тип | Связанные дефекты |
|---|---|---|
| `EVD-001` | Logcat | `BUG-ADS-001`, `BUG-ADS-002` |
| `EVD-002` | Дополнительный Logcat | `BUG-ADS-001`, `BUG-ADS-002` |
| `EVD-003` | Logcat | `BUG-SET-001` |
| `EVD-004` | Screenshots | `BUG-ADS-001`, `BUG-UI-001` |
| `EVD-005` | Screen recording | `BUG-ADS-001`, `BUG-GAME-001` |

## Проверка перед публикацией

Перед добавлением evidence необходимо проверить отсутствие:

- credentials и tokens;
- персональных email;
- device identifiers;
- посторонней персональной информации;
- конфиденциальных данных приложения или компании.

Крупные видео хранятся отдельно, чтобы не увеличивать размер репозитория.

APK не публикуются, так как являются сторонними application binaries.

## Текущий статус

Названия evidence и внешние ссылки указаны в Excel-отчёте.

Небольшие обезличенные screenshots и фрагменты Logcat могут быть добавлены позже после проверки содержимого.
