<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [interrupt handler](../../../../../interrupt-handler.md) is the only writer of `interval_ms`, `valid` and `next_slot`. The foreground function takes an [interrupt-safe ring-buffer snapshot](../../../../../interrupt-safe-ring-buffer-snapshot.md) inside a short [critical section](../../../../../critical-section.md), copying the count and exactly that many valid entries before restoring the previous mask. It performs the comparatively expensive summation and division after interrupts are restored. A new pulse then affects the next query, while the current query consistently describes the earlier snapshot.

Without exclusion, the foreground could read an old entry, be interrupted while the buffer is updated, then read new entries or an inconsistent count. Even indivisible 32-bit loads would not make that multi-element snapshot atomic. The [volatile-qualified objects in C](../../../../../volatile-qualified-objects-in-c.md) ensure that the compiler performs required shared or device accesses; `volatile` **does not provide mutual exclusion or a coherent multiword snapshot**.[Sections 5.1.2.3 and 6.7.3, observable volatile accesses and type qualifiers](../../../../../c11-committee-draft-n1570.md)

This design assumes a single-core foreground/interrupt execution model: no other interrupt, DMA engine or core modifies the protected buffer. The mask hooks must prevent compiler reordering across their boundaries and really mask the GPIO interrupt. Restoring the saved mask also makes the function safe to call when interrupts were already disabled. Keep the [critical section](../../../../../critical-section.md) short enough that the event register does not coalesce multiple heartbeats while interrupts are masked; otherwise the hardware interface cannot reconstruct events it never recorded.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
