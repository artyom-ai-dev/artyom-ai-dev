<!--
Design system (red/black cyberpunk):
  palette: #000000 · #141414 · #c41212 · #ff2a2a
  formats:
    banner  1280×400  hero
    about   960×720   4:3 panel
    cards   640×640   1:1 trio
    strip   1280×48   separator (RGBA glow, no solid bg)
    divider 1280×28   SVG red line + soft glow (transparent)
    footer  1280×220  closing
-->

<div align="center">
  <img src="assets/hero-skeleton.png" width="100%" alt="Hero" />
</div>

<br />

<div align="center">

# Артём Тюкин
### Fullstack / Python-инженер · AI в проде

Собираю сервисы, которыми реально пользуются:  
`AI-платформы` · `RAG` · `агенты` · `OCR` · `frontend` · `Docker/CI` · `корпоративные боты`

[![Сайт](https://img.shields.io/badge/%D0%A1%D0%B0%D0%B9%D1%82-ff2a2a?style=for-the-badge&logoColor=black)](https://prod-ai-cases.apps.grok.bot)
[![Telegram](https://img.shields.io/badge/Telegram-000000?style=for-the-badge&logo=telegram&logoColor=ff2a2a)](https://t.me/tryboth)
[![Python](https://img.shields.io/badge/Python-000000?style=for-the-badge&logo=python&logoColor=ff2a2a)](https://github.com/artyom-ai-dev/portfolio)
[![FastAPI](https://img.shields.io/badge/FastAPI-000000?style=for-the-badge&logo=fastapi&logoColor=ff2a2a)](https://github.com/artyom-ai-dev/portfolio)
[![Docker](https://img.shields.io/badge/Docker-000000?style=for-the-badge&logo=docker&logoColor=ff2a2a)](https://github.com/artyom-ai-dev/portfolio)
[![Кейсы](https://img.shields.io/badge/%D0%9A%D0%B5%D0%B9%D1%81%D1%8B-000000?style=for-the-badge&logoColor=ff2a2a)](https://github.com/artyom-ai-dev/portfolio)

<p>
  <a href="https://prod-ai-cases.apps.grok.bot">Сайт</a> ·
  <a href="https://t.me/tryboth">Telegram</a> ·
  <a href="mailto:tyukin69@bk.ru">Почта</a> ·
  <a href="https://github.com/artyom-ai-dev/portfolio">Кейсы на GitHub</a> ·
  гибрид / удалёнка · <b>Открыт к предложениям</b>
</p>

</div>

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/divider.svg?v=6" width="100%" alt="" />

## Начни отсюда

| Открой первым | Зачем |
|------------|-----|
| **[Сайт · prod-ai-cases](https://prod-ai-cases.apps.grok.bot)** | Живая витрина кейсов |
| **[portfolio](https://github.com/artyom-ai-dev/portfolio)** | Публичные кейсы: архитектура, потоки, результат — без приватного кода |
| **[01 · AI-платформа](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md)** | Главный кейс: RAG + агенты + пайплайн встреч |
| **[05 · OCR чертежей](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/05-drawing-ocr.md)** | PDF-скан → ТТ / паспорт / штамп в JSON |
| **[06 · LLM + Excel](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/06-excel-llm-qa.md)** | Проверка тысяч строк актов локальной моделью |

Рабочие репозитории **приватные** (корпоративные данные). Разбор кода — на собеседовании.

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/divider.svg?v=6" width="100%" alt="" />

## Обо мне

<table>
<tr>
<td width="58%" valign="top">

Инженер-программист / инженер-разработчик.

Делаю **продакшен-системы**, а не демо в ноутбуках:  
API → интеграции → Docker → пользователи.

Сильная сторона — стык **инженерии, AI и корпоративных систем**.

Ищу роли: **Fullstack / Python**, **инженер-программист**, **прикладной data scientist**.  
Не трек чистого DevOps и не РП.

</td>
<td width="42%" valign="top">
  <img src="assets/about.png" width="100%" alt="Обо мне" />
</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/divider.svg?v=6" width="100%" alt="" />

## Фокус

<table>
  <tr>
    <td align="center" width="33%">
      <img src="assets/card-ai.png" width="100%" alt="AI" /><br/>
      <b>AI-платформа</b><br/>
      <sub>агенты · RAG · LLM · STT · OCR</sub>
    </td>
    <td align="center" width="33%">
      <img src="assets/card-integrations.png" width="100%" alt="Интеграции" /><br/>
      <b>Интеграции</b><br/>
      <sub>REST · webhooks · Jira · LDAP</sub>
    </td>
    <td align="center" width="33%">
      <img src="assets/card-data.png" width="100%" alt="Данные" /><br/>
      <b>Frontend / DevOps</b><br/>
      <sub>Vue · React · Next · Docker · CI/CD</sub>
    </td>
  </tr>
</table>

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/divider.svg?v=6" width="100%" alt="" />

## Главный кейс

**Корпоративный AI-контур:** база знаний + агенты + встречи + документы.

```mermaid
%%{init: {'theme': 'dark', 'themeVariables': { 'primaryColor': '#2a0000', 'primaryTextColor': '#ffd0d0', 'primaryBorderColor': '#ff2a2a', 'lineColor': '#ff2a2a', 'secondaryColor': '#140000', 'tertiaryColor': '#000000'}}}%%
flowchart LR
  CF[Confluence] --> W[Sync Worker]
  W --> Q[(Qdrant)]
  Q --> AI[AI Assistant]
  MIC[Аудио встреч] --> CA[Clean Audio]
  CA --> AI
  LIR[Пакеты ЛИР] --> AI
  AI --> U[Пользователи / протоколы]
  PDF[Сканы чертежей] --> OCR[OCR service]
  OCR --> ERP[ERP / PLM]
```

Confluence → векторный поиск → агент с tools; встречи: очистка аудио → STT → протокол; чертежи: OCR → JSON.  
Подробнее → [кейс 01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) · [05](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/05-drawing-ocr.md) · все кейсы → [portfolio](https://github.com/artyom-ai-dev/portfolio)

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/divider.svg?v=6" width="100%" alt="" />

## Проекты

### AI-платформа и документы
| | Проект | Что внутри | Кейс |
|:-:|--------|------------|------|
| 01 | **AI Assistant** | Агенты, tool-calling, RAG, протоколы встреч, Ollama/GigaChat, Qdrant | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 02 | **Confluence Sync Worker** | Confluence → чанкинг → TEI/e5 → Qdrant | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 03 | **Clean Audio Service** | DeepFilterNet3 + ffmpeg → вход для STT | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 04 | **Peregovornaya** | Запись встреч на Pi → выгрузка → AI-протокол | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 05 | **lir-package-service** | Распаковка zip/rar пакетов заявок → `agent_task` для агента | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 06 | **drawing-ocr-service** | PDF-скан чертежа → ТТ, паспорт, штамп (JSON API) | [05](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/05-drawing-ocr.md) |
| 07 | **ai-data-agent** | LLM-проверка текстов актов в Excel (тысячи строк, llama.cpp) | [06](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/06-excel-llm-qa.md) |

### Интеграции и автоматизация
| | Проект | Что внутри | Кейс |
|:-:|--------|------------|------|
| 08 | **jira-to-servicedesk / bot-sd-jira** | Jira ↔ Express: чаты, файлы, CSAT, эпики, ВКС, webhooks | [02](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/02-messenger-tracker-sync.md) |
| 09 | **bot_jira** | Notification gateway: SLA-дайджесты → каналы, auth/TLS, gunicorn | [02](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/02-messenger-tracker-sync.md) |
| 10 | **pass_bot** | Self-service сброс пароля AD: FSM, LDAPS, без plaintext в БД | [03](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/03-identity-self-service.md) |
| 11 | **usercreatealertbot** | Alert-релей жизненного цикла учёток 1С/AD → чат | [03](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/03-identity-self-service.md) |
| 12 | **YGO_WEB** | Flask + LDAP + Excel + email | [04](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/04-excel-web-automation.md) |

### Frontend и порталы
| | Проект | Что внутри |
|:-:|--------|------------|
| 13 | **web-ai** | UI AI-ассистента: Vue 3 · Vite · Pinia · Naive UI |
| 14 | **dwh-api-portal** | Next.js · TypeScript · Tailwind · LDAP RBAC · SQL-консоль DWH |
| 15 | **web-dashboard** | React · Vite · dashboard UI + Docker Compose деплой |
| 16 | **utz-ai-feedback-protocol** | Next.js · React · Tailwind — протокол обратной связи |

> Рабочие репозитории **приватные**. Разбор кода — на собеседовании.  
> Публичные описания — в **[portfolio](https://github.com/artyom-ai-dev/portfolio)**.

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/divider.svg?v=6" width="100%" alt="" />

## Стек

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,flask,vue,react,nextjs,ts,vite,tailwind,docker,postgres,mysql,git,linux,gitlab,pytorch&theme=dark" alt="стек" />
</p>

```text
Backend        Python · FastAPI · Flask · gunicorn · REST · SQL
Frontend       TypeScript · Vue 3 · React · Next.js · Vite · Tailwind · Pinia · Naive UI
DevOps         Docker · Compose · GitLab CI/CD · Linux · multi-stage build · server deploy
AI / ML        LLM · RAG · Agents · LangChain · Qdrant · llama.cpp · Tesseract · PyTorch · STT
Интеграции     Webhooks · Jira · eXpress/BotX · LDAP/AD · Confluence
Данные         pandas · openpyxl · Excel-пайплайны · OCR чертежей · PostgreSQL DWH
Боты           FSM · notification gateway · alert relay · TLS/auth
```

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/divider.svg?v=6" width="100%" alt="" />

## Как работаю

- От «есть боль» до **сервиса в проде**
- Границы систем: webhooks, грязные данные, несколько источников истины
- Боты и интеграции — со слоями, auth на ingress и без утечек секретов/PII
- Документирую API и пайплайны так, чтобы их можно было сопровождать
- AI — только если даёт реальную пользу процессу

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/footer-anime.png?v=3" width="100%" alt="footer" />
