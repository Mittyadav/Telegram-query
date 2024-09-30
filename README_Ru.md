# TelegramQueryIDFetcher

![TelegramQueryIDFetcher](https://img.shields.io/badge/Telegram-QueryIDFetcher-blue.svg)
![Лицензия](https://img.shields.io/badge/Лицензия-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.7%2B-yellow.svg)

TelegramQueryIDFetcher - это мощный и простой в использовании инструмент для получения `query_id` от ботов Telegram. Этот проект использует библиотеку Pyrogram для взаимодействия с API Telegram и получает необходимые данные через запросы WebView.

[![Telegram Канал](https://img.shields.io/badge/Telegram-Канал-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedom)
[![Telegram Группа](https://img.shields.io/badge/Telegram-Группа-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedomGroup)

[English](README.md) | [中文](README_CN.md) | [Русский](#русский)

## 🌟 Особенности

- 🚀 **Создание и управление сессиями Telegram**
- 🔍 **Получение `query_id` от указанных ботов Telegram**
- 💾 **Сохранение полученных `query_id` в файлы**
- 🤖 **Поддержка нескольких ботов и нескольких сессий**
- 🌐 **Поддержка прокси для улучшения доступности**

## 📋 Предварительные требования

Прежде чем начать, убедитесь, что у вас есть:

- Python 3.7+

## 📦 Установка

1. Клонируйте репозиторий:

    ```bash
    git clone https://github.com/YourUsername/TelegramQueryIDFetcher.git
    cd TelegramQueryIDFetcher
    ```

2. Установите зависимости:

    ```bash
    pip install -r requirements.txt
    ```

3. Настройте конфигурацию:

    ```bash
    cp .env-example .env
    ```

## ⚙️ Конфигурация

1. Получите `API_ID` и `API_HASH` на [my.telegram.org](https://my.telegram.org)
2. Или ответьте "API" в нашей группе Telegram для получения публичных учетных данных API
3. Отредактируйте файл `.env` и заполните ваши `API_ID` и `API_HASH`

## 🚀 Использование

1. Запустите скрипт:

    ```bash
    python auto_get_token.py
    ```

   Для поддержки прокси:

    ```bash
    python auto_get_token_proxy.py
    ```

2. Выберите соответствующее действие:

    - **Создать сессию**: Введите свой номер телефона и имя сессии
    - **Использовать существующие сессии**: Скопируйте файлы сессий из папки сессий других скриптов в папку сессий этого скрипта
    - **Выберите бота для получения query_id**: Выберите бота и получите query_ids пакетно

3. Автоматическое сохранение query_id:

    - **Все query_ids автоматически сохраняются**: в файлах `botusername_token.txt`

## 🌐 Поддержка прокси

При использовании `auto_get_token_proxy.py` скрипт будет использовать прокси из файла `proxy.txt`. Если количество прокси меньше количества сессий, прокси будут использоваться повторно.
