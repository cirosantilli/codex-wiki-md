<h1 id="5/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**`start == null` if and only if `end == null`.** Otherwise there is a finite list of distinct [software objects](../../../../../../software-object.md) $v_0,\ldots,v_{m-1}$, with `start eq v0`, `end eq v(m-1)`, `v0.left == null`, and `v(m-1).right == null`. For every valid adjacent pair, `v(i).right eq v(i+1)` and `v(i+1).left eq v(i)`. These are exactly the entries reachable through the list links, so there is no extra cycle or branch. All counts are positive, all words are non-null, and words strictly increase from `start` to `end`.

This is the [representation invariant](../../../../../../representation-invariant.md) for a null-terminated [doubly linked list](../../../../../../doubly-linked-list.md) without a [list header](../../../../../../list-header.md). The [abstraction function](../../../../../../abstraction-function.md) reads the ordered word-count pairs from left to right. Conversion additionally requires the output entries, counts and words to be precisely those of the input [binary search tree](../../../../../../binary-search-tree.md); that preservation property is an operation [postcondition](../../../../../../postcondition.md), rather than an invariant of an arbitrary list by itself.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [5](../../../5.md)
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
