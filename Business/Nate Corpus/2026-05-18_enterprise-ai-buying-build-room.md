---
title: "Enterprise AI: почему роадмапы рушатся в build room"
slug: enterprise-ai-buying-build-room
source: "https://natesnewsletter.substack.com/p/enterprise-ai-buying-build-room"
author: "Nate Jones"
published: 2026-05-10
processed: 2026-05-18
type: video
themes:
  - "[[Implementation Layer]]"
  - "[[Forward Deployed Engineer]]"
  - "[[Frontier Labs]]"
  - "[[Agentic Workflow]]"
  - "[[Audit Trails]]"
  - "[[Moat]]"
frameworks:
  - "[[Implementation Fabric]]"
  - "[[Frontier Alliance]]"
  - "[[Systems of Record]]"
terminology:
  - "[[Forward Deployed Engineer]]"
  - "[[Implementation Layer]]"
  - "[[Audit Trails]]"
  - "[[Agentic Workflow]]"
  - "[[Workflow Completion]]"
---

## TL;DR

За 48 часов в мае 2026 года шесть крупных событий изменили логику закупки корпоративного ИИ. Совокупно ~$5.5 млрд поставлено на то, что ценность создаётся не моделью, а инфраструктурой вокруг неё — доступом к данным, правами, рабочими процессами и аудитом. Модель дешевеет. [[Implementation Layer]] дорожает.

---

## Шесть событий за 48 часов

| # | Событие | Сумма |
|---|---------|-------|
| 1 | Anthropic + Blackstone / Hellman & Friedman / Goldman Sachs — корпоративный AI-сервисный венчур | ~$1.5 млрд |
| 2 | OpenAI — аналогичный венчур с TPG, Brookfield, Advent, Bain | >$4 млрд |
| 3 | SAP покупает Dremio и Prior Labs | — |
| 4 | Pinecone запускает Nexus («compilation-stage knowledge engine») | — |
| 5 | ServiceNow выпускает Action Fabric на Knowledge 2026 (MCP, Anthropic — launch partner) | — |
| 6 | *(McKinsey/Lilli breach — фон, февраль 2026)* | — |

Все эти события — одна ставка: **капитал переходит от покупки модели к покупке сборки** (build).

---

## Главный тезис

> "What is being repriced is not intelligence. Intelligence is cheap and getting cheaper. What is being repriced is the surrounding infrastructure."
> *— Переоценивается не интеллект. Интеллект дёшев и дешевеет. Переоценивается окружающая инфраструктура.*

[[Frontier Labs]] называют это **forward-deployed engineering**. Платформенные вендоры — «governed action» (управляемое действие). Суть одна: [[Implementation Layer]] решает больше, чем строчка модели в бюджете.

---

## Ключевые фреймворки

### 1. Старый vs новый порядок закупки

| Старая последовательность | Новая реальность агентов |
|--------------------------|--------------------------|
| Стратегия → реализация | Реализация определяет стратегию |
| Бюджет на модель | Бюджет на [[Implementation Fabric]] |
| IT как исполнитель | Технические голоса в комнате решений |

Агенты **переворачивают** привычный порядок: ограничения build room теперь определяют, что вообще возможно на стратегическом уровне.

### 2. Контекст, не токены

Pinecone утверждает: **85% вычислений агента тратится на переоткрытие уже известного контекста** (rediscovery). Ограничение по токенам — ложная проблема; настоящая — контекстная архитектура.

> "Why context, not tokens, is the line item ruining agent economics. And why capping usage kills the use case without fixing the cause."
> *— Почему контекст, а не токены — та статья расходов, которая разрушает экономику агентов. И почему ограничение использования убивает сценарий, не устраняя причину.*

### 3. Build room test

Тест на выживаемость вендора: **способен ли его роадмап пережить build room?**

Три изменения, которые делают основную работу (детали за paywall, но структура ясна):
1. Доступ к реальным данным ([[Systems of Record]])
2. Работа в реальных разрешениях (permissions)
3. Встроенные [[Audit Trails]] на уровне платформы

### 4. Инцидент McKinsey / Lilli (февраль 2026)

Автономный агент CodeWall получил полный read-write доступ к внутренней AI-платформе McKinsey (Lilli) **за менее чем 2 часа** через 22 неаутентифицированных API-endpoint. Вектор: SQL-инъекция — класс уязвимостей 1998 года. Платформа обслуживала ~70% из 43 000 консультантов фирмы.

Вывод автора: история не о безопасности — она о закупке. **Платформа вышла без технических голосов в комнате.**

---

## Терминология

| Термин RU | EN | Пояснение |
|-----------|-----|-----------|
| [[Forward Deployed Engineer\|Форвард-инженер]] | Forward-deployed engineering | Инженеры вендора, встроенные в команду клиента для реализации |
| Сборочная комната | Build room | Место, где роадмап встречает реальность реализации |
| Управляемое действие | Governed action | Агентские действия внутри корпоративных границ доступа и аудита |
| Движок компиляции знаний | Compilation-stage knowledge engine | Подход Pinecone Nexus: контекст собирается до запуска агента |
| [[Audit Trails\|Аудитный след]] | Audit trail | Обязательный элемент enterprise-развёртывания агентов |
| [[Agentic Workflow\|Агентный рабочий процесс]] | Agentic workflow | Цепочки автономных шагов агента внутри бизнес-процесса |
| [[Implementation Layer\|Слой реализации]] | Implementation layer | Инфраструктура вокруг модели: данные, права, интеграции, аудит |

---

## Что использовать для нашего портфеля

**Контекст:** AI-интегратор, [[Implementation Layer]] как основной продукт, business objects как единица автоматизации, PE как канал.

1. **Валидация позиционирования.** $5.5 млрд подтверждают: рынок движется туда, где мы уже стоим. [[Implementation Fabric]] — не commodity, а дефицитный ресурс. Это аргумент для PE-фондов при оценке портфельных компаний.

2. **Build room как методология продаж.** Тест «выживет ли ваш роадмап в build room?» — готовый фрейм для квалификации клиентов и аудита их текущих вендоров. Технические голоса в комнате = наша роль на сделке.

3. **Контекстная архитектура вместо токен-экономики.** При проектировании [[Agentic Workflow]] для клиентов акцент на pre-assembly контекста (по модели Pinecone Nexus) даёт измеримый ROI (–85% compute). Это KPI, понятный CFO.

4. **[[Systems of Record]] как точка входа.** Action Fabric (ServiceNow + MCP) означает: enterprise-системы открываются для агентов через стандартный протокол. Наш [[Implementation Layer]] должен уметь подключаться к этому слою, а не обходить его.

5. **Безопасность = закупочный аргумент.** Инцидент McKinsey/Lilli — готовый кейс для разговора с CISO и советом директоров. [[Audit Trails]] и управляемый доступ — не опция, а условие выхода в продакшн.

> TBD: Какие конкретно три изменения в последовательности закупки предлагает автор? (Детали за paywall AI Executive Circle — стоит ли оформить доступ для полного разбора?)

---

## Связанные материалы из того же источника

- *Six things have to be true before AI changes a workflow* (2026-05-14) — deployment layer
- *Your AI agent is rediscovering 85% of its context every run* (2026-05-13) — RAG / knowledge layer
- *You gave your AI agent real tools. Here's the 4-part control layer it's missing* (2026-05-11) — judge layer