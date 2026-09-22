# Lock ordering

↑ **Parent:** [Deadlock](deadlock.md)

A shared order governing acquisition of distinct [mutex](mutex.md) objects. To prevent circular waiting, choose a strict [total order](total-order.md) and acquire only a higher-ranked [mutex](mutex.md) while retaining lower-ranked ones. In the two-object [deadlock](deadlock.md) example, every participant acquires A before B. An outline of the argument is that ranks would strictly increase around any alleged waiting cycle, yet return to the starting rank, a contradiction. The rule must include acquisitions hidden inside called routines. It excludes this kind of [deadlock](deadlock.md), not arbitrary waiting on other resources or failure to schedule an owner.[pp. 7–8: consistent acquisition ordering and hidden calls](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/common-concurrency-problems.md)

## ↑ Ancestors (7)

1. [Deadlock](deadlock.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Deadlock](deadlock.md)
