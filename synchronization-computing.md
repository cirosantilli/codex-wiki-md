# Synchronization (computing)

↑ **Parent:** [Thread (computing)](thread-computing.md)

Coordinating concurrent activities so that required ordering and visibility rules hold. [Mutual exclusion](mutual-exclusion.md) is one form of [synchronization](synchronization-computing.md); waiting for another [software thread](thread-computing.md) to finish is another.

**Table of contents**

- [Mutual exclusion](mutual-exclusion.md)
  - [Critical section](critical-section.md)
  - [Mutex](mutex.md)
    - [Spinlock](spinlock.md)
      - [Test-and-set](test-and-set.md)
  - [Thread interleaving](thread-interleaving.md)
    - [Lost update](lost-update.md)
- [Safety property](safety-property.md)
- [Liveness property](liveness-property.md)
  - [Starvation freedom](starvation-freedom.md)
- [Deadlock](deadlock.md)
  - [Deadlock freedom](deadlock-freedom.md)
  - [Lock ordering](lock-ordering.md)
- [Memory model](memory-model.md)
  - [Sequential consistency](sequential-consistency.md)
  - [Data race](data-race.md)
  - [Happens-before](happens-before.md)
    - [Acquire-release synchronization](acquire-release-synchronization.md)
- [Atomic operation](atomic-operation.md)
  - [Atomic read-modify-write](atomic-read-modify-write.md)

## ↑ Ancestors (5)

1. [Thread (computing)](thread-computing.md)
2. [Process (computing)](process-computing.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Buffer cache key](buffer-cache-key.md)
- [File-system crash consistency](file-system-crash-consistency.md)
- [Shared file mapping](shared-file-mapping.md)
- [xv6 buffer cache](xv6-buffer-cache.md)
