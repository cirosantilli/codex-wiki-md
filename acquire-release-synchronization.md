# Acquire-release synchronization

↑ **Parent:** [Happens-before](happens-before.md)

A release on an atomic object can synchronize with an acquire that reads the released value, establishing [happens-before](happens-before.md) for surrounding accesses. A [test-and-set](test-and-set.md) [spinlock](spinlock.md) needs suitable acquisition and release semantics for its guarded data; relaxed flag operations alone do not supply that relationship. This is a separate question from the flag's indivisibility.[pp. 1524–1525: relaxed ordering and release/acquire synchronization](working-draft-standard-for-programming-language-c-plus-plus-n4861.md)

## ↑ Ancestors (8)

1. [Happens-before](happens-before.md)
2. [Memory model](memory-model.md)
3. [Synchronization (computing)](synchronization-computing.md)
4. [Thread (computing)](thread-computing.md)
5. [Process (computing)](process-computing.md)
6. [Operating system](operating-system-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Atomic read-modify-write](atomic-read-modify-write.md)
- [Circular buffer operation costs](circular-buffer-operation-costs.md)
- [Mutual exclusion](mutual-exclusion.md)
