# Single-bit event latch

↑ **Parent:** [Interrupt](interrupt.md)

A [single-bit event latch](single-bit-event-latch.md) remembers whether at least one event has occurred since it was cleared. It does not count how many events occurred: histories with one and two unacknowledged events produce the same visible state. Therefore no software reading only that state can distinguish those histories. Exact counting needs a minimum rearming interval assumption or richer hardware, such as a counter or queue.

## ↑ Ancestors (4)

1. [Interrupt](interrupt.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Event counter](event-counter.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Single-bit event latch](single-bit-event-latch.md)
