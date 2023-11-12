# Технологический стек Node.js в 2024

Объем материала: 20 часов лекций, еженедельно 2 часа семинары в течении года, репозитории с примерами кода.
Что нужно знать на входе:
- [Синтаксис JavaScript без всяких триков](https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Fundamentals.md)
- [Основы асинхронного программирования](https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Asynchronous.md)
- Уверенно владеть git, иметь github аккаунт
- Желательно docker, иметь рабочую машину на linux или mac
- Любая среда разработки, IDE или редактор

Ссылки на старый курс:
- [Структура со ссылками на видео и репозитории с примерами кода](NodeJS.md)
- [Для части лекций есть таймкоды и подробное оглавление](NodeJS-timecodes.md)

Чем это курс не является: это не чтение документации, не курс по фреймворкам, не курс по Metarhia, не повторение старого курса, не лайвкодинг и не мастеркласс, не стрим. Новый курс - это максимально сконцентрированная информация и практические задачи по разработке на чистой ноде но с хорошей архитектурой и использованием всех современных возможностей Node.js

👉 Patreon: https://www.patreon.com/tshemsedinov  
👉 Видео обзор курса: (готовится)  
👉 Вопросы на интервью: https://github.com/tshemsedinov/NodeJS-Interview-Questions

## Содержание

