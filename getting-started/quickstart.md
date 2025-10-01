---
icon: bolt
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Quickstart

## Frontend Service (React.js)

### Установка и запуск

```bash
# клонирование репозитория
git clone https://github.com/ваш-аккаунт/hack-dashboard.git
cd hack-dashboard

# установка зависимостей
npm install

# запуск в dev-режиме
npm run dev
```

Приложение будет доступно на [http://localhost:5173](http://localhost:5173).

***

## Backend Service (Golang)

#### Запуск с Docker (рекомендуется)

1. Перейдите в папку проекта:

```bash
cd GoBackend
```

2. Запустите проект:

```bash
docker compose up --build
```

3. API будет доступно по адресу: `http://localhost:8080`

#### Запуск без Docker

1. Установите Go 1.25+
2. Установите зависимости:

```bash
cd GoBackend
go mod download
```

3. Запустите сервер:

```bash
go run cmd/server/main.go
```

***

## Ingest Service (Node.js)

### Установка и запуск

1.  Клонируйте репозиторий:

    ```bash
    git clone https://github.com/Hackaton-Moodify-2025/ingest.git
    cd ingest
    ```
2.  Перейдите в нужный модуль (например, `banki`):

    ```bash
    cd banki
    npm install
    node parser_links.js
    node parser_texts.js
    ```
3. После завершения парсинга данные будут сохранены в `reviews.json`.

***

## Machine Learning Service (Python)

### Сборка и запуск контейнера

`docker compose up -d --build`

### HealthCheck

`curl http://localhost:8000/health`
