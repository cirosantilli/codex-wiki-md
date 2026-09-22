# Thread interleaving

↑ **Parent:** [Mutual exclusion](mutual-exclusion.md)

An ordered execution obtained by mixing steps of several [software threads](thread-computing.md) while retaining each one's own step order. In the [sequential consistency](sequential-consistency.md) model of [mutual exclusion](mutual-exclusion.md), an indivisible step finishes before the next begins. Selecting the step boundaries is part of the model: an [atomic read-modify-write](atomic-read-modify-write.md) increment has one boundary, whereas a separate read, local addition and write have three. Enumerating all such orders checks this specified model, not an arbitrary [memory model](memory-model.md) or a real [mutex](mutex.md) implementation.

**Table of contents**

- [Lost update](lost-update.md)

## ↑ Ancestors (7)

1. [Mutual exclusion](mutual-exclusion.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Liveness property](liveness-property.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Sequential consistency](sequential-consistency.md)
