<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take an [integer](../../../../../../integer-split.md) pivot $0\leq p\leq N+1$. There are $p$ possible values in $[0,p)$ but only $k$ occurrences of such values in the whole [array](../../../../../../array-data-structure.md). When $k<p$, the [pigeonhole principle](../../../../../../pigeonhole-principle.md) gives

$$
\boxed{\text{Some value in }[0,p)\text{ is missing.}}
$$

Repeated values do not invalidate the argument: they can only reduce the number of distinct values represented by those $k$ occurrences. The other side might also contain a missing value.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
