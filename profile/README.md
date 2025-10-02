# 👋 Moodify Team

Приветствуем вас в GitHub-организации **Moodify**! Мы разрабатываем решения для мониторинга клиентского настроения и выявления проблем с банковскими продуктами в реальном времени, используя современные web-технологии и data science-подходы

## 📄 Документация

- [Команда](https://moodify.gitbook.io/docs)
- [Быстрый старт](https://moodify.gitbook.io/docs/getting-started/quickstart)
- [Frontend Service (React.js)](https://moodify.gitbook.io/docs/services/frontend)
- [Backend Service (Golang)](https://moodify.gitbook.io/docs/services/backend)
- [Ingest Service (Node.js)](https://moodify.gitbook.io/docs/services/ingest)
- [Machine Learning Service (Python)](https://moodify.gitbook.io/docs/services/ml)


## 👨‍💻 Участники команды

- [**Kamenskikh Valeriy**](https://github.com/neon4on) — Software Engineer
- [**Kaledin Danila**](https://github.com/danya1733) — Software Engineer
- [**Matveeva Anna**](https://github.com/moomivee) — Data Science Engineer
- [**Lapova Julia**](https://github.com/JuliaLapova) — Data Science Engineer
- **Gluhikh Anastasia** — Project Manager

---

## 🧠 Проект: Moodify

**Moodify** — это система, отслеживающая динамику пользовательских отзывов о банковских продуктах, анализирующая тональность, выявляющая проблемные зоны и визуализирующая данные в удобной дашборд-форме

Состоит из двух ключевых репозиториев:

---

### 📥 [Ingest Service](https://github.com/Hackaton-Moodify-2025/ingest)

Сервис сбора и парсинга отзывов с популярных сайтов (например, Banki)
Использует многопоточную очередь и автоматизацию браузера для сбора данных

**Технологии:**
- [`axios`](https://github.com/axios/axios) — HTTP-запросы
- [`cheerio`](https://cheerio.js.org/) — парсинг HTML
- [`puppeteer`](https://pptr.dev/) — безголовый браузер Chrome
- [`p-limit`](https://github.com/sindresorhus/p-limit) — управление параллелизмом
- [`selenium-webdriver`](https://www.selenium.dev/documentation/webdriver/) + `chromedriver` — альтернатива Puppeteer

---

### 💻 [Frontend Service](https://github.com/Hackaton-Moodify-2025/frontend)

Веб-интерфейс для отображения аналитики: карта тональностей, графики динамики, API-дашборд, просмотр отзывов.

**Стек:**
- [React 18](https://react.dev/) — основа UI  
- [Vite](https://vitejs.dev/) — быстрый сборщик  
- [Chakra UI](https://chakra-ui.com/) — UI-компоненты  
- [React Router](https://reactrouter.com/) — маршрутизация  
- [Recharts](https://recharts.org/) — диаграммы и графики  
- [React Simple Maps](https://www.react-simple-maps.io/) — геовизуализация  
- [Framer Motion](https://www.framer.com/motion/) — анимации

---

## 📊 Итог

> **Moodify** в рамках хакатона помогает банку быстро понимать, что чувствуют клиенты, и где возникают проблемы, опираясь на реальные отзывы в интернете. Мы объединяем data scraping, анализ тональности и удобную визуализацию данных.

---
