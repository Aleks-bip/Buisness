---
title: "Agent Context Bundle"
type: term
source_author: Nate B. Jones
date_processed: 2026-05-18
definition_ru: "Контекстный пакет агента"
tags: [agent-architecture, context-management, production-ai]
related_terms: ["Abstraction Tax", "Primitive Fluency", "Judge Layer", "Memory Governance"]
---

# Agent Context Bundle

**EN:** Agent Context Bundle
**RU:** Контекстный пакет агента

## Определение

Полный информационный пакет, передаваемый агенту в момент запуска задачи: системный промпт, память, определения инструментов, инструкции к задаче и релевантная история. Состав и качество контекстного пакета напрямую определяют надёжность и результативность агента. Плохо сформированный bundle — одна из ключевых причин тихих отказов в продакшне.

## Как используется в корпусе

Термин группируется с «Abstraction Tax» и «Primitive Fluency» как технический артефакт, требующий осознанного проектирования. В контексте безопасности агентов рассматривается как вектор атаки — манипуляция контекстным пакетом позволяет влиять на поведение агента без взлома модели.

## Источники

- [[2026-05-18_your-ai-agent-depends-on-six-layers]]
- [[2026-05-18_your-agent-has-12-blind-spots-you]]
- [[2026-05-18_the-complete-guide-to-building-ai]]
- [[2026-05-18_agent-judge-layer-production-control]]