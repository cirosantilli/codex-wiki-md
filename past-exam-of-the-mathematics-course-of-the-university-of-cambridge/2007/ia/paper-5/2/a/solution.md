<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [working set](../../../../../../working-set.md) $W(t,\Delta)$ is the set of virtual pages referenced by an [operating-system process](../../../../../../process-computing.md) within a recent window of $\Delta$ execution time or memory references. Its size estimates the number of frames needed for the process's current locality of execution. It is a set of recently used pages, not the entirety of the process's address space.

An [operating system](../../../../../../operating-system.md) can estimate it from reference bits or fault history and try to keep those pages resident. [Process scheduling](../../../../../../process-scheduling.md) and admission control should avoid simultaneously running processes whose combined working sets exceed physical memory; suspending some processes or reducing multiprogramming then allows the rest to make useful progress. If too many active pages compete for too few frames, repeated [page faults](../../../../../../page-fault.md) produce [memory thrashing](../../../../../../thrashing-computer-science.md). **Working sets connect memory allocation to the choice of processes allowed to run.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
