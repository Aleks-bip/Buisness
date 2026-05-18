---
title: "Systems of Record"
type: term
source_author: Nate B. Jones
date_processed: 2026-05-18
definition_ru: "Авторитетные корпоративные хранилища данных (CRM, ERP), с которыми агенты должны взаимодействовать в производственных процессах"
tags: [enterprise-ai, data, infrastructure, integration]
related_terms: ["[[Agentic Workflow]]", "[[Implementation Layer]]", "[[Business Object]]", "[[Audit Trails]]", "[[Workflow Completion]]"]
---

# Systems of Record

**EN:** Systems of Record
**RU:** Системы учёта / Системы записи

## Определение

Systems of Record — корпоративные системы (CRM, ERP, базы данных), являющиеся единственным источником истины для бизнес-данных. Агент, не имеющий доступа к этим системам, не может завершить реальные бизнес-задачи. В корпусе интеграция с systems of record — критерий зрелости агентного решения.

## Как используется в корпусе

- В [[2026-05-18_agent-judge-layer-production-control]]: systems of record упоминаются в контексте рисков — агент может модифицировать записи без осознанного намерения оператора.
- В [[2026-05-18_trillion-dollar-workflow-retest]]: доступ к systems of record описывается как условие «trillion-dollar workflow» — задачи, которую нельзя автоматизировать без него.

## Источники

- [[2026-05-18_agent-judge-layer-production-control]]
- [[2026-05-18_build-buy-hire-wait-ai-matrix]]
- [[2026-05-18_enterprise-ai-deployment-layer]]
- [[2026-05-18_trillion-dollar-workflow-retest]]
- [[2026-05-18_the-definitive-guide-to-ai-agents]]