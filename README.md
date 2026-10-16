# BEHR STORE — GitHub catalog example

APK-файлы намеренно не включены.

## Быстрый старт
1. Создай публичный репозиторий `borbehr-dev/store` с веткой `main`.
2. Загрузи `index.json` в корень репозитория.
3. HTML-демо уже настроено на `https://raw.githubusercontent.com/borbehr-dev/store/main/index.json`.
4. Открой `index.html` в браузере или размести его на GitHub Pages.

## Добавить APK позже
Положи APK, например, в `apps/my-app/MyApp.apk`, затем заполни поле `apk` в `index.json` значением `apps/my-app/MyApp.apk`. Рекомендуется добавить SHA-256 и публиковать только проверенные APK.

## Поля приложения
`id`, `name`, `version`, `type` (`app` или `game`), `emoji`, `category`, `description`, `apk`, `minAndroid`, `sha256`.

Если `apk` пустой, карточка отображается без кнопки скачивания.

## Ограничения HTML-демо
Демо загружает каталог из GitHub Raw, поддерживает поиск и фильтры, а кнопка обновления перечитывает список версий. Обычный HTML не может надёжно определить установленные Android-приложения и их версии, а также не может установить APK напрямую. Для этого нужна Android-оболочка с нативным кодом и системным установщиком.
