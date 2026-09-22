# Memory model

↑ **Parent:** [Synchronization (computing)](synchronization-computing.md)

Rules specifying which shared-data observations and operation orders are allowed. [Sequential consistency](sequential-consistency.md) is the model used in the two diagrams. A language [memory model](memory-model.md) can permit weaker ordering and impose additional conditions on conflicting accesses. Correct use of an indivisible flag must therefore be checked against that [memory model](memory-model.md), including [happens-before](happens-before.md) relationships for the data guarded by the flag.

**Table of contents**

- [Control dependency](control-dependency.md)
- [Address dependency](address-dependency.md)
- [Total store order](total-store-order.md)
- [Memory barrier](memory-barrier.md)
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

## ← Incoming links (11)

- [Atomic read-modify-write](atomic-read-modify-write.md)
- [Circular buffer operation costs](circular-buffer-operation-costs.md)
- [Control dependency](control-dependency.md)
- [Happens-before](happens-before.md)
- [Memory model](memory-model.md)
- [Multicore processor](multicore-processor.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-architecture/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-architecture/3/c/iii/solution.md)
- [Thread interleaving](thread-interleaving.md)
- [Total store order](total-store-order.md)
- [Understanding POWER Multiprocessors (2011)](understanding-power-multiprocessors-2011.md)
