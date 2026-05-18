---
title: "Accenture заработала $2.2 млрд на AI-консалтинге: что ваша команда могла бы сделать бесплатно"
slug: youre-about-to-spend-millions-on
source: https://natesnewsletter.substack.com/p/youre-about-to-spend-millions-on
author: "Nate Jones (@natebjones)"
published: 2026-03-24
processed: 2026-05-18
type: video
themes:
  - "[[Agentic Workflow]]"
  - "[[Implementation Layer]]"
  - "[[Moat]]"
  - "[[Frontier Labs]]"
  - "[[Implementation Fabric]]"
frameworks:
  - "[[Build-or-Buy Framework]]"
  - "[[Five Hard Problems]]"
  - "[[Specification Problem]]"
terminology:
  - "[[NemoClaw]]"
  - "[[Token Manufacturer]]"
  - "[[Context Compression]]"
  - "[[Agent Security Stack]]"
  - "[[Forward Deployed Engineer]]"
  - "[[Multi-Agent Coordination]]"
---

# Accenture заработала $2.2 млрд на AI-консалтинге: что ваша команда могла бы сделать бесплатно

## Тезис одной строкой

Из пяти главных проблем production-деплоя AI-агентов четыре — инженерные задачи вашей команды. Только одна требует внешней экспертизы. Индустрия этого не говорит, потому что обе стороны зарабатывают на вашей неопределённости.

---

## Контекст и противостояние

На GTC (март 2026) Jensen Huang выпустил **[[NemoClaw]]** — open-source стек безопасности для агентов — и призвал компании строить агентную инфраструктуру самостоятельно.

За три недели до этого OpenAI подписала multi-year партнёрства с McKinsey, BCG, Accenture и Capgemini для деплоя агентов. Anthropic — аналогичные сделки с Accenture и Deloitte.

> "The limiting factor isn't model intelligence — it's how agents are built and run in organizations."
> *«Ограничивающий фактор — не интеллект модели, а то, как агенты строятся и эксплуатируются в организациях.»*
> — OpenAI (позиционирование в пользу консультантов)

Это **две конкурирующие теории** о сложности деплоя агентов. Выбор между ними определяет: миллионы консультантам или десятки тысяч инженерного времени.

---

## Пять сложных проблем (scorecard)

| # | Проблема (EN) | Проблема (RU) | Кто решает |
|---|---|---|---|
| 1 | Context Compression | [[Context Compression]] | ✅ Инженерная команда |
| 2 | Codebase Instrumentation | Инструментация кодовой базы | ✅ Инженерная команда |
| 3 | Linting as Architecture | Линтинг как архитектура | ✅ Инженерная команда |
| 4 | [[Multi-Agent Coordination]] | Координация мультиагентов | ✅ Инженерная команда |
| 5 | [[Specification Problem]] | Проблема спецификации | ⚠️ Вероятно, нужна внешняя экспертиза |

**Соотношение 4:1** — четыре инженерных задачи, одна требующая доменной экспертизы. Это меняет логику [[Build-or-Buy Framework]] принципиально.

---

## Ключевые концепции

### [[NemoClaw]]
Open-source [[Agent Security Stack]] от Nvidia (анонс GTC, март 2026). Реализует принципы, которые конвергируют с работами Factory.ai по исследованию кодовой базы и работой Alvin Sng по lint-as-architecture. Общий вывод: engineering под агентов имеет 50-летний прецедент — это не беспрецедентная задача.

### [[Specification Problem]]
Единственная из пяти проблем деплоя, где доменная экспертиза действительно нужна. Это не техническая проблема — это проблема точного описания того, что агент должен делать в конкретном бизнес-контексте. [[Forward Deployed Engineer]] от консультанта здесь оправдан.

### [[Token Manufacturer]]
> "Every software company becomes a token manufacturer."
> *«Каждая software-компания становится производителем токенов.»*
> — Jensen Huang

