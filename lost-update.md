# Lost update

↑ **Parent:** [Thread interleaving](thread-interleaving.md)

A change that is overwritten by another update based on an older value. In [mutual exclusion](mutual-exclusion.md), both [software threads](thread-computing.md) read $0$ and later write $1$, so one intended increment is lost. This [race condition](race-condition.md) can occur with individually atomic reads and writes and therefore need not involve a [data race](data-race.md). Its repair must cover the complete update, using a [critical section](critical-section.md) or an appropriate [atomic read-modify-write](atomic-read-modify-write.md).

## ↑ Ancestors (8)

1. [Thread interleaving](thread-interleaving.md)
2. [Mutual exclusion](mutual-exclusion.md)
3. [Synchronization (computing)](synchronization-computing.md)
4. [Thread (computing)](thread-computing.md)
5. [Process (computing)](process-computing.md)
6. [Operating system](operating-system-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Critical section](critical-section.md)
- [Data race](data-race.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Sequential consistency](sequential-consistency.md)
