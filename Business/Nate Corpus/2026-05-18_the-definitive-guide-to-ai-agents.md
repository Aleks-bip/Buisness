---
title: "The Definitive Guide to AI Agents in 2025"
slug: the-definitive-guide-to-ai-agents
source: https://natesnewsletter.substack.com/p/the-definitive-guide-to-ai-agents
author: Nate Jones (Nate's Substack)
published: 2025-06-17
processed: 2026-05-18
type: video
themes:
  - "[[Agentic Workflow]]"
  - "[[Implementation Layer]]"
  - "[[Moat]]"
  - "[[Workflow Completion]]"
frameworks:
  - "[[Implementation Fabric]]"
  - "[[Systems of Record]]"
  - "[[Forward Deployed Engineer]]"
terminology:
  - "[[Evals]]"
  - "[[Harness]]"
  - "[[Audit Trails]]"
  - "[[Business Object]]"
  - "[[Hyperscalers]]"
  - "[[Frontier Labs]]"
  - "[[Frontier Alliance]]"
---

# The Definitive Guide to AI Agents in 2025

## Суть

Практическое руководство по AI-агентам от VP Product с независимой (не от модельных лабораторий) позицией. Структура — три вложенных уровня: TLDR → Executive Summary → полный разбор. Тон намеренно сухой, справочный — реакция на избыток хайпа.

Центральный тезис:

> "An AI agent is simply an LLM plus tools plus guidance. That's it."
> *AI-агент — это просто LLM плюс инструменты плюс руководство. Всё.*

Большинство провалов происходит не из-за плохих моделей, а из-за неправильных архитектурных решений.

---

## Ключевые тезисы

- Хайп опережает понимание: руководители спрашивают про агентов, не имея даже базового чат-бота.
- Паттерны успеха и провала уже видны — достаточно данных для выводов.
- Окно конкурентного преимущества сужается; ранние внедренцы получат устойчивый [[Moat]].
- Нельзя писать нейтральный гайд, будучи одновременно создателем модели — третья позиция (практик-оператор) имеет ценность.

---

## Архитектурные решения (Architecture Decisions)

| Решение | Варианты | Ключевая метрика |
|---|---|---|
| Топология (Topology) | Single-agent vs Multi-agent | Разница в стоимости 3–10x |
| Память (Memory) | Working / Episodic / Long-term | Риск memory poisoning |
| Купить vs Построить (Buy vs Build) | Zendesk, Salesforce Agentforce, ServiceNow vs custom | TCO + время до запуска |
| Безопасность (Security) | Prompt injection, data exfiltration, HIPAA/GDPR | [[Audit Trails]] |
| Интеграция инструментов (Tool Management) | MCP (Model Context Protocol), rate limiting | Устойчивость к сбоям |
| Наблюдаемость (Observability) | OpenTelemetry GenAI conventions | Production KPIs |

---

## Терминология

| RU | EN | Пояснение |
|---|---|---|
| Агентный воркфлоу | [[Agentic Workflow]] | LLM + инструменты + руководство в связке |
| Отравление памяти | Memory Poisoning | Атака на долгосрочную память агента |
| Протокол контекста модели | MCP — Model Context Protocol | Стандарт подключения инструментов к агенту |
| Слой наблюдаемости | Observability Layer | OpenTelemetry GenAI для prod-мониторинга |
| Слой внедрения | [[Implementation Layer]] | Инфраструктура вокруг модели, без которой она не работает |
| Слой ткани внедрения | [[Implementation Fabric]] | Совокупность процессов, интеграций, данных вокруг агента |
| Системы записи | [[Systems of Record]] | CRM, ERP — источники правды, с которыми работает агент |
| Оценки | [[Evals]] | Бенчмарки и тесты качества агентного поведения |

---

## Кейсы (Case Studies)

**Успех — Wells Fargo**
- 245 миллионов взаимодействий без передачи оператору (human handoff)
- Показывает: при правильной архитектуре агент масштабируется в продакшн

**Провал — MD Anderson / IBM Watson**
- Потери: $62 миллиона
- Диагноз: архитектурные решения, не соответствующие задаче, и несоответствие ожиданий

**Провал — McDonald's drive-thru**
- Вирусные TikTok-видео с ошибками агента
- Диагноз: развёртывание без достаточного контроля качества на высоко-видимом канале

---

## Структура гайда (для навигации)

1. **TLDR** — 1 минута, суть
2. **Executive Summary** — 3 минуты, ключевые рычаги решений
3. **Полный разбор** (~30 страниц):
   - Архитектура: single vs multi-agent
   - Управление памятью и состоянием
   - Buy vs Build: TCO-анализ
   - Безопасность в продакшн
   - Интеграция инструментов и MCP
   - Анализ режимов отказа
   - Мониторинг и наблюдаемость
   - Паттерны реального внедрения

---

## Что использовать для нашего портфеля

**Как AI-интегратор и [[Implementation Layer]]-игрок:**

- Кейс Wells Fargo = аргумент для продажи: 245M взаимодействий без [[Workflow Completion]] через человека — это измеримый ROI. Использовать в питчах.
- Кейсы MD Anderson и McDonald's = аргумент против "купи и запусти": провалы случаются не от плохих моделей, а от отсутствия [[Implementation Fabric]]. Это и есть наша ценность.
- MCP (Model Context Protocol) — следить как стандарт подключения инструментов; важен для унификации [[Harness]] агентов поверх разных [[Systems of Record]] клиентов.
- Buy vs Build фреймворк — применять при первичной диагностике клиента: Salesforce Agentforce / ServiceNow — легитимные альтернативы, но custom даёт контроль и [[Moat]].
- [[Frontier Labs]] (Anthropic, OpenAI) пишут гайды со своей позиции; независимая оценка (как у Nate) = то, что мы можем предложить клиентам как консультанты.
- PE-канал: аргумент "окно конкурентного преимущества сужается" работает как urgency в разговоре с портфельными компаниями фонда.

---

## Открытые вопросы

- Полный контент закрыт за paywall — доступна только превью-часть. Конкретные технические спецификации (бенчмарки single vs multi-agent, детали TCO-модели) недоступны без подписки. Стоит ли купить доступ для детального разбора архитектурных фреймворков?