- ⭐ [Введение в технологию 🚀](https://youtu.be/mRvzgBGLVyM)
  - 🧑‍💻 [HTTP сервер для статики](https://github.com/HowProgrammingWorks/NodeServer/tree/master/native-2022)
  - 🔗 [Таблица поддержки возможностей в версиях ноды](https://node.green/)
  - 🔗 [Автоматизация проверки безопасности кода](https://snyk.io/)
  - 🔗 [Встроенный в npm аудит безопасности](https://docs.npmjs.com/cli/v8/commands/npm-audit)
  - 🧩 [Сравнение кластеризации HTTP, TCP и UDP на процессах и потоках](https://youtu.be/dum4b4EZktY)
  - 🧩 [Стрим про асинхронность и фазы ивентлупа](https://youtu.be/ND5HNHicACI)
- ⭐ Структура приложений: системы модульности, пакеты и зависимости
  - 💻 [Системы модульности, CommonJS, ESModules, реализация своей системы модульности](https://github.com/HowProgrammingWorks/Modularity)
  - 💻 [Пакеты и их загрузка в разных системах модульности](https://github.com/HowProgrammingWorks/Packages)
- ⭐ Архитектура приложений: слои и внедрение зависимостей
  - 💻 [Пошаговый рефакторинг от мидлварей до слоеной архитектуры](https://github.com/HowProgrammingWorks/DDD)
  - 🧩 [Почему мидлвари это плохо](https://youtu.be/RS8x73z4csI)
- ⭐ Layers and Low Coupling на примере конфига и транспорта
  - 💻 [Примеры кода "A", "B" и "C" к лекции](https://github.com/HowProgrammingWorks/DDD)
- ⭐ Базы данных, модель, заголовки .d.ts и линтеры
- ⭐ Криптография: crypto, хеширование паролей с солью, session token, UUID, случайные числа
  - 💻 Реализация `randomPrefetcher` из библиотеки `metautil`: https://github.com/metarhia/metautil/blob/v3.7.0/lib/crypto.js
  - 💻 Упрощенное хеширование: https://github.com/HowProgrammingWorks/DDD/blob/master/JavaScript/d-messenger/lib/common.js
  - 💻 Полноценное хеширование: https://github.com/metatech-university/NodeJS-Pure/blob/main/lib/common.js
  - 💻 Генерация UUID: https://nodejs.org/api/crypto.html#cryptorandomuuidoptions
  - 🔗 Документация по `node:crypto`: https://nodejs.org/api/crypto.html
- ⭐ [Применение Chat GPT в оптимизации JavaScript для Node.js](https://youtu.be/Ebrzqj8cGUY)
  - 💻 [Chunk encode/decode with typed arrays](https://github.com/HowProgrammingWorks/ChatGPT/tree/main/JavaScript/1-Chunk)
  - 💻 [Promise chain and async code optimization](https://github.com/HowProgrammingWorks/ChatGPT/tree/main/JavaScript/2-Promise)
  - 💻 [Crypto random prefetcher](https://github.com/HowProgrammingWorks/ChatGPT/tree/main/JavaScript/3-Prefetcher)
- ⭐ Структура классов сервера и GoF паттерны в Node.js
- ⭐ Подсистема `Authentication`
- ⭐ Подсистема `Role Based Access Control`
  - Системы прав ACL, ABAC, RBAC, и проектирование нашей системы прав для курса
- ⭐ Стримы Readable, Writable, Transform, открытый конструктор, буферизация, backpressure
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Streams/tree/master/JavaScript
- ⭐ Инфраструктура и инструментарий: тайпинги, тестирование, линтеры, CI/CD, встроенный testing framework
- ⭐ Работа с ошибками и исключениями, `Graceful shutdown` в Node.js, `unhandled exceptions`, `async stack trace`
  - 💻 Async stack trace: https://github.com/HowProgrammingWorks/StackTrace/blob/master/JavaScript/6-pass-through.js
  - 💻 Graceful shutdown: https://github.com/HowProgrammingWorks/GracefulShutdown
- ⭐ Асинхронное, реактивное и параллельное программирование
  - ✨ Обзор асинхронного программирования в Node.js: https://youtu.be/hY6Z6qNYzmc
  - 💻 Разные контракты: https://github.com/HowProgrammingWorks/AsynchronousProgramming
  - 💻 Таймеры: https://github.com/HowProgrammingWorks/Timers
  - 💻 EventEmitter: https://github.com/HowProgrammingWorks/EventEmitter
  - 💻 Промисы: https://github.com/HowProgrammingWorks/Promise
  - 💻 Async/await: https://github.com/HowProgrammingWorks/AsyncAwait
  - 💻 Асинхронные адаптеры: https://github.com/HowProgrammingWorks/AsyncAdapter
  - 💻 Асинхронные итераторы: https://github.com/HowProgrammingWorks/AsyncIterator
  - 💻 Thenable: https://github.com/HowProgrammingWorks/Thenable
  - 💻 Асинхронная очередь: https://github.com/HowProgrammingWorks/ConcurrentQueue
  - 💻 Паттерн открытый конструктор (Revealing Constructor): https://github.com/HowProgrammingWorks/RevealingConstructor
- ⭐ Работа с файлами и файловыми потоками, наблюдение за файловой системой
  - ✨ Работа с файлами, буферами и файловыми потоками: https://youtu.be/eQGBS15vUac
  - 💻 Работа с файлами: https://github.com/HowProgrammingWorks/Files
  - 💻 Файловые потоки: https://github.com/HowProgrammingWorks/Streams
  - 💻 Буферы: https://github.com/HowProgrammingWorks/Buffers
  - 💻 Наблюдение за файлами: https://github.com/HowProgrammingWorks/FilesystemWatch
- ⭐ Принципы `GRASP` и `SOLID` в `JavaScript` с адаптацией для Node.js
  - ✨ GRASP принципы с адаптацией для JavaScript и Node.js: https://youtu.be/ExauFjYV_lQ
  - 💻 Information Expert: https://github.com/HowProgrammingWorks/InformationExpert
  - 💻 Coupling and Cohesion: https://github.com/HowProgrammingWorks/CouplingCohesion
  - 💻 Pure Fabrication: https://github.com/HowProgrammingWorks/PureFabrication
  - 💻 Single responsibility: https://github.com/HowProgrammingWorks/SingleResponsibility
  - 💻 Liskov substitution: https://github.com/HowProgrammingWorks/LiskovSubstitution
  - 💻 IoC and DI: https://github.com/HowProgrammingWorks/InversionOfControl
- ⭐ Вопросы безопасности: `DoS`, `XSS`, `Path traversal`, `CSRF`, `SQL`-инъекции
  - ✨ Безопасность приложений Node.js: https://youtu.be/Pdfo1G-gI6s
  - 🔗 Слайды: https://www.slideshare.net/tshemsedinov/nodejs-security-199004963
- ⭐ C/C++ Addons, Node-API (n-api), WebAssembly: Rust, WAT, C++, AssemblyScript
  - 💻 N-API examples for C++ and Rust: https://github.com/HowProgrammingWorks/Node-API
  - 💻 WebAssembly for C++, Rust, WAT, and AssemblyScript https://github.com/HowProgrammingWorks/WebAssembly
  - 💻 In-place callback solution: https://github.com/tshemsedinov/wasm-import
- ⭐ Трекинг асинхронных контекстов: AsyncLocalStorage, AsyncResource
  - 💻 Примеры использования AsyncLocalStorage и AsyncResource: https://github.com/HowProgrammingWorks/AsyncContextTracking
- ⭐ Проектирование API и проверка контрактов в рантайме
  - ✨ Контрактное программирование: https://youtu.be/K5_kSUvbGEQ
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Contract
- ⭐ Вынесение подсистем как отдельных микросервисов
- ⭐ `Performance hooks`, телеметрия ресурсов и оптимизация: I/O bound, CPU bound, memory bound, профилирование
- ⭐ `Serverless` и облачные `FaaS` решения на базе Node.js
  - ✨ Serverless Clouds (FaaS) и изоляция контекстов запросов в Node.js: https://youtu.be/x-Rd6fPV6L8
  - 🔗 Слайды: https://www.slideshare.net/tshemsedinov/serverless-clouds-faas-and-request-context-isolation-in-nodejs
- ⭐ Приложения, приближенные к реальному времени, Websocket, интерактивность и коллаборативные приложения
  - 💻 Серверная реализация
  - 💻 Клиентская реализация на C++ для Node.js 21
  - 💻 Интерактивность и коллоборативные приложения
- ⭐ Распределенные системы, высоконагруженные системы, балансировка нагрузки, кластеризация и масштабирование, IP sticky
  - ✨ Доклад по высоконагруженным системам: https://youtu.be/7tfZDABPvVs
  - ✨ HTTP сервер на Node.js (routing, cluster, IP sticky): https://youtu.be/7Ufxj0oTaUo
  - 💻 Примеры серверов: https://github.com/HowProgrammingWorks/NodeServer
- ⭐ Изоляция кода и данных в Node.js: `vm`, `v8`, защита `global`, контекстов, модулей и прототипов от патчинга
- ⭐ Структура и архитектура проекта, слои, `DDD`, `Clean architecture`, связанность и связность кода, протекание абстракций

# Доступ

План подписки формируется. Приходите через неделю.
