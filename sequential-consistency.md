# Sequential consistency

↑ **Parent:** [Memory model](memory-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sequential_consistency)

Execution behaves as if steps occurred in one [total order](total-order.md) preserving each participant's program order; reads observe the latest preceding writes in that order. This is the definition given in the 1979 paper [How to Make a Multiprocessor Computer That Correctly Executes Multiprocess Programs](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/12/How-to-Make-a-Multiprocessor-Computer-That-Correctly-Executes-Multiprocess-Programs.pdf), printed p. 690. It permits many [thread interleavings](thread-interleaving.md), including the [lost update](lost-update.md) under [mutual exclusion](mutual-exclusion.md); ordering individual accesses does not combine them into one [atomic operation](atomic-operation.md).

## ↑ Ancestors (7)

1. [Memory model](memory-model.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Deadlock](deadlock.md)
- [Memory model](memory-model.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Test-and-set](test-and-set.md)
- [Thread interleaving](thread-interleaving.md)
