# Data race

↑ **Parent:** [Memory model](memory-model.md)

For the C++ case used here, conflicting accesses by different [software threads](thread-computing.md), at least one non-atomic, with neither ordered before the other by [happens-before](happens-before.md). Such a [data race](data-race.md) has undefined behavior. A [race condition](race-condition.md) is broader: the [lost update](lost-update.md) with separate atomic reads and writes depends on their order while avoiding a [data race](data-race.md).[pp. 79–80: conflicting actions and undefined behavior](working-draft-standard-for-programming-language-c-plus-plus-n4861.md)

## ↑ Ancestors (7)

1. [Memory model](memory-model.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Data race](data-race.md)
- [Lost update](lost-update.md)
- [Mutual exclusion](mutual-exclusion.md)
