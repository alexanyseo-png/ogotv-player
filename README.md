# OGOTV Player

Публичный репозиторий бинарных релизов OGOTV Player для Windows и Android TV. Исходный код приложения не публикуется.

Готовые файлы доступны на странице [Releases](https://github.com/alexanyseo-png/ogotv-player/releases/latest).

## Android TV

Для Android TV публикуются APK и файл `android-tv.json` в одном GitHub Release. Плеер проверяет этот manifest при запуске, сравнивает `version_code`, загружает APK после согласия пользователя и проверяет SHA-256 перед системной установкой.

APK должен быть подписан тем же ключом, что установленная версия, и иметь больший `versionCode`. Сначала загрузите APK, затем `android-tv.json`; иначе приложение может увидеть обновление до появления самого APK.