---
title: "Evals"
type: framework
source_author: Nate B. Jones
date_processed: 2026-05-18
description: "Систематическая методология оценки агентов: измерение производительности, выявление слепых зон и верификация качества Harness."
tags: ["ai-agents", "framework", "evaluation", "quality", "benchmarks"]
related_terms: ["Harness", "Moat", "Implementation Fabric", "Forward Deployed Engineer", "Frontier Labs", "Workflow Completion"]
---

# Evals

## Суть

Evals — это не просто тесты, а структурированная система оценки, определяющая, насколько хорошо агент выполняет целевые задачи в реальных условиях. Один и тот же агент на одной и той же модели показывает результат 42% или 78% — разница полностью определяется качеством Harness, и именно Evals это выявляют. Без Evals улучшения агента не верифицируемы.

## Компоненты / Применение

- **Harness Audit** — оценка качества оболочки агента как отдельная процедура
- **Workflow Completion** — метрика успешного завершения end-to-end задач
- 12 слепых зон агента (blind spots) — типовой объект для покрытия Evals
- Применяется при Outcome-Based Pricing — клиент платит за результат, Evals его измеряют
- Встраивается в Implementation Fabric как постоянный компонент, а не разовая проверка
- Связан с Moat: команды с зрелыми Evals итерируют быстрее конкурентов

## Источники

- [[2026-05-18_executive-briefing-the-5-ai-shifts]]
- [[2026-05-18_same-model-78-vs-42-the-harness-made]]
- [[2026-05-18_your-agent-has-12-blind-spots-you]]