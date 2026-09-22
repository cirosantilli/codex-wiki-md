<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Version snapshots simplify correctness: a complicated command restores the complete prior state, so a bespoke inverse cannot accidentally omit an auxiliary field. Redo restores the recorded result without re-executing behavior that might depend on time, randomness or external input. Restoring an immutable root takes [constant time](../../../../../../constant-time.md), though refreshing the display can cost more.

The storage comparison depends on the representation. A change-specific record for these elementary edits retains only a few indices and song references. Copying a length-$m$ [array](../../../../../../array-data-structure.md) for each of $h$ edits can require $\Theta(hm)$ storage and $\Theta(m)$ copying per edit. A [persistent data structure](../../../../../../persistent-data-structure.md) with [structural sharing](../../../../../../structural-sharing.md) can preserve many versions much more cheaply; balanced path copying can make small edits allocate $O(\log m)$ new entries. Retaining versions also keeps their reachable data alive. Snapshot references are only constant-sized roots, not a guarantee of constant total retained memory. Neither scheme automatically reverses external effects such as playing audio or writing files. The desired undo boundary must be specified.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
