---
title: "Conversion Stack"
type: framework
source_author: Nate B. Jones
date_processed: 2026-05-18
description: "Слоистая архитектура преобразования вывода модели в надёжные агентные действия через последовательные фильтры и судьи."
tags: ["ai-agents", "framework", "orchestration", "output-quality"]
related_terms: ["Judge Layer", "Anticipatory Influence", "Primitive Fluency", "Harness"]
---

# Conversion Stack

## Суть

Conversion Stack описывает цепочку слоёв, через которые проходит вывод языковой модели прежде, чем превратиться в реальное действие агента. Каждый слой фильтрует, оценивает или трансформирует ответ. Без этого стека raw output модели напрямую управляет агентом — главный источник непредсказуемости.

## Компоненты / Применение

- **Judge Layer** — оценивает качество и безопасность вывода перед исполнением
- **Anticipatory Influence** — слой, предсказывающий последствия действия до его выполнения
- **Primitive Fluency** — базовый уровень, обеспечивающий правильную интерпретацию примитивов
- Используется при проектировании harness'а агента
- Критичен для Workflow Completion — завершение задачи без деградации качества
- Отсутствие стека = прямой путь к security breach и галлюцинациям

## Источники

- [[2026-05-18_anthropic-and-openai-just-admitted-the-model-isnt-enough]]
- [[2026-05-18_i-broke-down-anthropics-25-billion-leak-your-agent-is-missin]]
- [[2026-05-18_llm-agents-the-security-breach-pattern-nobodys-talking-about]]