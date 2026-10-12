# Evidence по тестированию Skillcinema

Папка предназначена для обезличенных доказательств, связанных с отчётом по тестированию мобильного приложения Skillcinema.

## Что можно добавлять

- screenshots воспроизведённых дефектов;
- screenshots Android Network Inspector;
- screenshots тестового окружения Emulator;
- изображения сравнения с дизайном;
- короткие фрагменты Logcat;
- screen recordings с воспроизводимым поведением.

## Рекомендуемые названия файлов

- `SK-BUG-001-onboarding-not-displayed.png`
- `SK-BUG-002-search-request-per-character.png`
- `SK-BUG-003-loader-after-network-error.png`
- `SK-BUG-004-related-movies-missing.png`
- `SK-BUG-005-gallery-categories-missing.png`
- `SK-BUG-006-filter-label-mismatch.png`
- `SK-BUG-007-button-radius-mismatch.png`

## Проверка перед публикацией

Необходимо убедиться, что evidence не содержит:

- email и passwords;
- authentication tokens;
- API keys;
- device identifiers;
- персональные данные;
- посторонние приложения или browser tabs;
- private URLs;
- конфиденциальные материалы компании или курса.

## Правила репозитория

- Сторонние APK не публикуются.
- Крупные recordings хранятся отдельно.
- Screenshots обрезаются до значимой области.
- Sensitive values скрываются или заменяются placeholders.
- Каждый evidence-файл должен ссылаться на соответствующий Bug ID.

## Текущий статус

Структурированные тест-кейсы и баг-репорты находятся в Excel-отчёте.

Дополнительные обезличенные screenshots могут быть добавлены после проверки содержимого и релевантности.
