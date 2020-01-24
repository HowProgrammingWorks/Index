# Технологический стек Node.js

Объем материала: 38 лекций, 37 репозиториев с примерами кода, 4 PDF со слайдами.
Перед основной частью курса по Node.js нужно сначала освоить хоть частично курс
по асинхронному программированию: https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Asynchronous.md

## Введение и основы

- [Node.js Введение в технологию](https://youtu.be/WBcHgaoHh1k)
- [Node.js в 2019 году](https://youtu.be/CUU49jjHloM)
  - Слайды: https://www.slideshare.net/tshemsedinov/nodejs-in-2019
- [Асинхронное программирование в Node.js](https://youtu.be/hY6Z6qNYzmc)
  - Это только обзорная лекция, ссылка на курс по асинхронному программированию
  находится выше, перед оглавлением
- [Обзор встроенного Node.js API](https://youtu.be/sOkjR-N6IAs)
  - Ссылка на документацию: https://nodejs.org/api/documentation.html
- [Настройка среды: Node.js, npm, git, eslint](https://youtu.be/hSyA7tcNaCE)
  - Репозиторий с инстрементами: https://github.com/HowProgrammingWorks/Tools
- [Работа с файлами, буферами и файловыми потоками в Node.js](https://youtu.be/eQGBS15vUac)
  - Работа с файлами: https://github.com/HowProgrammingWorks/Files
  - Файловые потоки: https://github.com/HowProgrammingWorks/Streams
  - Буферы: https://github.com/HowProgrammingWorks/Buffers
- [Наблюдение за файловой системой в Node.js](https://youtu.be/29QINR9rruQ)
  - Файловая система в Node.js: https://github.com/HowProgrammingWorks/Files
  - Наблюдение за файлами: https://github.com/HowProgrammingWorks/FilesystemWatch
- [Консоль и командная строка в JavaScript и Node.js](https://youtu.be/5aSZyKi5BmE)
  - Примеры кода: https://github.com/HowProgrammingWorks/CommandLine

## Структура и архитектура приложений на Node.js

- [Архитектурный подход к программированию](https://youtu.be/d_vyO2CkiOc)
- [Модули, слои, структура проекта, песочницы в JavaScript и Node.js](https://youtu.be/O7A9chb573E)
  - Пример проекта: https://github.com/HowProgrammingWorks/Project
  - Абстрактные слои: https://github.com/HowProgrammingWorks/AbstractionLayers
  - Песочницы: https://github.com/HowProgrammingWorks/Sandboxes
- [Инверсия управления и внедрение зависимостей в Node.js](https://youtu.be/Fz86Fdjz-LM)
  - Инверсия управления: https://github.com/HowProgrammingWorks/InversionOfControl
  - Внедрение зависимостей: https://github.com/HowProgrammingWorks/DependencyInjection
- [Межпроцессовое взаимодействие в Node.js](https://youtu.be/2OXWZFMvfbc)
  - Примеры кода: https://github.com/HowProgrammingWorks/InterProcessCommunication
- [Слои, связанность и связность кода](https://youtu.be/A3RpwNlVeyY)
  - Примеры кода: https://github.com/HowProgrammingWorks/Abstractions

## Разработка серверов приложений и API на Node.js

- [Клиент-сервер на Node.js TCP и UDP, DNS](https://youtu.be/bHn-wTlTTR0)
  - Примеры кода: https://github.com/HowProgrammingWorks/Socket
- [HTTP сервер на Node.js (routing, cluster, IP sticky)](https://youtu.be/7Ufxj0oTaUo)
  - Примеры кода: https://github.com/HowProgrammingWorks/NodeServer
- [HTTP сессии и cookies на чистом Node.js](https://youtu.be/T_wKXuWW4Wo)
  - Примеры кода: https://github.com/HowProgrammingWorks/Session
- [HTTP запросы в браузере и Node.js: XMLHttpRequest, fetch](https://youtu.be/wMMki2FEYGY)
  - Примеры кода: https://github.com/HowProgrammingWorks/HttpRequest
- [Разработка API на Node.js (клиент и сервер)](https://youtu.be/-az912XBCu8)
  - Примеры кода: https://github.com/HowProgrammingWorks/API
- [WebSocket сервер на Node.js (электронные таблицы и чат)](https://youtu.be/Sf7ln3n16ws)
  - Вебсокеты: https://github.com/HowProgrammingWorks/WebsocketChat
  - Чат: https://github.com/HowProgrammingWorks/LiveTable
- [Скаффолдинг для API, UI и данных](https://youtu.be/lipkLQVqDd8)
  - Примеры кода: https://github.com/HowProgrammingWorks/Scaffolding
- [Высоконагруженные распределенные приложения на Node.js](https://youtu.be/7tfZDABPvVs)
- [Отдача статики в Node.js](https://youtu.be/n_AdKIzbpBc)
  - Примеры кода и задачи: https://github.com/HowProgrammingWorks/ServeStatic

## Работа с базами данных на Node.js

- [Слой доступа к данным, курсор, транзакция](https://youtu.be/CRcSWtWVvrA)
  - Примеры кода: https://github.com/HowProgrammingWorks/Transaction
- [Работа с базами данных в Node.js на примере PostgreSQL](https://youtu.be/2tDvHQCBt3w)
  - Примеры кода: https://github.com/HowProgrammingWorks/Databases

## Лекции по CQRS и Event Sourcing

- [Паттерн Команда (Command) действие и параметры как объект](https://youtu.be/vER0vYL4hM4)
  - Этот паттерн понадобится для следующей лекции
  - Примеры кода: https://github.com/HowProgrammingWorks/Command
- [CQS, CQRS, Event Sourcing - Разделение запросов и модификации данных](https://youtu.be/T2tRc80Q8Qw)
  - CQS: https://github.com/HowProgrammingWorks/CQS
  - CQRS: https://github.com/HowProgrammingWorks/CQRS
  - EventSourcing: https://github.com/HowProgrammingWorks/EventSourcing
- [Применение EventSourcing](https://youtu.be/kFNtKiK2SPs)
  - См. примеры из предыдущей лекции
- [Модель акторов (Actor Model)](https://youtu.be/xp5MVKEqxY4)
  - Примеры кода: https://github.com/HowProgrammingWorks/ActorModel

## Управление памятью и параллельное программирование

- [Утечки памяти в Node.js и JavaScript, сборка мусора и профилирование](https://youtu.be/0oZa64SB2wM)
  - Примеры кода: https://github.com/HowProgrammingWorks/MemoryLeaks
- [Atomics, SharedArrayBuffer, worker_threads в Node.js](https://youtu.be/zLm8pnbxSII)
  - Потоки: https://github.com/HowProgrammingWorks/Threads/
  - Атомарные операции: https://github.com/HowProgrammingWorks/Atomics/
- [Семафоры и мьютексы в JavaScript и Node.js](https://youtu.be/JNLrITevhRI)
  - Семафоры: https://github.com/HowProgrammingWorks/Semaphore
  - Мьютексы: https://github.com/HowProgrammingWorks/Mutex
- [Разделяемая память в многопоточном Node.js](https://youtu.be/KNsm_iIQt7U) -
доклад на конференции JS Fest 2019 Spring
  - Слайды: https://www.slideshare.net/JSFestUA/js-fest-2019-nodejs

## Безопасность, надежность, развертывание и управление инфраструктурой

- [Необработанные ошибки в промисах](https://youtu.be/1Ml5NE2fsZ8)
  - Примеры кода: https://github.com/HowProgrammingWorks/PromiseError
- [Проблема асинхронного стектрейса в JavaScript и Node.js](https://youtu.be/pfiHTx3j87Y)
  - Примеры кода: https://github.com/HowProgrammingWorks/StackTrace
- [Логирование на Node.js и JavaScript](https://youtu.be/4DkZj2Cdokc)
  - Примеры кода: https://github.com/HowProgrammingWorks/Logging
- [Graceful Shutdown в Node.js](https://youtu.be/ZstnowFeCe0)
  - Примеры кода и задачи: https://github.com/HowProgrammingWorks/GracefulShutdown
- [Безопасность приложений Node.js](https://youtu.be/Pdfo1G-gI6s)
  - Слайды: https://www.slideshare.net/tshemsedinov/nodejs-security-199004963
- [Serverless Clouds (FaaS) и изоляция контекстов запросов в Node.js](https://youtu.be/x-Rd6fPV6L8)
  - Слайды: https://www.slideshare.net/tshemsedinov/serverless-clouds-faas-and-request-context-isolation-in-nodejs
