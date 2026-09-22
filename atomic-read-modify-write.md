# Atomic read-modify-write

↑ **Parent:** [Atomic operation](atomic-operation.md)

An [atomic operation](atomic-operation.md) that reads a shared object's value and changes it as one indivisible action. For an increment from $0$, the two operations under [mutual exclusion](mutual-exclusion.md) produce $1$ then $2$ in either [software thread](thread-computing.md) order. A [test-and-set](test-and-set.md) is another example. The operation's ordering guarantees for other data still depend on the [memory model](memory-model.md) and its selected [acquire-release synchronization](acquire-release-synchronization.md) semantics.

## ↑ Ancestors (7)

1. [Atomic operation](atomic-operation.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Lost update](lost-update.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Test-and-set](test-and-set.md)
- [Thread interleaving](thread-interleaving.md)
