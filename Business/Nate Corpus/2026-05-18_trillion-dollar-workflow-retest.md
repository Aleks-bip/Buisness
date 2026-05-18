---
title: Трillion-Dollar Agentic Workflow Opportunity
slug: trillion-dollar-workflow-retest
type: video
source: https://youtu.be/jwtpMSRAPAQ
published: unknown
processed: 2026-05-18
themes:
  - "[[Agentic Workflow]]"
  - "[[Implementation Layer]]"
  - "[[Frontier Labs]]"
  - "[[Systems of Record]]"
  - "[[Harness]]"
  - "[[Hyperscalers]]"
frameworks:
  - "[[Four Axes of Pressure]]"
  - "[[Object-Oriented AI Model]]"
terminology:
  - "[[Forward Deployed Engineer]]"
  - "[[Evals]]"
  - "[[Business Object]]"
  - "[[Audit Trails]]"
  - "[[Implementation Fabric]]"
  - "[[Workflow Completion]]"
  - "[[Moat]]"
  - "[[Frontier Alliance]]"
---

## Тезисы

- **Крах однородности SaaS.** Финансовая формула «все SaaS-компании на вкус как курица» (SaaS tastes like chicken) перестала работать: рост и прибыльность SaaS стагнируют, PE-фонды застряли с активами, купленными под старую модель.
- **Триллионная возможность [[Agentic Workflow]].** Весной 2026 года впервые стало возможным надёжно, масштабируемо и повторяемо доводить целые бизнес-воркфлоу до 100% [[Workflow Completion]] — это принципиально новое явление.
- **[[Implementation Layer]] — главное узкое место.** Сами [[Frontier Labs]] (OpenAI) заявляют: узкое место не модель, а слой имплементации — комплекс инфраструктуры вокруг агента внутри компании.
- **Кастомизация вытесняет commoditization.** Диспропорциональная ценность лежит не в дженерик-продукте, а в глубокой интеграции в [[Implementation Fabric]] конкретного предприятия.
- **Необходимость [[Forward Deployed Engineer]].** Высокоценная имплементация требует инженеров «в окопах» у клиента — это не решается weekend-проектом в Claude Code.

---

## Терминология

| Термин (RU) | EN | Определение |
|---|---|---|
| «SaaS на вкус как курица» | SaaS Tastes Like Chicken | Финансовое выражение: все SaaS-компании одинаковы по балансовым метрикам и предсказуемы как инвестиция |
| [[Implementation Layer]] / [[Harness]] | Implementation Layer / Harness | Вся инфраструктура вокруг модели: дизайн воркфлоу, права доступа к данным, бизнес-правила, аудит |
| [[Forward Deployed Engineer]] | Forward Deployed Engineer | Технический специалист, встроенный в среду клиента для решения имплементационных задач «в поле» |
| [[Evals]] | Evals | Не бенчмарки, а метод оценки соответствия выходных данных агента конкретным бизнес-правилам |
| [[Systems of Record]] | Systems of Record | Корпоративные платформы (Salesforce, SAP, ServiceNow), хранящие авторитетные данные; открывают API для защиты позиций |
| [[Business Object]] | Business Object | Конкретные сущности, которыми управляет воркфлоу: case, policy, escalation path, sales funnel stage |
| [[Implementation Fabric]] | Implementation Fabric | Интегрированный субстрат данных и логики, поверх которого работают агенты конкретной компании |
| Частный капитал как канал дистрибуции | PE as Distribution Channel | PE-фирмы владеют тысячами mid-market компаний и могут стандартизировать деплой одного партнёра по всему портфелю |

---

## Фреймворки

### [[Four Axes of Pressure]] — четыре оси давления на рынок агентских воркфлоу

| Ось | Кто движется | Направление |
|---|---|---|
| 1 | [[Frontier Labs]] (OpenAI, Anthropic) | Вниз по стеку: создают deployment-компании, нанимают [[Forward Deployed Engineer]] |
| 2 | Консалтинг (McKinsey, BCG, Accenture) | Вверх по стеку: строят agentic-практики, обучают delivery-команды production-деплою |
| 3 | [[Systems of Record]] (Salesforce, SAP, ServiceNow) | Открывают API/agent frameworks, чтобы агенты вызывали их напрямую, вытесняя посредников |
| 4 | Private Equity | Становится каналом дистрибуции: стандартизирует playbooks по портфелю из тысяч компаний |

