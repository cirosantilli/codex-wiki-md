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

## ← Incoming links (14)

- [Critical section](critical-section.md)
- [Event counter](event-counter.md)
- [Interrupt-driven pulse sequencer](interrupt-driven-pulse-sequencer.md)
- [Interrupt-safe ring-buffer snapshot](interrupt-safe-ring-buffer-snapshot.md)
- [Liveness property](liveness-property.md)
- [Lost update](lost-update.md)
- [Mutex](mutex.md)
- [Mutual exclusion](mutual-exclusion.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/b/solution.md)
- [Safety property](safety-property.md)
- [Volatile-qualified objects in C](volatile-qualified-objects-in-c.md)
