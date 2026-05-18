---
title: "Access-Meaning-Authority Framework"
type: framework
source_author: Nate B. Jones
date_processed: 2026-05-18
description: "Трёхмерный фреймворк оценки прав агента: что он может получить (Access), что интерпретировать (Meaning) и что санкционировать (Authority)."
tags: ["ai-agents", "framework", "security", "permissions", "governance"]
related_terms: ["Judge Layer", "Anticipatory Influence", "Vibe Coding", "J-Curve", "Agent Context Bundle", "Cybernetic Development"]
---

# Access-Meaning-Authority Framework

## Суть

Фреймворк декомпозирует агентные права на три независимых измерения, каждое из которых является самостоятельным вектором атаки. Недостаточно ограничить доступ — агент может иметь узкий доступ, но широкую интерпретацию (Meaning) или избыточные полномочия (Authority). Все три измерения должны быть явно определены и ограничены.

## Компоненты / Применение

- **Access** — к каким данным, инструментам и системам агент имеет доступ
- **Meaning** — что агент вправе интерпретировать и как широко он читает контекст
- **Authority** — какие действия агент может санкционировать или инициировать
- Применяется при проектировании Agent Context Bundle
- Связан с J-Curve: расширение прав ускоряет результат, но увеличивает риск
- Основа для threat modeling в контексте prompt injection и data exfiltration

## Источники

- [[2026-05-18_anthropic-and-openai-just-admitted-the-model-isnt-enough]]
- [[2026-05-18_i-broke-down-anthropics-25-billion-leak-your-agent-is-missin]]
- [[2026-05-18_llm-agents-the-security-breach-pattern-nobodys-talking-about]]