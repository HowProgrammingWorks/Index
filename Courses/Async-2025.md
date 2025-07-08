# Асинхронное программирование 2025

Те способы писать асинхронный код, которые мы использовали 10-15 лет назад безвозвратно уходят в прошлое и могут быть интересны лишь для поддержки легаси упражнения в глубоком понимании асинхронного программирования. Даже способы 5-7 летней давности уже имеют мало общего с современными практиками, но интернет полон устаревшей информации, даже [открытый курс сообщества Metarhia](https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Asynchronous.md) на сегодняшний момент стал слишком громоздким и излишним. Еще нужно упомянуть о том, что в системном и прикладном коде асинхронное программирование должно выглядеть принципиально по-разному. Полностью скрыть от продуктового разработчика сложность асинхронного кода за абстракциями не удастся, потому, что он в любом случае будет работать с таймерами, событиями, стримами, fetch и другими асинхронными API, но его можно писать в десятки раз проще, чем асинхронный код в системном слое. Что касается системного слоя, то нужно вводить в обиход теорию очередей (системы массового обслуживания), модель акторов, часть абстракций из параллельного программирования (семафоры, рандеву, атомарные операции). Конечно, содержать все это в одном курсе сложновато, поэтому, мы отдадим приоритет прикладному коду и сначала полностью подготовим курс для применения асинхронного программирования в продуктовой разработке, а потом будем добавлять необязательные темы из старого курса и много других полезных абстракций, широко распространенных в других языках программирования, но слабо известных в мире JavaScript.

## Содержание

Важные аспекты нового курса:

- Концентрация на практическом применении (примеры кода из реальных проектов)
- Актуальность и соответствие стандартам по состоянию на 2023-2025
- Задачи и разбор их решений, семинары, ревью кода (курс это не только видео)
- Рекомендации к выбору стиля и абстракций асинхронности под задачу
- Внимание к корректной обработке ошибок во всех стилях асинхронности
- Упор на надежность, поддерживаемость, тестируемость, снижение зацепления
- Примеры и задачи по исправлению скрытых проблемных состояний и data races

Для того, чтобы писать прикладной код хватит первого столбика таблицы (а в оглавлении темы помечены 💯). Второй столбик полезен, как дополнительные знания, (углубленное изучение помечено как 🧑‍🎓). Для бекенда на ноде нужно освоить два первых столбика. Третий столбик содержит системные вещи (помечены ⚙️ в оглавлении), которые нужны для разработки инструментов, платформ и библиотек. Четвертый столбик (помечен 🧑‍🚀) это дополнительные абстракции, которые можно осваивать выборочно, они понадобятся не всем, но если вы работаете в проектах, где много функционального и/или реактивного программирования. Пятый столбик - вещи, которые морально устарели и могут рассматриваться как интересный антиквариат (помечены ⚠️).

| Applied 💯     | Advanced 🧑‍🎓                | System ⚙️           | Elective 🧑‍🚀           | Legacy ⚠️          |
|:--------------|:--------------------------|:-------------------|:---------------------|:------------------|
| `callbacks`   | `AsyncQueue`              | `Thenable`         | `compose callbacks`  | `Deferred`        |
| `promises`    | `AsyncPool`               | `Semaphore`        | `async compose`      | `function*/yield` |
| `async/await` | `AsyncCollector`          | `Mutex`            | `Observer`           | `Async.js`        |
| `events`      | `Chain of responsibility` | `Spin Lock`        | `RxJS`               | `Metasync`        |
| `streams`     | `Async Generator`         | `MessageChannel`   | `Future`             | `middleware`      |
| `signals`     | `GoF pattern Iterator`    | `BroadcastChannel` | `coroutines`         |                   |
| `locks`       | `Actor pattern`           | `threads`          | `Actor Model`        |                   |
| `iterators`   | `Disposable`              | `processes`        | `do`                 |                   |

