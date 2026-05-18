---
title: "Business Object"
type: term
source_author: Nate B. Jones
date_processed: 2026-05-18
definition_ru: "Структурированная бизнес-сущность (клиент, контракт, заказ), над которой агент выполняет операции"
tags: [enterprise-ai, data-model, workflow, agents]
related_terms: ["[[Systems of Record]]", "[[Agentic Workflow]]", "[[Implementation Layer]]", "[[Audit Trails]]", "[[Workflow Completion]]"]
---

# Business Object

**EN:** Business Object
**RU:** Бизнес-объект

## Определение

Business Object — конкретная структурированная сущность внутри корпоративных систем: контракт, клиент, заказ, тикет. Агент действует не абстрактно, а всегда в отношении конкретного бизнес-объекта — читает, изменяет или создаёт его. В корпусе бизнес-объект служит единицей измерения «завершённости» агентной задачи: workflow считается выполненным, когда объект обновлён корректно.

## Как используется в корпусе

- В [[2026-05-18_agent-judge-layer-production-control]]: сбои агентов описываются именно через бизнес-объект — «письмо отправлено», «запись изменена» — когда это не было намерением пользователя.
- В [[2026-05-18_trillion-dollar-workflow-retest]]: business object входит в список ключевых framework-терминов для описания полного цикла задачи.

## Источники

- [[2026-05-18_agent-judge-layer-production-control]]
- [[2026-05-18_the-definitive-guide-to-ai-agents]]
- [[2026-05-18_trillion-dollar-workflow-retest]]
- [[2026-05-18_build-buy-hire-wait-ai-matrix]]
- [[2026-05-18_your-agent-has-12-blind-spots-you]]