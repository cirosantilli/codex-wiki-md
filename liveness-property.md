# Liveness property

↑ **Parent:** [Synchronization (computing)](synchronization-computing.md)

A requirement of eventual progress, with no finite prefix ruling out its eventual satisfaction. For [starvation freedom](starvation-freedom.md), a persistent requester must eventually enter its [critical section](critical-section.md). Establishing such a [liveness property](liveness-property.md) requires explicit scheduling and protocol assumptions in addition to [mutual exclusion](mutual-exclusion.md). Exhaustive finite [thread interleaving](thread-interleaving.md) checks alone do not establish eventual service for repeatedly competing [software threads](thread-computing.md).[p. 182: every finite prefix can still be extended to satisfy a liveness property](defining-liveness-by-bowen-alpern-and-others.md)

**Table of contents**

- [Starvation freedom](starvation-freedom.md)

## ↑ Ancestors (6)

1. [Synchronization (computing)](synchronization-computing.md)
2. [Thread (computing)](thread-computing.md)
3. [Process (computing)](process-computing.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Deadlock freedom](deadlock-freedom.md)
- [Liveness property](liveness-property.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Safety property](safety-property.md)