Условные обозначения: ⭐ новые лекции, ✨ открытые старые лекции, 💯 обязательные, 🧑‍🎓 продвинутые, ⚙️ системные, 🧑‍🚀 по выбору, ⚠️ устаревшее, 🧩 необязательные темы, 💻 примеры кода, 🧑‍💻 задания

- 💯 Контракты асинхронности на базе callback
  - ⭐ Контракты `Callback` и `Callback-last-error-first` (ссылка в платном курсе)
  - 💻 Колбеки: https://github.com/HowProgrammingWorks/Callbacks
  - 💻 Примеры кода с колбеками: https://github.com/HowProgrammingWorks/AsynchronousProgramming
  - 🧑‍💻 [Задания по колбекам](https://github.com/HowProgrammingWorks/Callbacks/tree/master/JavaScript/Tasks) (решения, ревью и разбор в платном курсе)
- 💯 Минимально необходимое понимание рантайма: event loop, I/O, таймеры
  - ⭐ Фазы Event-loop в V8 и Node.js (ссылка в платном курсе)
  - 🧩 [Стрим с разбрром Event loop и асинхронности](https://www.youtube.com/live/ND5HNHicACI)
  - 💻 Таймеры: https://github.com/HowProgrammingWorks/Timers
  - 🧑‍💻 Задания по таймерам (в платном курсе)
- 💯 Контракты на базе событий `EventTarget`, `EventEmitter`
  - ⭐ События (ссылка в платном курсе)
  - 🧑‍💻 [Задания по событиям](https://github.com/HowProgrammingWorks/Events/tree/main/JavaScript/Tasks) (решения, ревью и разбор в платном курсе)
  - ✨ [EventEmitter из старой лекции](https://youtu.be/LK2jveAnRNg)
  - 💻 EventEmitter: https://github.com/HowProgrammingWorks/EventEmitter
- 💯 Абстракция потоков `Stream`
  - ⭐ Стримы Readable, Writable, Transform, открытый конструктор, буферизация, backpressure  (ссылка в платном курсе)
  - 🧑‍💻 Задания по стримам (в платном курсе)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Streams/tree/master/JavaScript
  - ✨ [Паттерн открытый конструктор (Revealing Constructor)](https://youtu.be/leR5sXRkuJI)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/RevealingConstructor
- ⚙️ Контракт `Thenable`
  - ⭐ Контракт `Thenabe` (ссылка в платном курсе)
  - ✨ [Thenable из старой лекции](https://youtu.be/Jdf_tZuJbHI)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Thenable
  - 🧑‍💻 [Задания по `Thenabe`Thenable](https://github.com/HowProgrammingWorks/Thenable/tree/master/JavaScript/Tasks) (решения, ревью и разбор в платном курсе)
- 💯 Контракт `Promise`
  - ⭐ Promise: then/catch/finally и методы класса all, allSettled, race, any (ссылка в платном курсе)
  - ✨ [Асинхронность на промисах из старой лекции](https://youtu.be/RMl4r6s1Y8M)
  - 💻 [Примеры кода](https://github.com/HowProgrammingWorks/Promise/tree/master/JavaScript)
  - 🧑‍💻 [Задания по `Promise`](https://github.com/HowProgrammingWorks/Promise/tree/master/JavaScript/Tasks) (решения, ревью и разбор в платном курсе)
- 💯 Контракт асинхронных функций `async/await`
  - ⭐ Асинхронные функции (ссылка в платном курсе)
  - ✨ [Асинхронные функции из старой лекции](https://youtu.be/Jdf_tZuJbHI)
  - 💻 [Примеры кода](https://github.com/HowProgrammingWorks/AsyncFunction/tree/main/JavaScript)
  - 🧑‍💻 [Задания по `async/await`](https://github.com/HowProgrammingWorks/AsyncAwait/tree/master/JavaScript/Tasks) (решения, ревью и разбор в платном курсе)
- 💯 Контракт сигналов `signals`
  - ⭐ Сигналы (в платном курсе)
  - 💻 Примеры кода: (готовятся), будут тут https://github.com/HowProgrammingWorks/Signals
  - 🧑‍💻 Задания по сигналам (в платном курсе)
- 💯 Обработка ошибок, их выявление и решение проблем со стектрейсом
  - ✨ [Обработка ошибок из старой лекции](https://youtu.be/Jdf_tZuJbHI)
  - 💻 Примеры кода
  - 💻 Примеры кода из старого курса: https://github.com/HowProgrammingWorks/AsyncAwait
  - 💻 Примеры кода: (готовятся), будут тут https://github.com/HowProgrammingWorks/AsyncErrorHandling
  - 🧑‍💻 Задания по обработке ошибок
- 🧑‍🎓 Контракт `Disposable`
  - ⭐ Явное управление ресурсами (Explicit Resource Management)
  - ⭐ Подсчет ссылок и освобождение ресурсов на базе `Disposable`
  - ⭐ Реализация концепции `Ownership` на базе `Disposable`
- 🧑‍🎓 Асинхронная очередь `AsyncQueue`
  - ⭐ Асинхронная очередь (в платном курсе)
  - ✨ Конкурентная асинхронная очередь из старой лекции](https://youtu.be/Lg46AH8wFvg)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/ConcurrentQueue
  - 💻 Примеры кода: (готовятся), будут тут https://github.com/HowProgrammingWorks/AsyncQueue
- 🧑‍🎓 Асинхронный пул `AsyncPool`
  - ✨ [Асинхронный пул для worker thread pool в Node.js](https://youtu.be/Jj5KZRq4wYI)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Pool
  - 💻 Примеры кода: (готовятся), будут тут https://github.com/HowProgrammingWorks/AsyncPool
- 🧑‍🎓 Асинхронная коллекция `Collector`
  - 🧩 Асинхронные коллекции (собираем значения до готовности)
  - ✨ [Асинхронные коллекторы данных](https://youtu.be/tgodt1JL6II)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Collector
- 🧑‍🎓 Паттерн цепочка ответственности `Chain of responsibility`
  - 💻 Примеры кода: (готовятся), будут тут https://github.com/HowProgrammingWorks/ChainOfResponsibility
- 🧑‍🎓 Конвертеры контрактов `asyncify`, `callbackify`, стыковка кода в разных стилях
  - ⭐ Асинхронные адаптеры (в платном курсе)
  - ✨ [Асинхронные адаптеры из старой лекции](https://youtu.be/76k6_YkYRmU)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/AsyncAdapter
  - 🧑‍💻 Задания по адаптерам (в платном курсе)
- 🧑‍🎓 Предотвращение состояния гонки по данным и управлению в асинхронном коде (в платном курсе)
- 🧑‍🎓 Отмена асинхронных операций: `AbortController`, `AbortSignal` (в платном курсе)
  - 🧩 Документация на MDN: https://developer.mozilla.org/en-US/docs/Web/API/AbortController
- 🧑‍🎓 `Async Generator` и `Async Iterator` (в платном курсе)
  - ✨ [Генераторы и асинхронные генераторы из старой лекции](https://youtu.be/kvNm9D32s8s)
- ⚙️ Абстракции портированные из параллельного программирования в асинхронное
  - 🧩 Асинхронные абстракции: `Semaphore`, `Mutex`
  - 🧩 Блокировки `Lock`, `Spin Lock`
- ⚙️ Абстракции параллельного программирования
  - 🧩 Системные абстракции: `threads`, `processes`
  - 🧩 Межпроцессовое и межпотоковое взаимодействие, `MessageChannel`, `BroadcastChannel`
  - 🧩 Корутины `coroutines`
- 🧑‍🎓 Асинхронные генераторы и асинхронные итераторы
  - ✨ [Генераторы и асинхронные генераторы из старой лекции](https://youtu.be/kvNm9D32s8s)
  - 💻 Генераторы: https://github.com/HowProgrammingWorks/Generator
  - 💻 Асинхронные генераторы: https://github.com/HowProgrammingWorks/AsyncGenerator
  - ✨ [Итераторы и асинхронные итераторы из старой лекции](https://youtu.be/rBGFlWpVpGs)
  - 💻 Итераторы: https://github.com/HowProgrammingWorks/Iterator
  - 💻 Асинхронные итераторы: https://github.com/HowProgrammingWorks/AsyncIterator
- 🧑‍🚀 Композиция функций на колбеках `compose callbacks`
  - ✨ [Асинхронная композиция функций](https://youtu.be/3ZCrMlMpOrM)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/AsyncCompose
- 🧑‍🚀 Композиция асинхронных функций `async compose`
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/AsyncCompose
- 🧑‍🚀 Асинхронность на потоках событий `RxJS`
  - ✨ Потоки событий, паттерн `Observer/Observable`
  - ✨ [Асинхронность на RxJS из старой лекции](https://youtu.be/0kcpMAl-wfE)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Rx
- 🧑‍🚀 Модель акторов `actor model`
  - ✨ [Модель акторов](https://youtu.be/xp5MVKEqxY4)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/ActorModel
- 🧑‍🚀 Библиотека `do`: https://www.npmjs.com/package/do
- 🧑‍🚀 Функциональное асинхронное программирование, контракт `Future`
  - ✨ [Асинхронность на фьючерах без состояния](https://youtu.be/22ONv3AGXdk)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Future
- ⚠️ Асинхронность на синхронных генераторах `function*/yield`
- ⚠️ Мидлвары `middleware` как антипаттерн: https://youtu.be/RS8x73z4csI
  - 💻 Примеры кода: (готовятся), будут тут https://github.com/HowProgrammingWorks/Middleware
- ⚠️ Контракты семейства `Deferred`
  - ✨ [Deferred: Асинхронность на диферах с состоянием](https://youtu.be/a2fVA1o-ovM)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/Deferred
- ⚠️ Async.js
  - 🧩 [Легаси код на библиотеке `Async.js`](https://youtu.be/XQ94wQc-erU)
  - 💻 Примеры кода: https://github.com/HowProgrammingWorks/AsynchronousProgramming
- ⚠️ Коллекция асинхронных абстракций `Metasync`: https://www.npmjs.com/package/metasync
  - ✨ [Архивная лекция](https://youtu.be/xNfOv9I1MDk)
- ⚙️ Трекинг асинхронных контекстов
  - ⭐ AsyncLocalStorage, AsyncResource (в платном курсе)
  - 💻 Примеры использования AsyncLocalStorage и AsyncResource: https://github.com/HowProgrammingWorks/AsyncContextTracking
- ⚙️ Процессы и потоки
  - 🧩 [Многопоточность в Node.js](https://youtu.be/VNXga8zomrY)
  - 🧩 [Web Locks API in Node.js and browser](https://youtu.be/auMM-uV12F0)

## Обратите внимание

Что нужно знать и уметь на входе:

- 🔗 [Синтаксис JavaScript без всяких триков](https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Fundamentals.md)  
- 💡 Уверенно владеть git, иметь github аккаунт
- 💡 Любая среда разработки, IDE или редактор

Чем это курс не является: это не чтение документации, не курс по библиотекам и фреймворкам, не повторение старого курса, не лайвкодинг и не мастеркласс, не стрим. Новый курс - это максимально сконцентрированная информация и практические задачи как для прикладного, так и для системного программирования со сравнением этих подходов.

## Как попасть на курс

🎫 Регистрация: следите за публикациями чтобы не пропустить начало регистрации.

👉 Новости курса будут в канале: https://t.me/asyncify  
👉 Открытая группа курса: https://t.me/asynctalks  
👉 Подписывайтесь на https://t.me/metarhia и https://www.youtube.com/@TimurShemsedinov чтобы следить за новостями