Тезис о том, что SaaS-компании трансформируются в производителей токенов. Клиенты консалтинговых фирм — первые под ударом: они теряют дифференциацию через software и становятся зависимы от тех, кто контролирует [[Implementation Layer]].

### [[Build-or-Buy Framework]]
Три переменные для честной оценки:
1. Уровень доменной специфики задачи
2. Инженерная зрелость команды
3. Наличие аналогов в 50-летней инженерной практике

---

## Терминология

| EN | RU | Wikilink |
|---|---|---|
| NemoClaw | Стек безопасности агентов от Nvidia | [[NemoClaw]] |
| Specification Problem | Проблема спецификации (единственная не-инженерная) | [[Specification Problem]] |
| Context Compression | Сжатие контекста между запусками агента | [[Context Compression]] |
| Multi-Agent Coordination | Координация между агентами | [[Multi-Agent Coordination]] |
| Token Manufacturer | Производитель токенов (новая роль SaaS) | [[Token Manufacturer]] |
| Agent Security Stack | Стек безопасности для агентов | [[Agent Security Stack]] |
| Build-or-Buy | Фреймворк «строить vs. покупать» | [[Build-or-Buy Framework]] |
| Lint-as-Architecture | Линтинг как архитектурный слой | — |

---

## Связи с vault

- [[Implementation Layer]] / [[Implementation Fabric]] — именно за контроль над этим слоем идёт борьба между open-source (NemoClaw) и консультантами
- [[Agentic Workflow]] — пять проблем описывают барьеры production-запуска
- [[Forward Deployed Engineer]] — оправданная роль консультанта только для [[Specification Problem]]
- [[Workflow Completion]] — без решения всех пяти проблем completion невозможен
- [[Audit Trails]] — подразумевается в Agent Security Stack, но не раскрыт в этом материале
- [[Frontier Labs]] — OpenAI и Anthropic играют в обе стороны: модели + консалтинговые партнёрства
- [[Moat]] — SaaS-компании теряют moat, становясь [[Token Manufacturer]]

---

## Что использовать для нашего портфеля

Как AI-интегратор мы находимся точно в центре этого противостояния. Практические выводы:

**1. Позиционирование против «консалтингового захвата»**
Accenture берёт миллионы за то, что наша команда может закрыть как инженерную задачу. Соотношение 4:1 — это наш аргумент в продажах: мы берём инженерные 4/5 по разумной цене и честно говорим, когда нужна доменная экспертиза клиента (1/5).

**2. [[Specification Problem]] как вход через PE-канал**
Private Equity-портфели имеют доменную экспертизу внутри (операционные директора, отраслевые советники). Именно они закрывают [[Specification Problem]]. Наша роль — [[Implementation Fabric]] поверх их спецификации. Это делает PE идеальным каналом: они приносят 1/5, мы закрываем 4/5.

**3. [[NemoClaw]] как технологический рычаг**
Open-source Agent Security Stack снижает стоимость нашей инфраструктуры. Изучить и интегрировать до того, как это сделает Accenture — значит удешевить [[Implementation Layer]] для клиентов и увеличить маржу.

**4. [[Business Object]]-ориентированная спецификация**
Проблема спецификации решается через точное определение [[Business Object]] в процессе клиента. Это наш методологический вклад — не код, а структура знания о том, с чем работает агент.

**5. SaaS-клиенты под угрозой**
Портфельные компании, строящие SaaS-продукты, рискуют стать [[Token Manufacturer]] — commodity-производителями. Надо ставить вопрос о том, где их новый moat в мире агентов.

---

## Открытые вопросы

- Где конкретно проходит граница [[Specification Problem]] в B2B SaaS vs. внутренних операциях? Нужен кейс из нашей практики.
- Как [[NemoClaw]] соотносится с тем, что мы уже строим в [[Harness]]?
- Если каждая SaaS-компания становится [[Token Manufacturer]], какова наша позиция как интегратора — мы тоже в зоне риска?

---

## Источник

Nate's Substack · Paid · ~4 800 слов · Видео + аудио · Опубликовано 2026-03-24