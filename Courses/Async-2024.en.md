# Asynchronous programming 2024

The methods of writing asynchronous code that we used 10-15 years ago are irretrievably a thing of the past and can be interesting only to support the legacy exercise in a deep understanding of asynchronous programming. Even the methods of 5-7 years ago already have little in common with modern practices, but the Internet is full of outdated information, even [Metarhia community open course](https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Asynchronous.md ) has become too bulky and redundant at the moment. It should also be mentioned that asynchronous programming should look fundamentally different in system and application code. It will not be possible to completely hide the complexity of asynchronous code behind abstractions from the product developer, because it will in any case work with timers, events, streams, fetch and other asynchronous APIs, but it can be written dozens of times easier than asynchronous code in a system layer. As for the system layer, it is necessary to introduce the theory of queues (systems of mass service), the model of actors, some abstractions from parallel programming (semaphores, rendezvous, atomic operations). Of course, it is difficult to contain all this in one course, therefore, we will give priority to the application code and first fully prepare the course for the use of asynchronous programming in product development, and then we will add optional topics of the old course and many other useful abstractions widely used in other programming languages, but little known in the world of JavaScript.

## Content

Important aspects of the new course:

- Concentration on practical application (code examples from real projects)
- Relevance and compliance with standards of 2023-2024
- Tasks and analysis of the solutions, seminars, code review (the course is not just video)
- Recommendations for choosing the style and abstractions of asynchrony for the task
- Attention to correct error handling in all styles of asynchrony
- Emphasis on reliability, maintainability, testability, reduction of coupling
- Examples and tasks for correcting hidden problem states and data races

Topics of the new course:

- Asynchrony contracts based on callback: callback-last, error-first
- Minimum required understanding of runtime: event loop, I/O, timers
- Asynchrony contracts based on events: EventEmitter, Streams
- Promise/then/catch/finally contract and async/await syntax
- Parallel and serial execution, all/any/race/allSettled
- Contract converters, code docking in different styles
- Prevention of race conditions of data and control in asynchronous code
- Cancellation of asynchronous operations: AbortController, AbortSignal
- Error processing, their detection and possible problems with the stacktrace
- Asynchronous collection (we collect values until ready)

## Pay attention

What you need to know and be able to do to start:

- [JavaScript syntax, but possible without any tricks](https://github.com/HowProgrammingWorks/Index/blob/master/Courses/Fundamentals.md)
- Confidently know git, have a github account
- Preferably docker, have a working machine on linux or mac
- Any development environment, IDE or editor

What this course is not: it is not reading documentation, not a course on libraries and frameworks, not a repetition of an old course, not live coding and not a master class, not a stream. The new course is the most concentrated information and practical tasks for both applied and system programming with a comparison of these approaches.

## How to get to the course

- News will be in the channel: https://t.me/asyncify
- Course group: https://t.me/asynctalks