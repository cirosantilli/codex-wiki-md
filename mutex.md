# Mutex

↑ **Parent:** [Mutual exclusion](mutual-exclusion.md)

An object with acquire and release operations that provides exclusive ownership to a participating [software thread](thread-computing.md). Several source-code regions can acquire the same [mutex](mutex.md); two different [mutex](mutex.md) objects do not exclude each other's users. The caller should enter its [critical section](critical-section.md) only after successful acquisition and release ownership on every exit path. A [mutex](mutex.md) may make a waiting [software thread](thread-computing.md) sleep or use a [spinlock](spinlock.md); the interface and the waiting mechanism are distinct.[Locks](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/locks.md)

**Table of contents**

- [Spinlock](spinlock.md)
  - [Test-and-set](test-and-set.md)

## ↑ Ancestors (7)

1. [Mutual exclusion](mutual-exclusion.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Critical section](critical-section.md)
- [Deadlock](deadlock.md)
- [Happens-before](happens-before.md)
- [Lock ordering](lock-ordering.md)
- [Mutex](mutex.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Pinned buffer](pinned-buffer.md)
- [Starvation freedom](starvation-freedom.md)
- [Thread interleaving](thread-interleaving.md)
- [xv6 buffer cache](xv6-buffer-cache.md)
