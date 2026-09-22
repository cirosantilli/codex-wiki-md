# Head-of-line blocking

↑ **Parent:** [Message passing](message-passing.md)

Delay to otherwise serviceable work because a preceding operation cannot complete. A timer service using serial [synchronous message passing](synchronous-message-passing.md) can block on one unready subscriber before delivering notifications to other ready subscribers. Buffered delivery moves the issue to queue capacity and service rate rather than guaranteeing its absence.

## ↑ Ancestors (7)

1. [Message passing](message-passing.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Channel multiplexing](channel-multiplexing.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/concurrent-programming/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/3/b/solution.md)
