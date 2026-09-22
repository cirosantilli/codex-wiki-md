# Happens-before

↑ **Parent:** [Memory model](memory-model.md)

An ordering [binary relation](binary-relation.md) used by a [memory model](memory-model.md) to constrain observation of shared data. For the [mutex](mutex.md) example, T1's write precedes its release, that release synchronizes with T2's successful acquisition, and that acquisition precedes T2's read. Together these steps order the write before the read. Wall-clock timing alone does not establish [happens-before](happens-before.md).[Working Draft, Standard for Programming Language C++ (N4861)](working-draft-standard-for-programming-language-c-plus-plus-n4861.md)

**Table of contents**

- [Acquire-release synchronization](acquire-release-synchronization.md)

## ↑ Ancestors (7)

1. [Memory model](memory-model.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Acquire-release synchronization](acquire-release-synchronization.md)
- [Data race](data-race.md)
- [Happens-before](happens-before.md)
- [Memory model](memory-model.md)
- [Mutual exclusion](mutual-exclusion.md)
