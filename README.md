# ISCRA Task Tracking Bot

Проект чат-бота для управления СУП Redmine.

### Текущий список целей:
 - [X] Поддержка управления СУП Redmine
 - [X] Поддержка мессенджера Telegram

### Зависимости не из стандартной библиотеки Python 3
* `redminebotlib` - библиотека обеспечивающая исполнение сценария
* `origamibot` - библиотека для связи с Telegram API

### Установка и запуск

1. Склонируйте репозиторий
2. Исправьте конфигурацию. На данный момент она находится в переменной `config`.
Параметры указанные ниже отвечают за соединение с сервером.
```json
    "use_https"             : false, // При false будет использован простой http
    "redmine_root_url"      : "localhost/redmine",
    "bot_user_key"          : "8e7a355d7f58e4b209b91d9d1f76f2a85ec4b0b6", // ключ API Redmine
```
3. Установите библиотеки:
```sh
python3 -m venv tg_rdbot
source ./tg_rdbot/bin/activate
python3 -m pip install --upgrade redminebotlib origamibot
```
4. Запустите bot.py
```sh
python3 bot.py [ключ бота в Telegram]
```
----

```
Copyright 2023 Fe-Ti aka T.Kravchenko, ISCRA
```
