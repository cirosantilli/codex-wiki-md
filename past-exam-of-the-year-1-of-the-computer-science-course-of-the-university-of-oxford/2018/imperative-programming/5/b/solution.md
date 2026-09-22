<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [representation invariant](../../../../../representation-invariant.md) says that `root` is either `null` or the root of a finite, acyclic [binary search tree](../../../../../binary-search-tree.md), with no [software object](../../../../../software-object.md) shared between different child [subtrees](../../../../../subtree.md). Every reachable entry has a non-null word and a strictly positive frequency. For each entry $t$, **every word in its entire left [subtree](../../../../../subtree.md) is strictly less than `t.word`, and every word in its entire right [subtree](../../../../../subtree.md) is strictly greater**. This is an inherited ordering condition on all descendants, rather than merely a comparison with immediate children. It implies that each distinct word has exactly one entry. The empty initial state satisfies it.

The [abstraction function](../../../../../abstraction-function.md) is the finite [multiset](../../../../../multiset.md) assigning each stored word its positive count and assigning all other words zero. Frequencies and their increments must fit in `Int`; the implementation below explicitly rejects an increment at its representational limit instead of silently violating positivity through [integer overflow](../../../../../integer-overflow.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
