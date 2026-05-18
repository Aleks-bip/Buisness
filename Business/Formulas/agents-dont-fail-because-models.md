---
title: "Агенты дают сбой не из-за моделей"
type: formula
source_author: "Nate B. Jones"
date_processed: "2026-05-18"
quote_en: "Agents don't fail because models are too dumb. They fail because every session starts with no grounded sense of where the work stands."
theme: "память агенты"
tags: []
---

# Провал агента — это провал памяти

> "Agents don't fail because models are too dumb. They fail because every session starts with no grounded sense of where the work stands."

**Перевод:** Агенты дают сбой не из-за того, что модели недостаточно умны. Они дают сбой потому, что каждая сессия начинается без чёткого понимания того, на каком этапе стоит работа.

**Контекст:** Корневая причина отказов — отсутствие персистентного контекста о состоянии задачи, а не недостаток интеллекта модели.

**Применение в нашем портфеле:** Tonttu решает именно эту проблему через `data/memory/` и checkpoint-систему между сессиями.

## Источник

- [[2026-05-18_executive-briefing-the-memory-gap]]