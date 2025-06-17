# Software Structure & Architecture

1. Introduction
2. Layered (onion), DDD, Clean architecture
3. App structure, Modularity, DI, unittesting
4. DTOs, models, race conditions
5. Hexagonal Architecture, ports and adapters architecture
6. Clustering, Parallel, Distributed systems, CAP, ACID, BASE, Locking, CQRS
7. Actor Model
8. Databases, data modeling
9. Domain Specific Languages: DSL, AST, LISP
10. Command, QueryObject, CQS, CQRS, EventSourcing
11. Messaging: MQ, Pub/Sub, Pull
12. System integration and topology: API, bus, brocker, MQ
13. Communication styles: data, call, event, log sync, p2p, blockchain
14. Feature-Sliced Design
15. Architecture for Web: DDD for Frontend and Backend
16. Data access patterns
17. Asynchronous programming
18. Imperative shell, Functional core
19. Multi-paradigm programming in Architecture
20. Metaprogramming

## Students seminar topics

Timing: 30-60 min + discussion (min 30 min)
Requirements: PDF or MD file in github repo, presentation google docs
Topic: please propose before call in 3-7 days

- Pipeline architecture
- SOA: web services, microservices, serverless
- One of noSQL db solution
- Task and resource schedulers
- Testing, quality assessments
- Infrastructure, deployment, CI/CD
- DB Migration
- DB Balancing and sharding
- DB replication
- DB Backups and recovery
- API Balancing
- Application and system logging
- Law of Demeter (LoD) // See comments in next section
- DAL (data access layer)
- Dependency injection & Inversion of Control (for your language)
- DDD: Value object, Null object, DTO, Active Record, Data access object, Data mapper
- Blockchain: voting system for decision making and specialist selecting; registers; distributed data storage // Andrii Schavinskyi
- Object-relational mismatch (from Kleppmann)
- Cache strategies
- Indexing structures
- Serialization formats comparison and evolution: binary files, xml, yml, json, protobuf, v8 ser format, etc.
- DB ACID // Fowler
- Locking and offline concurrency patterns // Fowler
- Sessions: session token, JWT token

## Books

- «Patterns of Enterprise Application Architecture» Martin Fowler
- «Designing Data-intensive Applications» Martin Kleppmann
- «Clean Architecture: A Craftsman's Guide to Software Structure and Design» Robert C. Martin
- «Refactoring: Improving the Design of Existing Code Edition Unstated» Martin Fowler, Kent Beck, John Brant, William Opdyke, Don Roberts, Erich Gamma
- «Working Effectively with Legacy Code» Robert C. Martin
- «Clean Agile: Back to Basics» Robert C. Martin
- «Clean Craftsmanship: Disciplines, Standards, and Ethics» Robert C. Martin
- «Functional Design: Principles, Patterns, and Practices» Robert C. Martin
- Computation theory: Turing, von Neumann, Curry, Church
- Ludwig Wittgenstein 
- Avram Noam Chomsky- A Pattern Language: Towns, Buildings, Construction // Christopher W. Alexander
- Cybernetics: Norbert Wiener and Victor Mikhailovich Glushkov
- System approach: Ludwig von Bertalanffy, William Ross Ashby
- Stafford Beer

## Additional topics

- Pipeline architecture
- SOA: web services, microservices, serverless
- Data warehouses and DBMS: relational, noSQL, columnar, key-value
- API Design
- Corporate integration buses (exchange with external subsystems)
- Task and resource schedulers
- Testing, quality assessments, continuous integration
- Infrastructure, deployment, update, migration, reengineering
- Balancing, replication, sharding, resharding, backups and recovery
- Security, authorization, authentication, application firewall
- Application and system logging, incident investigation
- Analysis and reengineering of business processes
- Law of Demeter (LoD) - Principle of Least Knowledge or Don't Talk to Strangers
  - Low Coupling (LC): The goal of LoD is to reduce coupling by reducing the knowledge of a class about other classes.
  - Tell, Don't Ask/Information Expert (TdA/IE): LoD is more specific than TdA/IE because TdA/IE can be applied in a wider context (e.g. for responsibility assignment). Applying TdA leads to solutions which are good according to LoD. Note that the reverse is not true: According to LoD you may get and set values from an object passed as a parameter to a method.
  - A method of an object should invoke only the methods of the following kinds of objects:
    - itself
    - its parameters
    - any objects it creates/instantiates
    - its direct component objects

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
