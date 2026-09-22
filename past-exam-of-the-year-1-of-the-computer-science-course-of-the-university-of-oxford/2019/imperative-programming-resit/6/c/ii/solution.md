<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Not necessarily: [structural sharing](../../../../../../structural-sharing.md) can make snapshots cheap, but the trait alone gives no storage guarantee.** With a [persistent data structure](../../../../../../persistent-data-structure.md), unchanged portions of old and new [sequences](../../../../../../sequence.md) can be shared safely. Saving two root references costs $O(1)$ additional space per edit, and adjacent history entries commonly refer to the same intermediate version. With an appropriate balanced persistent [tree](../../../../../../tree-graph-theory-split.md), each positional edit may add only $O(\log n)$ new [vertices](../../../../../../vertex-graph-theory.md), giving approximately $O(n+h\log n)$ storage for $h$ retained edits of comparable presentation size, plus references to slides.

There are important qualifications. A fully copied immutable [array](../../../../../../array-data-structure.md) may allocate $\Theta(n)$ per edit and use $\Theta(hn)$ across its history. A persistent [linked list](../../../../../../linked-list.md) shares suffixes but may copy a long prefix for a late positional edit. Moreover, snapshot history keeps old versions alive that an edit-specific inverse representation might otherwise release. Consequently a significant increase is possible with some implementations or workloads; it is not forced by saving `Sequence` references, and it cannot be ruled out from the interface alone.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Imperative programming resit](../../../../imperative-programming-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
