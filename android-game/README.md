# Тестирование Android-игры

Независимое black-box тестирование Android-игры **Spider Hero 2 / Spider Fighter 3D**.

Проект демонстрирует ручное тестирование gameplay, рекламы, настроек, магазина, Android lifecycle и отдельных технических событий в Logcat.

## Объект тестирования

| Параметр | Значение |
|---|---|
| Приложение | Spider Hero 2 / Spider Fighter 3D |
| Build | `game: 0.0.1.1686131318` |
| Package | `com.starplay.spider.fighter3d` |
| Activity | `com.superlevel.fighting.GameActivity` |
| Дата тестирования | 2026-06-09 |
| Подход | Ручное black-box тестирование |

## Тестовое окружение

| Параметр | Значение |
|---|---|
| Device | Pixel 4 Android Studio Emulator |
| Android | API 36 |
| Emulator | 36.3.10-14472402 |
| CPU / ABI | x86_64 |
| RAM | 2048 MB |
| Экран | 1080 × 2280, density 440 |
| Host OS | macOS 26.4 |
| Network | Wi-Fi / online |

## Область тестирования

Проверялись:

- установка и запуск приложения;
- версия build;
- pause / resume;
- повторные pause / resume;
- fullscreen-реклама;
- restart после смерти персонажа;
- настройки и управление звуком;
- выбор и сохранение языка;
- настройки качества графики;
- Restore Purchases;
- переход в Shop;
- gameplay и поведение врагов;
- границы карты и физика персонажа;
- Android Back и application lifecycle;
- базовый анализ Logcat.

## Результаты

| Метрика | Результат |
|---|---:|
| Пунктов чек-листа | 19 |
| Passed | 8 |
| Passed with note | 1 |
| Failed | 9 |
| Need retest | 1 |
| Баг-репортов | 10 |
| Open bugs | 9 |
| Need retest bugs | 1 |

## Основные дефекты

### Blocker

- `BUG-ADS-001` — пользователь блокируется на fullscreen-рекламе без доступного способа вернуться в игру.

### High priority

- `BUG-ADS-002` — реклама прерывает restart flow после смерти персонажа;
- `BUG-SHOP-001` — кнопка Shop не открывает магазин;
- `BUG-GAME-002` — вооружённые враги целятся в игрока, но не стреляют;
- `BUG-UI-001` — элемент управления рекламой открывает feedback menu вместо закрытия рекламы.

### Дополнительные находки

- Restore Purchases не даёт видимого результата или обратной связи;
- выбранный язык интерфейса не применяется;
- Low / Medium / High graphics визуально не отличаются;
- информация о build плохо читается;
- персонаж один раз вышел за пределы игровой области и застрял в пустом пространстве.

Проблема с картой/физикой отмечена как **Need retest**, потому что воспроизвелась один раз и требует дополнительных попыток и технических логов.

## Инструменты

- Android Studio Emulator;
- ADB;
- Logcat;
- Android screen recorder;
- screenshots;
- ручной чек-лист;
- структурированные баг-репорты.

## Тестовые артефакты

Полный отчёт:

- [Android game QA report](artifacts/android-game-test-report.xlsx)

В workbook входят:

- сводка проекта;
- 10 баг-репортов;
- 19 пунктов чек-листа;
- реестр technical evidence;
- информация об окружении;
- Severity, Priority и Status legend.

## Evidence

Правила публикации evidence описаны здесь:

- [Описание evidence](evidence/README.md)

Крупные screen recordings хранятся отдельно и не добавляются в Git.

## Ограничения

- Тестирование проводилось на Android Emulator, а не на физическом устройстве.
- Server-side implementation и source code недоступны.
- Часть monetization behaviour зависит от сторонних advertising / billing services.
- APK тестируемого приложения в репозитории не публикуется.
- При отсутствии формальных требований Expected Result определялся по наблюдаемой продуктовой логике и стандартным mobile usability expectations.

## Дисклеймер

Это независимый QA portfolio project.

Тестируемое приложение, игровые материалы, названия и товарные знаки принадлежат соответствующим владельцам. Репозиторий не распространяет приложение или его proprietary source code.
