# Memory model

↑ **Parent:** [Synchronization (computing)](synchronization-computing.md)

Rules specifying which shared-data observations and operation orders are allowed. [Sequential consistency](sequential-consistency.md) is the model used in the two diagrams. A language [memory model](memory-model.md) can permit weaker ordering and impose additional conditions on conflicting accesses. Correct use of an indivisible flag must therefore be checked against that [memory model](memory-model.md), including [happens-before](happens-before.md) relationships for the data guarded by the flag.

**Table of contents**

- [Sequential consistency](sequential-consistency.md)
- [Data race](data-race.md)
- [Happens-before](happens-before.md)
  - [Acquire-release synchronization](acquire-release-synchronization.md)

## ↑ Ancestors (6)

1. [Synchronization (computing)](synchronization-computing.md)
2. [Thread (computing)](thread-computing.md)
3. [Process (computing)](process-computing.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Atomic read-modify-write](atomic-read-modify-write.md)
- [Circular buffer operation costs](circular-buffer-operation-costs.md)
- [Happens-before](happens-before.md)
- [Memory model](memory-model.md)
- [Thread interleaving](thread-interleaving.md)
