# Параллельное программирование

## Структура курса

- Разделяемая память и потоки, атомарные операции, memory mapped files
- Проблемы и понятия: race condition, deadlock, livelock, синхронизация, critical section
- Подходы к решению задач: локинг, потокобезопасные и потоконезависимые структуры данных
- Примитивы параллельного программирования в операционных системах
- Мьютексы, Фьютексы и семафоры в том числе бинарные, рекурсивные и легковесные
- Условные переменные, сравнение их с семафорами, оптимизация параллельных программ
- Барьерная синхронизация, спинлоки и синхронизация в юзерспейсе
- Read-write блокировки (много параллельно читают, но только один эксклюзивно пишет)
- Другие подходы: транзакционная память, модель акторов, map/reduce, сети петри
- Другие подходы: асинхронное программирование, реактор, корутины, фьючеры и монады
- Практическое применение Java Threads, C# Tasks
- Параллельное программирование на OpenMP и MPI
- Алгоритмы консенсуса, CAP-теорема и распределенные системы

## Видео-лекции

- [Межпроцессовое взаимодействие в Node.js](https://youtu.be/2OXWZFMvfbc)
  - Примеры кода: https://github.com/HowProgrammingWorks/InterProcessCommunication
- [Atomics, SharedArrayBuffer, worker_threads в Node.js](https://youtu.be/zLm8pnbxSII)
  - Потоки: https://github.com/HowProgrammingWorks/Threads/
  - Атомарные операции: https://github.com/HowProgrammingWorks/Atomics/
- [Семафоры и мьютексы в JavaScript и Node.js](https://youtu.be/JNLrITevhRI)
  - Семафоры: https://github.com/HowProgrammingWorks/Semaphore
  - Мьютексы: https://github.com/HowProgrammingWorks/Mutex
- [Модель акторов (Actor Model)](https://youtu.be/xp5MVKEqxY4)
  - Примеры кода: https://github.com/HowProgrammingWorks/ActorModel
- [Разделяемая память в многопоточном Node.js](https://youtu.be/KNsm_iIQt7U)
