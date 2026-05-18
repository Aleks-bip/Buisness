---
title: "Executive Briefing: The Memory Gap Killing Your Enterprise Agent Investments"
slug: executive-briefing-the-memory-gap
source: https://natesnewsletter.substack.com/p/executive-briefing-the-memory-gap
author: Nate Jones
published: 2025-12-07
processed: 2026-05-18
type: video
tags:
  - agent-architecture
  - enterprise-ai
  - memory
themes:
  - "[[Agentic Workflow]]"
  - "[[Implementation Layer]]"
  - "[[Moat]]"
  - "[[Workflow Completion]]"
frameworks:
  - "[[Domain Memory]]"
  - "[[Two-Agent Pattern]]"
  - "[[Agent Workflow Audit]]"
terminology:
  - "[[Domain Memory]]"
  - "[[Memory Gap]]"
  - "[[Two-Agent Pattern]]"
  - "[[Implementation Fabric]]"
  - "[[Harness]]"
---

# The Memory Gap Killing Your Enterprise Agent Investments

## Суть в одном абзаце

Предприятия инвестируют в агентов, но те регулярно проваливаются на задачах длиннее одной сессии. Причина — не слабость модели, а отсутствие памяти: каждая сессия стартует без контекста о состоянии работы. Gartner фиксирует рост запросов по AI-агентам на 750% в 2024 году, однако fantasy of drop-in universal agents is dead — *фантазия об универсальных «plug-and-play» агентах мертва*. Решение — [[Domain Memory]] как инфраструктура, а не как фича.

---

## Терминология

| Термин (RU) | EN | Определение |
|---|---|---|
| [[Memory Gap]] | Memory Gap | Провал между сессиями агента: отсутствие сохранённого состояния цели, прогресса и процедур |
| [[Domain Memory]] | Domain Memory | Структурированная внешняя память агента: цели (goal artifacts), трекинг прогресса, операционные процедуры |
| [[Two-Agent Pattern]] | Two-Agent Pattern | Архитектурный паттерн Anthropic: один агент выполняет работу, второй управляет состоянием и памятью |
| Доменная память как инфраструктура | Domain Memory as Infrastructure | [[Domain Memory]] рассматривается не как опция, а как обязательный инфраструктурный слой — наравне с БД или очередью |
| Тридж вендорских обещаний | Vendor Claim Triage | Методика отсева маркетинговых заявлений о «готовых» агентах по критерию: решена ли проблема памяти |
| Агентный [[Harness]] | Agent Harness | Обёртка над frontier-моделью, которая сама по себе не решает проблему памяти — её нужно решать отдельно |

---

## Ключевые тезисы

### 1. Это проблема памяти, а не интеллекта

> "Agents don't fail because models are too dumb. They fail because every session starts with no grounded sense of where the work stands."
> *Агенты не проваливаются потому, что модели тупые. Они проваливаются потому, что каждая сессия начинается без понимания, где находится работа.*

Anthropic подтвердил это в своей инженерной документации. Расширение контекстного окна до миллиона токенов **ухудшает** ситуацию, а не улучшает — академические исследования показывают деградацию внимания на больших контекстах («lost in the middle»).

### 2. [[Domain Memory]] — три обязательных компонента

| Компонент | Что хранит |
|---|---|
| Goal Artifacts | Явная формулировка цели + критерии завершения |
| Progress Tracking | Что сделано, что в процессе, что заблокировано |
| Operating Procedures | Правила, ограничения, процедуры эскалации |

Без всех трёх агент деградирует в «sophisticated amnesiac» — *изощрённый амнезиак*.

### 3. [[Two-Agent Pattern]] (архитектура Anthropic)

Элегантность паттерна в том, что он **не борется** с амнезиачной природой LLM, а принимает её:
- **Agent A (executor)** — выполняет работу в рамках одной сессии
- **Agent B (memory manager)** — читает и пишет [[Domain Memory]] между сессиями, передаёт контекст следующей сессии

### 4. Стратегический [[Moat]]

> "Your competitive advantage lies in memory design, not model selection."
> *Ваше конкурентное преимущество — в дизайне памяти, а не в выборе модели.*

Все имеют доступ к одним и тем же frontier-моделям. [[Domain Memory]] специфична для домена и не копируется.

### 5. Пять дисциплин серьёзных агентов

TBD — полный контент за paywall. Известно, что разделяют агентов, которые **завершают работу**, от тех, которые **буксуют**.

> Открытый вопрос: какие именно пять дисциплин перечислены в полном тексте?

---

## Пять промптов из материала

| Промпт | Назначение |
|---|---|
| Domain Memory Designer | Универсальный фреймворк для любого [[Agentic Workflow]] |
| Research Workflow Memory | Расследования: бэклог гипотез, лог свидетельств, журнал решений |
| Operations Agent Memory | Инциденты, тикеты, SLA-трекинг, ранбуки |
| Content Production Memory | Редакционные пайплайны, реестры черновиков, источники |
| [[Agent Workflow Audit]] | Диагностика текущих агентных деплойментов — где ломается и почему |

---

## Что использовать для нашего портфеля

**Контекст:** AI-интегратор, [[Implementation Layer]] как продукт, [[Business Object]]-ориентированные агенты, PE как канал продаж.

### Прямое применение

- **[[Domain Memory]] = продаваемый артефакт.** Клиент покупает не агента — он покупает систему, которая не забывает. Это переформулирует ценностное предложение: мы строим не [[Harness]] над моделью, а [[Implementation Fabric]] с памятью.
- **Тридж вендорских обещаний** — готовый инструмент для PE-аудиторий: помогает CIO/CTO отсеивать нереалистичные питчи на закупках. Можно упаковать как discovery-фреймворк.
- **[[Two-Agent Pattern]]** применим к нашим агентным workflows прямо сейчас: выделить memory-агента как отдельный компонент [[Implementation Layer]].

### Для PE-канала

[[Workflow Completion]] как метрика ROI: агент, который завершает многосессионные задачи, напрямую конвертируется в FTE-экономию. Аргумент для LP-обоснования инвестиций в [[Implementation Fabric]].

### Что требует уточнения

TBD — пять дисциплин серьёзных агентов (за paywall). Нужно получить доступ или найти аналогичный источник.

> Открытый вопрос: как именно Anthropic предлагает валидировать [[Domain Memory]] — через [[Evals]] или через отдельный audit-слой?

---

## Связанные материалы в vault

- [[Agentic Workflow]]
- [[Implementation Fabric]]
- [[Workflow Completion]]
- [[Harness]]
- [[Moat]]
- [[Evals]]
- [[Forward Deployed Engineer]] — смежная роль: тот, кто строит [[Domain Memory]] для конкретного клиента