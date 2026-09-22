# Spinlock

↑ **Parent:** [Mutex](mutex.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spinlock)

A mechanism that waits for ownership by repeatedly trying while consuming [CPU](central-processing-unit.md) execution time. A [spinlock](spinlock.md) built from [test-and-set](test-and-set.md) can enforce [mutual exclusion](mutual-exclusion.md) without guaranteeing [starvation freedom](starvation-freedom.md). Progress also requires the owner to run and release: if a waiting [software thread](thread-computing.md) monopolizes the only [CPU](central-processing-unit.md) while the owner is suspended, exclusive entry alone cannot help.[pp. 8–9: preemption requirement and lack of fairness guarantees](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/locks.md)

**Table of contents**

- [Test-and-set](test-and-set.md)

## ↑ Ancestors (8)

1. [Mutex](mutex.md)
2. [Mutual exclusion](mutual-exclusion.md)
3. [Synchronization (computing)](synchronization-computing.md)
4. [Thread (computing)](thread-computing.md)
5. [Process (computing)](process-computing.md)
6. [Operating system](operating-system-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Acquire-release synchronization](acquire-release-synchronization.md)
- [Mutex](mutex.md)
- [Spinlock](spinlock.md)
- [xv6 buffer cache](xv6-buffer-cache.md)
