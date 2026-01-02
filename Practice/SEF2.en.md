# Practice and projects

## Possible options of work organization:

- Contribution to any open-source project or library.
- Contribution to [Metarhia](https://github.com/metarhia).
- A student group project or an open source community project.
- Personal open-source project.

## What is allowed and what is prohibited:

- You can use any language and all the libraries built into it.
- You cannot use third-party libraries installed from npm, GitHub, etc.
- The repository must be posted on https://github.com in the public domain.
- It is necessary to develop group work skills, for this students form groups
2-5 people each; the group can write one common project or make a cross-review of code of individual projects of each group member. Rewatch:
  - [What is a code review](https://youtu.be/EKL6NiIQ6ZU)
  - [Seminar on code review](https://youtu.be/AgH4OAKbmkM)
- A project cannot be immediately uploaded to Github the day before delivery; it needs to be maintained on Github for several months so that the work, commit history and PR (pull request) are visible. It will be good if it is possible to track the improvement of the code base, refactoring and optimization. Rewatch:
  - Ganeral [antipatterns for all paradigms](https://youtu.be/NMUsUiFokr4), и
  - Antipatterns of [procedural programming](https://youtu.be/cTv7V22mkwE);
  - Lecture on [refactoring](https://youtu.be/z73wmpdweQ4).
- Good repository management: issues, pull requests, milestones (see the buttons on the issues and pr tabs in github), discussions (optional), kanban (a project planning tool, look for the project tab in github), wiki (optional).
- Every project should have unit tests to check functionality.
- The repository should include:
  - License and list of contributors
  - File `README.md` with a brief (1-2 pages) description of the project. No folders, no paperwork needed, everything is done electronically, without bureaucracy.
  - Customized linter (and if the code is in JavaScript, also prettier). Project example
  with configuration here: https://github.com/HowProgrammingWorks/NodejsStarterKit
  - The `package.json` file in which in the `scripts` section there is a `lint` command
  - `.eslintrc.json`, `.eslintignore` and `.prettierrc` files
  - Before each commit, run from the command line: `npm run lint`
  (some problems are automatically corrected, the rest are corrected manually).
  - Dotfiles for version control system and package manager.

## Topic examples:

- Library for working with IPv4 and IPv6 addresses: parser, comparison, manipulation, working with masks and ranges, serialization as strings and numbers, any other operations that you come up with.
- Parser for HTML, CSS, JSON, YAML or any other file format.
- Develop a universal class for caching: calculations, operations
I/O, database queries, or other operations that need to be accelerated
with caching (optional). Containing a configurable cache with the following
characteristics: a certain size of the number of records or memory capacity,
cache eviction time, eviction priorities.
- Implement machine checking for correct syntax and code style. There could be a separate topic on correcting simple syntax errors. And one more topic on auto-formatting code and bringing it to style conventions.
- An improved EventEmitter, for example, with the following features: one-time and N-time subscription, automatic unsubscription after a timeout or sending a special event, waiting for events using async/await syntax, etc.
- Projection of data structures in memory. You can create a special syntax (projection language), which has already been done in JavaScript in the repository
https://github.com/HowProgrammingWorks/Projection
- Develop a simple key-value in-memory DBMS (database management system that stores everything in RAM). In the simplest case, it is a hash table. Example implementations are Redis, Memcached or MongoDB, you can take their interfaces as a basis and modify them.
- Develop a task scheduler in the form of a class or prototype that can repeat the execution of a method according to a schedule, for example: on Fridays at 2 am or every second Monday of the month at 12:30 UTC. It creates the necessary timers for this and executes the tasks.
- Command line interface utilities.

## Register topics

- Fill in the form: https://forms.gle/u7v7nUFxamcgJ2aQ6
- And give me rights to the repository, my account: https://github.com/tshemsedinov
