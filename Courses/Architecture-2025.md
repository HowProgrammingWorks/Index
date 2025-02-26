# Software Structure & Architecture

1. Introduction
2. Layered (onion), DDD, Clean architecture
3. App structure, Modularity, DI, unittesting
4. DTOs, models, race conditions
5. Hexagonal Architecture, ports and adapters architecture
6. Clustering, Parallel, Distributed systems, CAP, ACID, BASE, Locking, CQRS
7. Actor Model
8. Databases, data modeling
9. DSL, AST, LISP
10. Command, QueryObject, CQS, CQRS, EventSourcing
11. Messaging: MQ, Pub/Sub, Pull
12. System integration: api, bus, brocker, mq
13. Communication styles: data, call, events, log, p2p
14. Architecture for Web: Frontend and Backend

Additional topics:
- Interaction: Data (shared state), Calls (RPC), Events (MQ)
- Three-Tier Architecture, Multitier, Pipeline
- SOA: web services microservices, serverless
- Data warehouses and DBMS: relational, noSQL, columnar, key-value
- Distributed IS topologies: star, bus, ring, pipeline, fully connected
- API Design
- Corporate integration buses (exchange with external subsystems)
- Task and resource schedulers
- Testing, quality assessments, continuous integration
- Infrastructure, deployment, update, migration, reengineering
- Balancing, replication, sharding, resharding, backups and recovery
- Security, authorization, authentication, application firewall
- Application and system logging, incident investigation
- Analysis and reengineering of business processes

## Old lectures

- [Архитектурный подход к программированию](https://youtu.be/d_vyO2CkiOc)
- [Слои, связанность и связность кода](https://youtu.be/A3RpwNlVeyY)
  - Примеры кода: https://github.com/HowProgrammingWorks/Abstractions
- [Модули, слои, структура проекта, песочницы в JavaScript и Node.js](https://youtu.be/O7A9chb573E)
  - Пример проекта: https://github.com/HowProgrammingWorks/Project
  - Абстрактные слои: https://github.com/HowProgrammingWorks/AbstractionLayers
  - Песочницы: https://github.com/HowProgrammingWorks/Sandboxes
- [Инверсия управления и внедрение зависимостей в Node.js](https://youtu.be/Fz86Fdjz-LM)
  - Инверсия управления: https://github.com/HowProgrammingWorks/InversionOfControl
  - Внедрение зависимостей: https://github.com/HowProgrammingWorks/DependencyInjection
- [Межпроцессовое взаимодействие в Node.js](https://youtu.be/2OXWZFMvfbc)
  - Примеры кода: https://github.com/HowProgrammingWorks/InterProcessCommunication
- [Высоконагруженные распределенные приложения на Node.js](https://youtu.be/7tfZDABPvVs)
- [Слой доступа к данным, курсор, транзакция](https://youtu.be/CRcSWtWVvrA)
  - Примеры кода: https://github.com/HowProgrammingWorks/Transaction
- [Разработка API на Node.js (клиент и сервер)](https://youtu.be/-az912XBCu8)
  - Примеры кода: https://github.com/HowProgrammingWorks/API
- [CQS, CQRS, Event Sourcing - Разделение запросов и модификации данных](https://youtu.be/T2tRc80Q8Qw)
  - CQS: https://github.com/HowProgrammingWorks/CQS
  - CQRS: https://github.com/HowProgrammingWorks/CQRS
  - EventSourcing: https://github.com/HowProgrammingWorks/EventSourcing
- [Применение EventSourcing](https://youtu.be/kFNtKiK2SPs)
  - https://github.com/HowProgrammingWorks/EventSourcing
  - https://github.com/HowProgrammingWorks/CQRS
  - https://github.com/HowProgrammingWorks/Command
- [Serverless Clouds (FaaS) и изоляция контекстов запросов в Node.js](https://youtu.be/x-Rd6fPV6L8)
  - Слайды: https://www.slideshare.net/tshemsedinov/serverless-clouds-faas-and-request-context-isolation-in-nodejs

## Additional topics

- Law of Demeter (LoD) - Principle of Least Knowledge or Don't Talk to Strangers
  - Low Coupling (LC): The goal of LoD is to reduce coupling by reducing the knowledge of a class about other classes.
  - Tell, Don't Ask/Information Expert (TdA/IE): LoD is more specific than TdA/IE because TdA/IE can be applied in a wider context (e.g. for responsibility assignment). Applying TdA leads to solutions which are good according to LoD. Note that the reverse is not true: Accoring to LoD you may get and set values from an object passed as a parameter to a method.
  - A method of an object should invoke only the methods of the following kinds of objects:
    - itself
    - its parameters
    - any objects it creates/instantiates
    - its direct component objects
