# Lost wake-up

↑ **Parent:** [Synchronization (computing)](synchronization-computing.md)

A [lost wake-up](lost-wake-up.md) occurs when a notification arrives after a worker checks for work but before it safely starts waiting, so the worker sleeps despite available work. Avoid it by coupling the condition check with the wait protocol, or by using a persistent notification that is checked atomically with entering sleep. A queue test followed by an unrelated sleep instruction is insufficient.

## ↑ Ancestors (6)

1. [Synchronization (computing)](synchronization-computing.md)
2. [Thread (computing)](thread-computing.md)
3. [Process (computing)](process-computing.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Lost wake-up](lost-wake-up.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/concurrent-programming/3/b/i/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/concurrent-programming/3/b/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
