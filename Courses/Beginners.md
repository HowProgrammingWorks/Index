# Основы программирования

- Автор: https://github.com/tshemsedinov
- Новости в телеграм канале: https://t.me/HowProgrammingWorks
- Для вопросов группа в телеграме: https://t.me/MetarhiaHPW
- Youtube: https://www.youtube.com/@MetatechEducation/playlists

## Оглавление

- ⭐ [Введение](https://youtu.be/2DM5I2CI4gY)
- ⭐ [Идентификаторы: переменные и константы](https://youtu.be/fb318yXGwxo)
- ⭐ [Запись значений и типы данных](https://youtu.be/B1Y00zN31Yg)
- ⭐ [Функции и блоки, область видимости, контексты](https://youtu.be/JdscRDLG9A4)
- ⭐ [Условия и ветвление](https://youtu.be/O_EJ0StSnac)
- ⭐ [Циклы: for, for..of и for..in](https://youtu.be/_Jxe-WacgUs)
- ⭐ [Циклы while и do..while](https://youtu.be/wDVQrZx2dKU)
- ⭐ [Коллекции: массивы и объекты - Array и Object](https://youtu.be/dZJ97DMu2cA)
- ⭐ [Объекты: примеси и сериализация](https://youtu.be/zRr-WZB7AK8)
- 🧑‍💻 [Задачи 1-5](https://github.com/HowProgrammingWorks/Book/blob/master/content/ru/2-9-Tasks.md)
- 🧑‍💻 [Разбор решения задач 1-5](https://youtu.be/WNNJfjL3h3s)
- ⭐ [Коллекции: Множества Set и хеш-таблицы Map](https://youtu.be/OE9DxIBu-8I)
- ⭐ [Callback - функции обратного вызова и Таймеры](https://youtu.be/6eg-WMDejSM)
- ⭐ [Замыкания (closure) функция и контекст](https://youtu.be/LUd-cFkhCrY)
- ⭐ [Async/await - асинхронные функции](https://youtu.be/DrOiZBcWlKg)
- ⭐ [Ошибки (Error), исключения (exceptions), баги, throw, try/catch](https://youtu.be/MF8u1Oj64Dk)
- ⭐ [Системы модульности: ESM (ECMAScript Modules) та CJS (CommonJS)](https://youtu.be/roinnSNNgjs)
- ⭐ [Декомпозиция программы на модули](https://youtu.be/7S6TrUbFMlQ)
- ⭐ [Рекурсия (recursion), выход из нее и стек вызовов (call stack)](https://youtu.be/c1rJema94iY)
- 🧑‍💻 [Задачи: 38 примеров плохого кода для переписывания](https://github.com/HowProgrammingWorks/Exams/tree/master/Tasks)

Продолжение будет...

Более сложные лекции можно найти тут: https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Fundamentals.md

## Рекомендации по решению задач

🧑‍💻 Задачи: https://github.com/HowProgrammingWorks/Exams/tree/master/Tasks

- Код изначально работает, и выдает правильный результат, вам нужно исправлять файл, но не сломать код
- Используйте тесты из каталога `Tests` для проверки решений.
- Ваша задача улучшить: понятность кода, стиль, простоту
- Тут чеклист частых ошибок (они точно должны быть исправлены):
  - Не модифицируйте входные параметры функций
  - Предпочитайте стрелочные функции
  - Используйте eslint и prettier с нашими настройками (см. в корне репозитория [NodejsStarterKit](https://github.com/HowProgrammingWorks/NodejsStarterKit))
  - Предпочтительно использовать `for..of`, реже `Array/map`, реже `for` по переменной, избегайте `for..in` и `forEach`
  - Используйте промежуточные идентификаторы разделяя длинные выражения
  - Предпочитайте `const`, реже используйте `let`, но никогда не используйте `var`
  - Преобразуйте все магические значения в константы
  - Придерживайтесь правил именования идентификаторов
  - Хорошо подумайте над именами идентификаторов, чтобы при прочтении кода всем было понятно их содержимое
  - Не делайте слишком длинных функций
  - Не делайте большую стопку if-выражений, вместо этого используйте массивы и объекты
  - Важно не переписать с нуля, а именно пошагово улучшать

👉 Индекс других курсов: https://github.com/HowProgrammingWorks/Index
