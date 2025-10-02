---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# 👋 Moodify Team

Приветствуем вас в [GitHub-организации **Moodify**](https://github.com/Hackaton-Moodify-2025)! Мы разрабатываем решения для мониторинга клиентского настроения и выявления проблем с банковскими продуктами в режиме реального времени, используя современные web-технологии и data science-подходы.

### 👨‍💻 Участники команды

* [**Kamenskikh Valeriy**](https://github.com/neon4on) — Software Engineer
* [**Kaledin Danila**](https://github.com/danya1733) — Software Engineer
* [**Matveeva Anna**](https://github.com/moomivee) — Data Science Engineer
* [**Lapova Julia**](https://github.com/JuliaLapova) — Data Science Engineer
* **Gluhikh Anastasia** — Project Manager

***

### 🧠 Проект: Moodify

**Moodify** — это система, отслеживающая динамику пользовательских отзывов о банковских продуктах, анализирующая тональность, выявляющая проблемные зоны и визуализирующая данные в удобной дашборд-форме

Состоит из четырёх ключевых репозиториев:

***

#### 📥 [Ingest Service](https://github.com/Hackaton-Moodify-2025/ingest)

Сервис сбора и парсинга отзывов с популярных сайтов (например, Banki) Использует многопоточную очередь и автоматизацию браузера для сбора данных

**Технологии:**

* [`axios`](https://github.com/axios/axios) — HTTP-запросы
* [`cheerio`](https://cheerio.js.org/) — парсинг HTML
* [`puppeteer`](https://pptr.dev/) — безголовый браузер Chrome
* [`p-limit`](https://github.com/sindresorhus/p-limit) — управление параллелизмом
* [`selenium-webdriver`](https://www.selenium.dev/documentation/webdriver/) + `chromedriver` — альтернатива Puppeteer

***

#### 💻 [Frontend Service](https://github.com/Hackaton-Moodify-2025/frontend)

Веб-интерфейс для отображения аналитики: карта тональностей, графики динамики, API-дашборд, просмотр отзывов.

**Стек:**

* [React 18](https://react.dev/) — основа UI
* [Vite](https://vitejs.dev/) — быстрый сборщик
* [Chakra UI](https://chakra-ui.com/) — UI-компоненты
* [React Router](https://reactrouter.com/) — маршрутизация
* [Recharts](https://recharts.org/) — диаграммы и графики
* [React Simple Maps](https://www.react-simple-maps.io/) — геовизуализация
* [Framer Motion](https://www.framer.com/motion/) — анимации

***

#### 🎁 [Backend Service](https://github.com/Hackaton-Moodify-2025/backend)

Backend — это центральный API-шлюз для взаимодействия фронтенда и ML-сервисов

**Стек:**

* Go 1.25 — язык разработки
* Fiber v3 — веб-фреймворк (быстрая альтернатива Gin/Chi)
* Zap — логирование
* YAML v3 — конфиги
* Docker & Docker Compose — контейнеризация и локальный запуск

***

#### 🎓 [Machine Learning Service](https://github.com/Hackaton-Moodify-2025/ml)

Модуль машинного обучения для анализа клиентских отзывов:

* Кластеризация текстов (выделение тем: кредитные карты, вклады, мобильное приложение и т.д.).
* Мультилейбл классификация по темам.
* Определение тональности (положительно / нейтрально / отрицательно).

**ML/NLP стек:**

* NumPy, Pandas, SciPy — обработка данных
* scikit-learn — классические ML-алгоритмы
* PyTorch — обучение и инференс моделей
* BERTopic + HDBSCAN — тематическое моделирование
* NLTK, pymorphy2 — NLP-утилиты для русского языка

**Сервисный стек:**

* FastAPI + Uvicorn — REST API
* Pydantic — валидация и схемы данных
* MLflow — управление экспериментами и моделями

