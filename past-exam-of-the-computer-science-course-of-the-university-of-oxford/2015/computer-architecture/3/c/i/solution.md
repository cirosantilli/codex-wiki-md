<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With O1, even readers must acquire and release the same [mutex](../../../../../../mutex.md). Acquiring it normally uses an [atomic read-modify-write](../../../../../../atomic-read-modify-write.md) on the lock's [cache line](../../../../../../cache-line.md); releasing writes that [cache line](../../../../../../cache-line.md) again. As different [CPU cores](../../../../../../cpu-core.md) repeatedly read the data, ownership of the lock's [cache line](../../../../../../cache-line.md) moves among them, causing [cache coherence](../../../../../../cache-coherence.md) traffic and serializing the protected operations. If the lock shares a [cache line](../../../../../../cache-line.md) with otherwise stable data, [false sharing](../../../../../../false-sharing.md) can also invalidate useful reader data. The actual data need not change for this lock traffic to occur.

With O2 and correctly ordered publication, readers perform only [load instructions](../../../../../../load-instruction.md): copy `p` once into a [processor register](../../../../../../processor-register.md), then read that version of the data. Multiple [CPU cores](../../../../../../cpu-core.md) can keep read-only shared copies of its [cache lines](../../../../../../cache-line.md). No per-reader exclusive ownership transfer is needed. During an update, a writer fills newly allocated [computer memory](../../../../../../computer-memory-split.md) privately; the old version's [cache lines](../../../../../../cache-line.md) remain unchanged for readers already using it. Publishing the new [pointer](../../../../../../pointer-computer-programming.md) writes `p` and invalidates cached copies of that pointer's [cache line](../../../../../../cache-line.md), but this occurs only on updates.

**For many reads and rare updates, O2 avoids lock-line contention and permits concurrent readers, so it can be substantially faster.** The costs are [heap allocation](../../../../../../heap-allocation.md), construction or copying of a whole replacement, first accesses to its newly populated [cache lines](../../../../../../cache-line.md), and deferred [memory reclamation](../../../../../../memory-reclamation.md). Frequent updates or very large replacements can reverse the comparison. O1 can modify a small field in place and may then save copying and [computer memory](../../../../../../computer-memory-split.md). These are workload-dependent comparisons, not a claim that removing every [mutex](../../../../../../mutex.md) always accelerates an operation.

$$
\boxed{\text{Read-mostly immutable versions avoid per-reader lock-line writes.}}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Computer architecture](../../../../computer-architecture-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
