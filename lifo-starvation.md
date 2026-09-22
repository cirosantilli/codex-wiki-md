# LIFO starvation

↑ **Parent:** [Starvation freedom](starvation-freedom.md)

With a [LIFO stack](stack-data-structure.md) of waiting requests, an old request may remain at the bottom while a new request arrives before each completion and is served next. Every service can finish in finite time while the old request waits forever. A [FIFO queue](fifo-queue.md) prevents this overtaking within one priority class. [Nonpreemptive strict-priority arbitration](nonpreemptive-strict-priority-arbitration.md) can separately starve a lower-priority class; using a [LIFO stack](stack-data-structure.md) adds potential starvation even among requests of equal priority.

## ↑ Ancestors (8)

1. [Starvation freedom](starvation-freedom.md)
2. [Liveness property](liveness-property.md)
3. [Synchronization (computing)](synchronization-computing.md)
4. [Thread (computing)](thread-computing.md)
5. [Process (computing)](process-computing.md)
6. [Operating system](operating-system-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/2/c/solution.md)
