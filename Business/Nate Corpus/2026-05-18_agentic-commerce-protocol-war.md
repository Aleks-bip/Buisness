---
title: "Agentic Commerce Is A Protocol War. Here's Who's Fighting."
slug: agentic-commerce-protocol-war
source: "https://natesnewsletter.substack.com/p/agentic-commerce-protocol-war"
date_published: 2026-05-12
date_processed: 2026-05-18
type: video
author: "Nate (VP Product, Nate's Substack)"
themes:
  - "[[Agentic Workflow]]"
  - "[[Implementation Layer]]"
  - "[[Moat]]"
  - "[[Audit Trails]]"
  - "[[Systems of Record]]"
frameworks:
  - "[[Responsibility Layer Audit]]"
  - "[[Authorization Spec]]"
  - "[[Six Commerce Layers]]"
terminology:
  - "[[Agentic Commerce]]"
  - "[[Protocol War]]"
  - "[[Instant Checkout]]"
  - "[[Authorization Layer]]"
  - "[[Stablecoin Rails]]"
  - "[[Hyperscalers]]"
  - "[[Workflow Completion]]"
---

# Agentic Commerce Is A Protocol War. Here's Who's Fighting.

## Суть в одном абзаце

Традиционная кнопка «купить» скрывала за одним кликом шесть коммерческих ответственностей. Агентная коммерция ([[Agentic Commerce]]) разрывает этот пакет: программный агент сам держит кошелёк, подписывает авторизацию и платит мерчанту. Вопрос смещается с «может ли клиент заплатить?» на «откуда все знают, что агент был уполномочен совершить то, что только что сделал?». За ответ на этот вопрос идёт [[Protocol War]] — Stripe, Shopify, Google и AWS делят слои, которые раньше принадлежали одному клику.

---

## Ключевой тезис

> "The old purchase bundle comes apart, and the market isn't converging on a single replacement. It's splitting into protocol camps, each owning a different piece of what used to live behind one click."
> *Старый пакет покупки распадается, и рынок не сходится к единой замене. Он дробится на протокольные лагеря, каждый из которых владеет своим куском того, что раньше жило за одним кликом.*

---

## Шесть слоёв агентной покупки ([[Six Commerce Layers]])

| # | Слой (RU) | Layer (EN) | Кто борется | Статус |
|---|-----------|------------|-------------|--------|
| 1 | Идентификация агента | Agent Identity | Google, Stripe | Активная разработка |
| 2 | Авторизация | Authorization | Google, Stripe | Два разных подхода |
| 3 | Фрод и риск | Fraud & Risk | Сети, кошельки | TBD — детали за пейволлом |
| 4 | Платёжные учётные данные | Payment Credentials | Stripe, OpenAI | Instant Checkout откатили |
| 5 | Расчёт | Settlement | Stablecoin rails | Отдельный кейс (B2B) |
| 6 | Возвраты, ответственность, права на данные | Refunds, Liability, Data Rights | Shopify, AWS | AWS «тихо важнее всех» |

> **Ключевое разграничение**: Авторизация ≠ Платёж. Слой доказательств ([[Audit Trails]]) должен пережить транзакцию.

---

## Хронология протокольной войны

| Дата | Событие |
|------|---------|
| Сентябрь 2025 | OpenAI + Stripe запускают **Instant Checkout** |
| Февраль 2026 | OpenAI **откатывает** ChatGPT-шопинг, масштаб снижен |
| К маю 2026 | Контр-протокол Shopify + Google набирает позиции |

---

## Кейс стейблкоинов ([[Stablecoin Rails]])

Software-to-software-платежи — это другая бизнес-задача, нежели «человек покупает кроссовки». Аргумент за отдельные рельсы:
- Агент не нуждается в клиентском опыте checkout
- Риск-профиль иной (нет человека-гаранта)
- Расчёт должен быть программируемым и аудируемым

TBD — полная аргументация закрыта пейволлом.

> **Открытый вопрос**: Какой порог объёма/частоты транзакций делает stablecoin-рельсы экономически оправданными по сравнению с card rails?

---

## Терминология

| Термин (RU) | Term (EN) | Определение |
|-------------|-----------|-------------|
| [[Agentic Commerce]] | Agentic Commerce | Коммерция, где агент (ПО) держит кошелёк, подписывает авторизации и платит без прямого участия человека |
| [[Protocol War]] | Protocol War | Конкуренция между платформами за владение отдельными слоями коммерческого доверия в агентном стеке |
| [[Instant Checkout]] | Instant Checkout | Совместный продукт OpenAI + Stripe (сент. 2025), позволявший агенту совершать покупки; свёрнут в феврале 2026 |
| [[Authorization Layer]] | Authorization Layer | Слой доказательств, подтверждающих, что агент был уполномочен совершить действие; должен пережить транзакцию |
| [[Responsibility Layer Audit]] | Responsibility Layer Audit | Фреймворк: явное назначение владельца для каждого из 6 слоёв агентной покупки в продукте |
| [[Authorization Spec]] | Authorization Spec | Спецификация авторизации, приемлемая для финансов и юридического отдела |
| [[Stablecoin Rails]] | Stablecoin Rails | Платёжная инфраструктура на базе стейблкоинов для программируемых B2B-платежей агент→мерчант |
| [[Hyperscalers]] | Hyperscalers | Здесь: AWS — «тихо важнее всех» в агентной коммерческой инфраструктуре |

---

## Что использовать для нашего портфеля

### Как AI-интегратор / [[Implementation Layer]]

**Практический вывод**: большинство продуктов проработали 1–2 слоя из шести. Это наша точка входа — аудит [[Responsibility Layer Audit]] как discovery-инструмент перед каждым агентным внедрением.

**Чеклист для клиентов**:
- [ ] Кто владеет идентификацией агента? Как доказать, что это «наш» агент?
- [ ] Авторизация задокументирована? Может ли она пережить транзакцию для [[Audit Trails]]?
- [ ] Как обрабатываются возвраты, когда агент ошибся? Кто несёт ответственность?
- [ ] Нужны ли stablecoin-рельсы или достаточно card rails?

**Позиционирование**: мы помогаем клиентам назвать и распределить ответственность по всем 6 слоям — до того, как один из агентов отправит деньги не туда. Это и есть [[Implementation Fabric]].

### Business Objects angle

Агентная покупка создаёт новый [[Business Object]] — «авторизованное агентное действие» (authorized agent action) — который должен храниться в [[Systems of Record]] клиента. Это не транзакция. Это доказательство намерения + полномочий + исполнения.

### PE-канал

Портфельным компаниям с e-commerce или B2B-платежами: провести [[Responsibility Layer Audit]] до следующего раунда — это due diligence нового типа. Кто из портфеля уже внедряет агентов с доступом к платёжным инструментам без [[Authorization Layer]]?

---

## Авторы и источники

- **Nate** ([@natebjones](https://twitter.com/natebjones)), VP Product — Nate's Substack
- Смежные материалы в том же издании: Judge Layer (2026-05-11), RAG/Knowledge Layer (2026-05-13), Enterprise AI Deployment Layer (2026-05-14)

---

*Контент за пейволлом — детали по слоям 2–4, два промпта для аудита, кейс AWS. Краткое изложение построено на публичном превью.*