### Компоненты [[Implementation Layer]]

1. **Workflow Design** — какие решения принимает модель, где остаётся человек, что считается «выполнено»
2. **Data Access** — источники истины, разрешения на уровне строк и полей, свежесть данных
3. **Authority** — лимиты на действия агента; read vs write — принципиально разные профили риска
4. **[[Evals]]** — оценка соответствия выходных данных бизнес-правилам
5. **[[Audit Trails]] & Recovery** — логирование, реконструкция после сбоя, откат действий

### [[Object-Oriented AI Model]]

Стратегический подход: агент прикрепляется к «субстрату» [[Business Object]] (sales funnel, support case) и действует поверх него надёжно и последовательно. Ценность не в абстрактных рассуждениях, а в понимании конкретных объектов конкретного бизнеса.

---

## Формулы / Паттерны

> "SaaS companies all taste like chicken"
> *«Все SaaS-компании одинаковы на вкус» — формула PE-инвесторов, описывавшая предсказуемость SaaS как класса активов.*

> "forward deployed engineers who have to sit in the weeds with customers"
> *«Форвард-деплоенные инженеры, которые должны сидеть в окопах вместе с клиентами».*

> "the way an implementation layer assembles a model assembles a harness assembles data into an actionable workflow"
> *«То, как [[Implementation Layer]] собирает модель, собирает [[Harness]], собирает данные в actionable-воркфлоу» — в этой сборке и лежит реальный [[Moat]].*

> "sit closer to the business object"
> *«Садись ближе к бизнес-объекту» — главный принцип продуктовой стратегии на ближайшие 12 месяцев.*

> "standardize the playbooks where the same patterns repeat very quickly"
> *«Стандартизировать playbooks там, где одни паттерны повторяются снова и снова» — логика PE как канала дистрибуции.*

---

## Открытые вопросы

- **Кто захватит владение?** Кто в итоге «явно претендует на ownership» пространства агентских воркфлоу — лабы, консалтинг, [[Systems of Record]] или сами предприятия?
- **Где главный рычаг?** В данных, модели, [[Harness]] или памяти (memory)? Ответ не дан — называется как открытая битва.
- **Паралич выбора.** Как компании навигируют «choice paralysis», когда все вендоры одновременно сходятся на одном триллионном рынке?
- **Масштабируемость кастомизации.** Может ли бизнес-модель, основанная на глубокой кастомизации, масштабироваться — или она структурно ограничена единичными сделками?

---

## Что использовать для нашего портфеля

**Контекст: AI-интегратор, [[Implementation Layer]], [[Business Object]], PE как канал.**

- **[[Object-Oriented AI Model]] — наша точка входа.** Для каждого клиента нужно выявлять ключевые [[Business Object]] (case, policy, deal stage) и строить [[Implementation Fabric]] вокруг них, а не предлагать дженерик-агента поверх данных. Это создаёт [[Moat]], который лабы не могут легко заменить product release'ом.
- **[[Implementation Layer]] как продукт, не услуга.** Компоненты (Workflow Design, Data Access, Authority, [[Evals]], [[Audit Trails]]) — наш deliverable. Вендоры, которые «продают доступ к данным», проигрывают; побеждают те, кто строит и остаётся владеть слоем.
- **PE как канал дистрибуции — стратегический приоритет.** Партнёрство с одной PE-структурой даёт доступ к портфелю из десятков компаний с повторяющимися паттернами. Это принципиально другой CAC, чем продажа enterprise one-to-one.
- **[[Forward Deployed Engineer]] — наша модель доставки.** Нельзя продать [[Implementation Layer]] дистанционно. Нужна модель «в окопах» — это и дифференциатор, и барьер входа для конкурентов без такой экспертизы.
- **Открытый вопрос для нас:** Какой [[Business Object]] в нашем целевом сегменте является наиболее повторяемым и недостаточно покрытым существующими [[Systems of Record]]?