---
title: "OpenClaw: от Agent Harness к Agent Runtime — Model Swapping и Durable Workflows"
slug: openclaw-agent-runtime-model-swapping
source: "https://natesnewsletter.substack.com/p/openclaw-agent-runtime-model-swapping"
author: "Nate Jones (@natebjones)"
date_published: 2026-05-07
date_processed: 2026-05-18
type: video
themes:
  - "[[Agentic Workflow]]"
  - "[[Harness]]"
  - "[[Implementation Layer]]"
  - "[[Moat]]"
  - "[[Frontier Labs]]"
frameworks:
  - "[[TaskFlows]]"
  - "[[Open Brain Agent Memory]]"
  - "[[Durable Workflows]]"
terminology:
  - "[[Agent Runtime]]"
  - "[[Model Swapping]]"
  - "[[OpenClaw]]"
  - "[[ClawHub]]"
  - "[[OpenBrain Memory]]"
---

# OpenClaw: от Agent Harness к Agent Runtime

## Краткое содержание

Апрель 2026 — пороговый месяц: [[OpenClaw]] перестал быть [[Harness|обёрткой над моделью]] и стал [[Agent Runtime|исполняющей средой для агентов]]. Одновременно модельный слой стал оспариваемым: Anthropic ограничил сторонний доступ, OpenAI открыл подписки ChatGPT/Codex для пользователей OpenClaw, Google выпустил Gemma 4 для агентной и on-device работы. Центральный тезис: **не модель является продуктом — им является runtime**.

## Ключевые идеи

### 1. Порог апреля 2026
[[TaskFlows]], каналы, память и маршрутизация созрели одновременно — их комбинация пересекла линию [[Agent Runtime|runtime]]. Старое описание ("чат-обёртка над Claude") больше не работает: OpenClaw стал action-слоем, где задачи, инструменты, память, каналы, права, субагенты и выбор модели собираются в [[Durable Workflows|устойчивые воркфлоу]].

### 2. Контекст шага Anthropic
Anthropic вернул subscription-backed третьесторонний доступ в свои продукты — это рациональный шаг монетизации. Разработчики отреагировали негативно. Следствие: Claude переходит в статус **дозированного premium-компонента** вместо дефолтного flat-rate движка.

### 3. Модель больше не мозг — runtime больше не привязан к мозгу
"The model is no longer the product. The runtime is."
*Модель больше не является продуктом. Им является runtime.*

Если «мозг» заменяем — память не может жить внутри ни одного мозга. Архитектурное следствие: [[OpenBrain Memory]] / [[Open Brain Agent Memory]] живёт вне модели и переживает любую её замену.

### 4. Семь воркфлоу, которые теперь реально собрать
| # | Воркфлоу | EN |
|---|---|---|
| 1 | Операции с репозиторием | Repo operations |
| 2 | Память код-ревью | Code review memory |
| 3 | Реагирование на инциденты | Incident response |
| 4 | Обработка обратной связи | Customer feedback |
| 5 | Из встреч — в исполнение | Meetings to execution |
| 6 | Маршрутизация с учётом модели | Model-aware routing |
| 7 | Командная память между агентами | Team memory across agents |

### 5. Запуск Open Brain Agent Memory
Живой скилл на [[ClawHub]], плагин-пакет и четыре рецепта:
- Память код-ревью (Code review memory)
- Рабочие логи [[TaskFlows]] (TaskFlow work logs)
- Рецепт OpenClaw Agent Memory
- Safe Agent Memory Contract — граница между доказательствами и инструкциями

## Терминология

| Термин | EN | Определение |
|---|---|---|
| [[Agent Runtime]] | Agent Runtime | Среда исполнения, объединяющая задачи, инструменты, память, каналы и выбор модели в [[Durable Workflows]] |
| [[TaskFlows]] | TaskFlows | Механизм устойчивых цепочек задач внутри OpenClaw |
| [[Model Swapping]] | Model Swapping | Замена LLM под существующим воркфлоу без перестройки логики |
| [[Durable Workflows]] | Durable Workflows | Воркфлоу, переживающие смену модели, перезапуски и паузы |
| [[OpenBrain Memory]] | OpenBrain / Open Brain Agent Memory | Внешнее хранилище памяти агента, независимое от конкретной модели |
| [[ClawHub]] | ClawHub | Маркетплейс скиллов и плагинов для OpenClaw |
| [[Harness]] | Agent Harness | Устаревшее описание OpenClaw: обёртка-запускатор модели без собственной логики runtime |

## Цитаты

> "The model is no longer the product. The runtime is."
> *Модель больше не является продуктом. Им является runtime.*

> "Build a durable workflow once and swap the model underneath it. That is a much bigger idea."
> *Собери устойчивый воркфлоу один раз и меняй под ним модель. Это значительно более крупная идея.*

> "If the brain is swappable, memory cannot live inside any one brain."
> *Если мозг заменяем, память не может жить внутри ни одного из мозгов.*

## Что использовать для нашего портфеля

**Как AI-интегратор и [[Implementation Layer]]:**
Паттерн «собери [[Durable Workflows|воркфлоу]] один раз — меняй [[Model Swapping|модель]] под ним» напрямую снижает риск вендорной зависимости клиента. Это сильный аргумент при продаже [[Implementation Fabric|implementation fabric]] — клиент не покупает привязку к Anthropic или OpenAI, он покупает устойчивый runtime.

**[[Business Object|Business Objects]] и внешняя память:**
[[OpenBrain Memory|Open Brain Agent Memory]] как архитектурный паттерн = внешнее хранилище [[Business Object|бизнес-объектов]] клиента, персистентное между сменами моделей и агентов. Это конкретная реализация того, что мы описываем как «memory layer» в нашем [[Implementation Layer]].

**[[Forward Deployed Engineer]] как канал:**
Семь рецептов-воркфлоу (код-ревью, инциденты, встречи → исполнение, командная память) — готовые демо-кейсы для [[Forward Deployed Engineer|FDE]]-работы с клиентом. Каждый покрывает реальный болевой сценарий без абстрактных обещаний.

**[[Moat]] и конкурентная картина:**
Борьба [[Frontier Labs|лабораторий]] за «мозг» — Anthropic ограничивает, OpenAI открывается, Google атакует on-device — подтверждает: [[Moat]] строится не в модели, а в слое runtime + memory + workflow. Это наш слой.

**Открытый вопрос:** Как Safe Agent Memory Contract (граница evidence vs instruction) можно формализовать в контрактах с клиентами как часть governance-рамки [[Agentic Workflow]]?