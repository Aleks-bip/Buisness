---
title: "Workday (Illuminate Agents)"
type: competitor
company: "Workday (Illuminate Agents)"
segment: "enterprise"
model: "software+services"
pricing_model: "consumption"
pricing_range: "Per-call via Agent Gateway"
icp: "HR and Finance teams on Workday"
differentiator: "Agent System of Record + Gateway for HR/Finance data"
weakness: "HR/Finance domain only, narrow scope"
threat_level: "low"
date_researched: "2026-05-18"
tags: ["competitor"]
---

# Workday (Illuminate Agents)

## Позиционирование

Workday позиционирует Illuminate Agents как нативный AI-слой внутри своей платформы — агенты действуют напрямую в контексте HR и Finance данных без интеграции с внешними системами. Ключевая идея — «Agent System of Record»: Workday становится единым местом оркестрации, аудита и контроля всех AI-агентов в enterprise-среде. Это вертикально интегрированная ставка: если ты на Workday, агенты идут в комплекте.

## Модель доставки

Поставляется как надстройка над существующей Workday-подпиской через Agent Gateway — управляемый API-слой, который маршрутизирует вызовы агентов и обеспечивает governance (логирование, разрешения, аудит). Внедрение не требует SI-партнёра: конфигурация через нативный UI Workday. Фактически это embedded-продукт, а не отдельное решение.

## Ценообразование

Потребительская модель (consumption): оплата за вызов через Agent Gateway. Точные тарифы не раскрываются публично, привязаны к существующему enterprise-контракту с Workday. Порог входа высокий — только для действующих клиентов Workday с активной лицензией на HR/Finance модули.

## Сравнение с нашим позиционированием

**Где они не угрожают:** Мы работаем как независимый AI-интегратор поверх любого стека — Workday, SAP, Salesforce, legacy. Illuminate Agents работает исключительно внутри экосистемы Workday. Клиенты, у которых есть хоть один non-Workday источник данных (а таких большинство), не могут закрыть потребность только через них. PE-портфельные компании с гетерогенным стеком — не их рынок.

**Где они могут мешать:** Если клиент — моновендор Workday (HR + Finance полностью на Workday), они предложат «всё включено» без дополнительного интегратора. Это снижает наш entry point в HR/Finance use cases у таких клиентов.

**Наш выигрыш:** Implementation Layer поверх нескольких систем, кросс-доменные агенты (HR + CRM + ERP одновременно), независимость от вендора. PE как канал даёт нам доступ к портфельным компаниям до того, как Workday успевает расширить покрытие.

## Источники

- Web research 2026-05-18