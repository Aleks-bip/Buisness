---
title: "Swiss Cheese Model of Defense"
type: framework
source_author: Nate B. Jones
date_processed: 2026-05-18
description: "Адаптация модели защиты Джеймса Ризона для безопасности LLM-агентов: несколько несовершенных слоёв защиты, взлом происходит при совпадении дыр."
tags: ["ai-agents", "framework", "security", "defense-in-depth"]
related_terms: ["Audit Trails", "Workflow Completion", "Judge Layer", "Access-Meaning-Authority Framework"]
---

# Swiss Cheese Model of Defense

## Суть

Фреймворк переносит классическую модель системной безопасности Ризона на агентные LLM-системы: каждый защитный слой содержит «дыры» (несовершенства), но взлом происходит только тогда, когда дыры всех слоёв выровнены. Один слой защиты — не защита. Надёжная система требует многослойности.

## Компоненты / Применение

- **Слой 1**: ограничения на уровне промпта и системных инструкций
- **Слой 2**: Judge Layer — оценка вывода перед действием
- **Слой 3**: Audit Trails — логирование и обнаружение аномалий постфактум
- **Слой 4**: ограничения на уровне инструментов и прав доступа (Access-Meaning-Authority)
- Применяется при threat modeling агентных пайплайнов
- Объясняет, почему одна защита (например, только system prompt) всегда будет обойдена

## Источники

- [[2026-05-18_anthropic-and-openai-just-admitted-the-model-isnt-enough]]
- [[2026-05-18_i-broke-down-anthropics-25-billion-leak-your-agent-is-missin]]
- [[2026-05-18_llm-agents-the-security-breach-pattern-nobodys-talking-about]]