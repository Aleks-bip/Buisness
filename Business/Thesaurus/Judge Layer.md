---
title: "Judge Layer"
type: term
source_author: Nate B. Jones
date_processed: 2026-05-18
definition_ru: "Слой-судья / Оценочный слой"
tags: [agent-architecture, evals, production-control]
related_terms: ["Evals", "Audit Trails", "Anticipatory Influence", "Workflow Completion", "Agent Context Bundle"]
---

# Judge Layer

**EN:** Judge Layer
**RU:** Слой-судья / Оценочный слой

## Определение

Выделенный компонент агентной системы, который инспектирует, оценивает или одобряет выходные данные агента до того, как они произведут внешний эффект. Judge Layer работает отдельно от модели, генерирующей ответ, и выступает внутренним фильтром качества, безопасности или соответствия политике. Без него агент действует «вслепую» относительно корректности собственных решений.

## Как используется в корпусе

Термин вынесен в заголовок ключевого материала о контроле агентов в продакшне ([[2026-05-18_agent-judge-layer-production-control]]). Группируется с «Evals», «Audit Trails» и «Workflow Completion» как элемент производственной инфраструктуры, а не опциональная надстройка.

## Источники

- [[2026-05-18_agent-judge-layer-production-control]]
- [[2026-05-18_your-ai-agent-depends-on-six-layers]]
- [[2026-05-18_your-agent-has-12-blind-spots-you]]
- [[2026-05-18_enterprise-ai-deployment-layer]]