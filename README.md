<!--
Design system (red/black cyberpunk):
  palette: #000000 · #141414 · #c41212 · #ff2a2a
  formats:
    banner  1280×400  hero
    about   960×720   4:3 panel
    cards   640×640   1:1 trio
    strip   1280×40   separator (transparent PNG)
    divider 1280×24   thin SVG line (no background)
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
`AI-платформы` · `RAG` · `агенты` · `REST/webhooks` · `корпоративные боты`

[![Python](https://img.shields.io/badge/Python-000000?style=for-the-badge&logo=python&logoColor=ff2a2a)](https://github.com/artyom-ai-dev/portfolio)
[![FastAPI](https://img.shields.io/badge/FastAPI-000000?style=for-the-badge&logo=fastapi&logoColor=ff2a2a)](https://github.com/artyom-ai-dev/portfolio)
[![Docker](https://img.shields.io/badge/Docker-000000?style=for-the-badge&logo=docker&logoColor=ff2a2a)](https://github.com/artyom-ai-dev/portfolio)
[![Портфолио](https://img.shields.io/badge/%D0%9F%D0%BE%D1%80%D1%82%D1%84%D0%BE%D0%BB%D0%B8%D0%BE-ff2a2a?style=for-the-badge&logoColor=black)](https://github.com/artyom-ai-dev/portfolio)

<p>
  <a href="mailto:tyukin69@bk.ru">Почта</a> ·
  <a href="https://github.com/artyom-ai-dev/portfolio">Кейсы</a> ·
  гибрид / удалёнка · <b>Открыт к предложениям</b>
</p>

</div>

<img src="assets/divider.svg" width="100%" alt="" />

## Начни отсюда

| Открой первым | Зачем |
|------------|-----|
| **[portfolio](https://github.com/artyom-ai-dev/portfolio)** | Публичные кейсы: архитектура, потоки, результат — без приватного кода |
| **[01 · AI-платформа](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md)** | Главный кейс: RAG + агенты + пайплайн встреч |
| **[02 · Мессенджер ↔ трекер](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/02-messenger-tracker-sync.md)** | Прод: webhooks и двусторонняя синхронизация |

Рабочие репозитории **приватные** (корпоративные данные). Разбор кода — на собеседовании.

<img src="assets/divider.svg" width="100%" alt="" />

## Обо мне

<table>
<tr>
<td width="58%" valign="top">

Инженер-программист / инженер-разработчик в **Уральском турбинном заводе (УЦТ)**.

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

<img src="assets/divider.svg" width="100%" alt="" />

## Фокус

<table>
  <tr>
    <td align="center" width="33%">
      <img src="assets/card-ai.png" width="100%" alt="AI" /><br/>
      <b>AI-платформа</b><br/>
      <sub>агенты · RAG · LLM · STT</sub>
    </td>
    <td align="center" width="33%">
      <img src="assets/card-integrations.png" width="100%" alt="Интеграции" /><br/>
      <b>Интеграции</b><br/>
      <sub>REST · webhooks · Jira · LDAP</sub>
    </td>
    <td align="center" width="33%">
      <img src="assets/card-data.png" width="100%" alt="Данные" /><br/>
      <b>Данные / автоматизация</b><br/>
      <sub>pandas · Excel · matching</sub>
    </td>
  </tr>
</table>

<img src="assets/divider.svg" width="100%" alt="" />

## Главный кейс

**Корпоративный AI-контур:** база знаний + агенты + встречи.

```mermaid
%%{init: {'theme': 'dark', 'themeVariables': { 'primaryColor': '#2a0000', 'primaryTextColor': '#ffd0d0', 'primaryBorderColor': '#ff2a2a', 'lineColor': '#ff2a2a', 'secondaryColor': '#140000', 'tertiaryColor': '#000000'}}}%%
flowchart LR
  CF[Confluence] --> W[Sync Worker]
  W --> Q[(Qdrant)]
  Q --> AI[AI Assistant]
  MIC[Аудио встреч] --> CA[Clean Audio]
  CA --> AI
  AI --> U[Пользователи / протоколы]
```

Confluence → векторный поиск → агент с tools; встречи: очистка аудио → STT → протокол.  
Подробнее → [кейс 01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) · все кейсы → [portfolio](https://github.com/artyom-ai-dev/portfolio)

<img src="assets/divider.svg" width="100%" alt="" />

## Проекты

### AI-платформа
| | Проект | Что внутри | Кейс |
|:-:|--------|------------|------|
| 01 | **AI Assistant** | Агенты, tool-calling, RAG, протоколы встреч, Ollama/GigaChat, Qdrant | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 02 | **Confluence Sync Worker** | Confluence → чанкинг → TEI/e5 → Qdrant | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 03 | **Clean Audio Service** | DeepFilterNet3 + ffmpeg → вход для STT | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |
| 04 | **Peregovornaya** | Запись встреч на Pi → выгрузка → AI-протокол | [01](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/01-ai-platform.md) |

### Интеграции и автоматизация
| | Проект | Что внутри | Кейс |
|:-:|--------|------------|------|
| 05 | **jira-to-servicedesk** | Jira ↔ Express: чаты, файлы, CSAT, webhooks | [02](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/02-messenger-tracker-sync.md) |
| 06 | **bot_jira** | Дайджесты SLA Jira/ServiceDesk в каналы | [02](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/02-messenger-tracker-sync.md) |
| 07 | **pass_bot** | Сброс пароля AD из мессенджера (LDAPS) | [03](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/03-identity-self-service.md) |
| 08 | **usercreatealertbot** | Алерты по жизненному циклу учёток | [03](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/03-identity-self-service.md) |
| 09 | **YGO_WEB** | Flask + LDAP + Excel + email | [04](https://github.com/artyom-ai-dev/portfolio/blob/main/cases/04-excel-web-automation.md) |

> Рабочие репозитории **приватные**. Разбор кода — на собеседовании.  
> Публичные описания — в **[portfolio](https://github.com/artyom-ai-dev/portfolio)**.

---

## Стек

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,flask,docker,postgres,mysql,git,linux,js,pytorch&theme=dark" alt="стек" />
</p>

```text
Backend        Python · FastAPI · Flask · Docker · REST · SQL
AI / ML        LLM · RAG · Agents · LangChain · Qdrant · PyTorch · STT
Интеграции     Webhooks · Jira · eXpress · LDAP/AD · Confluence
Данные         pandas · openpyxl · Excel-пайплайны
```

## Как работаю

- От «есть боль» до **сервиса в проде**
- Границы систем: webhooks, грязные данные, несколько источников истины
- Документирую API и пайплайны так, чтобы их можно было сопровождать
- AI — только если даёт реальную пользу процессу

<img src="https://raw.githubusercontent.com/artyom-ai-dev/artyom-ai-dev/main/assets/footer-anime.png?v=3" width="100%" alt="footer" />
