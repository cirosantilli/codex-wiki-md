# Safety property

↑ **Parent:** [Synchronization (computing)](synchronization-computing.md)

A requirement whose violation has a finite execution prefix that no continuation can repair. Two [software threads](thread-computing.md) simultaneously inside a protected [critical section](critical-section.md) already violate [mutual exclusion](mutual-exclusion.md); later leaving does not erase that violation. This contrasts with a [liveness property](liveness-property.md), for which a long finite wait alone does not establish failure.[pp. 181–182: finite irremediable prefixes](defining-liveness-by-bowen-alpern-and-others.md)

## ↑ Ancestors (6)

1. [Synchronization (computing)](synchronization-computing.md)
2. [Thread (computing)](thread-computing.md)
3. [Process (computing)](process-computing.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Deadlock freedom](deadlock-freedom.md)
- [Mutual exclusion](mutual-exclusion.md)
