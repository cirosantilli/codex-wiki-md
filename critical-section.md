# Critical section

↑ **Parent:** [Mutual exclusion](mutual-exclusion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_section)

A region whose accesses must obey a shared [synchronization](synchronization-computing.md) protocol. For the [lost update](lost-update.md) in [mutual exclusion](mutual-exclusion.md), the [critical section](critical-section.md) includes the read and the local addition as well as the write. Choosing its boundary means identifying the complete operation whose intermediate state must be protected. Every conflicting access must participate in a compatible protocol; merely declaring a [mutex](mutex.md) does not protect accesses that bypass it.

## ↑ Ancestors (7)

1. [Mutual exclusion](mutual-exclusion.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Critical section](critical-section.md)
- [Liveness property](liveness-property.md)
- [Lost update](lost-update.md)
- [Mutex](mutex.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Safety property](safety-property.md)
