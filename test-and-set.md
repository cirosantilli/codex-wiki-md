# Test-and-set

↑ **Parent:** [Spinlock](spinlock.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Test-and-set)

An [atomic read-modify-write](atomic-read-modify-write.md) that returns a flag's old value while setting it. In a [sequential consistency](sequential-consistency.md) model with the flag initially $0$, `exchange(flag, 1)` permits entry only when it returns $0$; an owner resets the flag to $0$ on release. Between releases only one exchange can observe $0$. By contrast, separate `read(flag)` and `write(flag, 1)` steps allow both contenders to read $0$ before either writes $1$. The indivisibility of the exchange is an assumed primitive, not something proved by writing its steps as ordinary assignments.[Locks](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/locks.md)

## ↑ Ancestors (9)

1. [Spinlock](spinlock.md)
2. [Mutex](mutex.md)
3. [Mutual exclusion](mutual-exclusion.md)
4. [Synchronization (computing)](synchronization-computing.md)
5. [Thread (computing)](thread-computing.md)
6. [Process (computing)](process-computing.md)
7. [Operating system](operating-system.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Acquire-release synchronization](acquire-release-synchronization.md)
- [Atomic read-modify-write](atomic-read-modify-write.md)
- [Spinlock](spinlock.md)
