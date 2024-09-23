# 🚀 Patterns 2024 Тренінг із наставниками

***Rethinking GRASP, SOLID, and GoF for JavaScript and Node.js***

> Translations: [EN](./Patterns-2024.md), [UA](./Patterns-2024-ua.md), [RU](./Patterns-2024-ru.md)

Практичний тренінг з переосмислення та застосування патернів GoF, SOLID та GRASP в асинхронному програмуванні на JavaScript та Type для прикладних та системних розробників бекенду та фронтенду, з прикладами для Node.js та браузерних додатків.

***Наступний онбординг розпочнеться 1 жовтня 2024 року***

Розуміння цих концепцій не можна просто витягти з коробки (або книги) і помістити собі у голову. Таке розуміння сильно відрізняється для різних мов та платформ.
Сліпе перенесення знань і практик з C++ або Java в **JavaScript** та C# призводить до мертвих церемоній.
Однак їх можна відродити за допомогою практики, прив'язати до реалій та переосмислити, щоб вони не стали марними монстрами.

## 💡 Унікальність програми наставництва
  
Від автора першого курсу з асинхронного програмування на JavaScript, прочитаного в Київському політехнічному інституті ще 17 років тому, безліч доповідей та лекцій з Node.js. За ці роки зібрано багато досвіду, відгуків, практики, усі курси автора перероблялися практично щороку, вбираючи найновіші пактики. Тимур Шемсединов також є контриб'ютором багатьох платформ і бібліотек у відкритому коді, серед яких Node.js, Metarhia, geoip-lite, MDN, HowProgrammingWorks, metasync... Тимур один з перших, хто почав портувати в JavaScript абстракції паралельного програмування з C++, C#, Java, Go та інших мов.

Автор стверджує, що це найважливіші речі, які слід вивчати та практикувати:

* 📂 Системи модульності, Dependency Injection (DI) та інверсія управління (IoC)
* 📦 Декомпозиція абстракцій та принципи GRASP із сучасною інтерпретацією
* 🧩 Паттерни «Банди чотирьох» (GoF) переосмислені для JavaScript та TypeScript
* 🔮 Принципи ізоляції та SoC (Розподіл відповідальності)
* 👷🏻‍♂️ Відокремлення прикладного та системного коду (різні спеціальності)
* 🧩 Принципи SOLID: SRP, OCP, ISP, DIP, LSP з адаптацією для різних парадигм
* 🌟 Мультипарадигменне програмування та створення доменних мов (DSL)
* 🧩 Контрактне програмування та декларативне моделювання через схеми
* 🏛️ Чиста архітектура (Clean) та лукова архітектура (Onion або Layered)

## Тарифні плани

* Minimal: навчання у загальній групі без наставника, але з груповими семінарами
* Standard: навчання з наставником у невеликих групах (10 осіб)
* Professional: навчання з наставником, індивідуально та в групах, додаткові матеріали
* Exclusive: персоналізований навчальний трек з автором курсу та запрошеними експертами

## Формат тренінгу

- 🗓️ 12 тижнів (3 місяці) + онбординг (1 тиждень) + секретний модуль
- 👍 Доступ до матеріалів курсу надається назавжди
- 🕑 Щотижня обов'язково: 1 година лекцій + 2 години семінар + 2 години самостійної роботи
- 🥋 Тренування та групова робота з наставниками, а не тільки перегляд видосів та читання
- 🙋‍♂️ За бажанням: для глибокого занурення +3 години додаткових матеріалів на старших тарифах
- 🏅 По завершенню курсу Ви отримуєте сертифікат
- 💬 Робочі мови: руська - лекцій; українська, англійська, руська, турецька - семінари та наставники
- ⚠️ Вхідні вимоги: базовий JavaScript + рекомендується досвід практичного програмування
- 🙅 Для кого не підійде: не для початківців, безкоштовні матеріали для початківців шукайте у Тимура
- 💳 Розстрочка: помісячна оплата для всіх тарифів, окрім мінімального
- 🗺️ Після курсу участь у ком'юніті випускників, де вже тисячі людей по всьому світу

