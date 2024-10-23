﻿# Localhost Shop Docker Compose

## Описание

Этот репозиторий предназначен для запуска приложения "Shop" с помощью Docker Compose в локальной среде разработки. Вы можете работать с проектом без необходимости загружать образы из Docker Hub и можно свободно просматривать код в сабмодулям.

## Структура проекта

Проект состоит из нескольких подмодулей, которые содержат код для веб-API, фронтенда.

## Требования

- Docker
- Docker Compose

## Установка

1. **Клонируйте репозиторий с подмодулями**:

   ```bash
   git clone --recurse-submodules https://github.com/Lom101/localhost-shop-docker-compose.git
   ```

    Если вы уже клонировали репозиторий без подмодулей, вы можете инициализировать и обновить их следующим образом:

    ```bash
    git submodule update --init --recursive
    ```

2. **Создайте файл .env**:

    Скопируйте файл .env.example в .env:
    ```bash
    cp .env.example .env
    ```
    Заполните переменные в .env необходимыми значениями.

## Запуск приложения

Чтобы запустить приложение, выполните следующую команду в корневой директории проекта:

```bash
docker-compose up --build
```

Эта команда соберет необходимые образы и запустит все сервисы.

## Доступ к приложению

- Web API: http://localhost:5000/swagger/index.html
- Фронтенд: http://localhost

## Остановка приложения

Чтобы остановить приложение, нажмите `Ctrl+C` в терминале, где запущен `docker-compose`. Вы также можете выполнить команду:

```bash
docker-compose down
```

## Поддержка

Если у вас возникли вопросы или проблемы, пожалуйста, откройте issue в этом репозитории.