[👉 Придбати: https://nodeua.com/Patterns-2024-buy.html](https://nodeua.com/Patterns-2024-buy.html)

## 📖 Структура курсу

### 📦 Unit 1: Structure and Modularity

Структура та модульність. Чому потрібно переосмислити та адаптувати GoF, SOLID та GRASP для сучасного JavaScript/TypeScript. Як це зробити?

> Ми навчимося застосовувати патерни та принципи на практичних завданнях, які зустрічаються у типових проектах, а також проведемо паралелі між теорією з класичних книг та щоденною практикою, покажемо, що всі ці знання потрібні не лише на співбесідах, а й дозволяють покращити характеристики коду ваших проектів та розуміння між фахівцями у колективі.

Що ми отримуємо як результат цього юніту:

+ Починаємо писати код, який зручно покривати тестами.
+ Наш код стає кращим для читання та розуміння.
+ Після оптимізації наш повільний код стає швидше і їсть менше пам'яті.
+ Код стає модульним, надійним і готовим до інтеграції.
+ Як змінити код, щоб зменшити час, необхідний для його підтримки.

> Для кожного тижня підготовлені завдання, деякі з них передбачають рефакторинг готових прикладів коду, інші – написання коду, треті – оптимізацію та дослідження характеристик коду.

**🗓️ Week 1: Характеристики коду та стратегії оптимізації**

> Існує шлях, який веде до радикального покращення структури та характеристик коду. Ми розглянемо принципи та шаблони GoF, SOLID, GRASP, як їх застосовувати та що вони дають. Характеристики коду: читання, надійність, тестування, підтримуваність, повторне використання, гнучкість, безпека. Оптимальне використання обчислювальних ресурсів: процесор, пам'ять, введення-виведення та когнітивні ресурси розробників.

**🗓️ Week 2: Вбудовані можливості в мові та платформі**

> JavaScript має вбудовані контракти: Thenable, Iterable, AsyncIterator, Callback-last, Callable, Cancelable, Observable, але культура розробки через контракти та інтерфейси не дуже поширена у спільноті. Як покращити продуктивність розробки за допомогою підходу, що базується на знаннях. Як шаблони можуть допомогти нам у цьому: реалізовувати нові фічі швидко та ефективно, бути продуктивними, робити щоденну роботу цікавою, бути вмотивованими та не вигорати.

**🗓️ Week 3: Інстанціювання: шаблони та техніки створення екземплярів**

> Шаблони створення екземплярів: Constructor, Singleton, Factory, Pool, Builder, Prototype, Flyweight, інші шаблони і техніки. Давайте знайдемо пов'язані принципи та переосмислимо прикладне значення GRASP: Creator; GRASP: Polymorphism, SOLID: ISP; Aggregation і Composition. Як заощаджувати пам'ять та інші ресурси; як ефективно застосовувати оптимізацію та кешування. Як розробляти вкрай швидкий код та мінімізувати latency, зробити код крос-платформним та зрозумілим для колег.

**🗓️ Week 4: Ізоляція та розподіл відповідальності (SoC)**

> Separation of Concerns (SoC) — це загальний інженерний принцип, спрямований на створення гнучких, надійних систем, що легко модифікуються. Ми можемо використовувати шаблони GoF: Mediator, Bridge, Abstract factory, Strategy (в JavaScript реалізації: Map<PropertyKey, Implementation>); Системи модульності; GRASP принципи Information Expert, Indirection, та Protected variations; SOLID: SRP. Це покращить тестованість коду та знизить витрати на інтеграцію.

### 📦 Unit 2: Execution and Contracts

Для побудови структури програми з модулів та програмних компонентів, нам потрібен контрактний підхід до програмування, він дозволяє розробляти частини системи незалежно, масштабувати команду, покращувати керованість проектами та робити план розробки більш передбачуваним.

> Ми будемо застосовувати три типи зв'язування: зв'язування через дані, зв'язування через виклики та зв'язування через події. Ми навчимося керувати зачепленням між компонентами програмних систем та проектувати їх таким чином, щоб мати можливість динамічно збирати з них програми, відкладаючи рішення про компонування. Іншими словами, наше завдання на етапі проектування не прибити все цвяхами, а надати архітектору можливість пізнього маневру.

+ Навчимося створювати структуру коду.
+ Навчимося створювати структуру колективу, що відповідає структурі коду. (За законом Конвея: «організації проектують системи, які копіюють структуру комунікацій у цій організації»).
+ Відпрацьовуємо написання додатків, що добре підтримуються.

**🗓️ Week 5: Контракти: інтерфейси для взаємодії компонентів**

> Паттерни: Adapter (Wrapper), Facade, Bridge, Composite, Proxy, Promisify; Front controller; GRASP: Low Coupling and High Cohesion; SOLID: LSP (Liskov); та SOLID: OCP (Open-Closed). Застосування контрактів відкриває можливість покрокового рефакторингу, усунення технічного боргу та підвищення стабільності підсистем; зниження залежності (зв'язаності) між шарами та модулями. На рівні управління проектом це дозволяє масштабувати команду, керувати пріоритетами та приймати архітектурні рішення.

**🗓️ Week 6: Послаблення зачеплення в коді через події та повідомлення**

> Наступний потужний підхід - це застосування шин подій всередині програми та між підсистемами. Це поширене в інтерфейсах користувача, розподілених системах, спільному доступі до шарених ресурсів. На базі асинхронного програмування та програмування через потоки подій побудовано рішення з неблокуючим введенням-виводом в Node.js. Ми розглянемо GRASP: Pure Fabrication and Low Coupling; AsyncQueue and queueing systems, Async collections, та інші.

**🗓️ Week 7: Streams: Потоки даних та їх перетворення**

> Реактивне програмування розвинулося у окрему парадигму; потоки та сигнали засновані на GoF: Observer; GRASP: Pure Fabrication та Event-driven підході з потоками даних та операторами перетворення даних. Це широко використовується в мережевих протоколах, доступі до даних та файлових систем, розробки ігор, фінансових та аналітичних систем, управління вбудованими системами, телеметрії та інших областях. Це дає виразний синтаксис, більш високий рівень абстракції, гнучкість і продуктивність для поліпшення досвіду користувача (UX).

**🗓️ Week 8: Обробка помилок: Exceptions та Soft Failures**

> Ми розглянемо найкращі практики обробки помилок як із винятковими ситуаціями, так і доменними (м'якими) помилками. Gracefully recover та м'які помилки підвищать загальну продуктивність системи. Ми будемо використовувати Chain of Responsibility, SOLID, Promises, fallback mechanisms to handle non-critical errors; GRASP: Protected Variations and Custom JavaScript-specific AggregateError and Error.prototype.cause, а також серіалізацію помилок для передачі по мережі.

### 📦 Unit 3: Runtime for Applications

Об'єднання всіх розглянутих технік та підходів у реальних умовах. У цьому юніті ми розглянемо, як основні концепції побудови структури додатків, контрактне програмування та шаблони перетворюються на працюючі та масштабовані додатки.

> Цей модуль зосереджений у тому, як питання середовища виконання лягають завдання структури та архітектури додатків. Ви отримаєте навичку впровадження технік програмування, що перетворюють програмне рішення на цифрову платформу, розраховану на тривалу експлуатацію; це включає підтримку зміни інструментарію, розширення колективу, постійне інтенсивне нарощування функціональності та навантажень.

**🗓️ Week 9: Семантика: виразні DSL**

> Для покращення виразності коду та ясності семантики будь-яке складне програмне забезпечення потребує створення DSL (мов, спеціалізованих для предметної області). При розробці DSL можна використовувати добре відомі синтаксиси, такі як JSON, JSON5, Markdown і навіть JavaScript. Ми розглянемо патерни: Command, Interpreter, State, Strategy, Visitor. DSL робить код зрозумілим для аналітиків предметної області та навіть досвідчених користувачів. Це покращує спілкування та розуміння, прискорює розробку, адаптацію рішень до нових вимог, спрощує навчання та передачу знань, приховує технічні складності та дозволяє фахівцям зосередитися на своїй галузі, покращуючи загальну передбачуваність проекту.

**🗓️ Week 10: All-agnostic як стратегія за замовчуванням**

> Розробка систем, незалежних від фреймворків, платформ, протоколів, баз даних та хмарних рішень, як стандартний підхід для забезпечення гнучкості та свободи архітектурних рішень. Такий підхід усуває залежність від постачальників хмарних рішень та фреймворків. Звичайно, не потрібно реалізовувати всі аспекти агностичного підходу, але деякі з них принесуть значні вигоди в масштабуванні системи та в процесі її експлуатації. Ми будемо використовувати ізоляцію, GRASP: Controller; SOLID: DIP; принципи IoC та DI; інтерфейси та патерн Strategy для відв'язування від конкретних реалізацій.

**🗓️ Week 11: Масштабування додатків та архітектурні стилі**

> На цьому тижні ми розглянемо, як проектувати системи, які можуть масштабуватися та розвиватися ефективно, використовуючи різні архітектурні стилі: DDD, листкова архітектура, SOA, мікросервіс, подійна архітектура, монолітна, порти та адаптери, чиста архітектура, Event-Sourcing, CQRS, Pipeline , Peer-to-Peer, Client-Server архітектура та як застосовувати SOLID, GRASP та GoF для реалізації архітектури.

**🗓️ Week 12: Методологія: як почати застосовувати концепції**

> Заключна частина програми тренінгу зосереджена практичному застосуванні всіх знань у комплексі. Ми розглянемо, як почати впроваджувати концепції та шаблони, вивчені на курсі у реальних проектах. Цей модуль надає практичні стратегії для створення дорожньої карти щодо їх впровадження. Як виявити необхідність у шаблонах та принципах та врахувати можливі негативні аспекти. Рефакторинг успадкованих систем, впровадження нових методів розробки та активностей у колективі. Як спланувати власне навчання та налагодити розвиток команди з використанням знань із цього тренінгу.

## Тарифні плани

* Minimal: навчання у загальній групі без наставника, але з груповими семінарами
* Standard: навчання з наставником у невеликих групах (10 осіб)
* Professional: навчання з наставником, індивідуально та в групах, додаткові матеріали
* Exclusive: персоналізований навчальний трек з автором курсу та запрошеними експертами

[👉 Придбати: https://nodeua.com/Patterns-2024-buy.html](https://nodeua.com/Patterns-2024-buy.html)