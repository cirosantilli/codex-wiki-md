<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume a [proper lazy list](../../../../../proper-lazy-list.md) with defined elements and terminating [equality tests](../../../../../equality-test.md). If infinitely many distinct values occur, [first-occurrence duplicate removal](../../../../../first-occurrence-duplicate-removal.md) produces an infinite [list](../../../../../list-abstract-data-type.md) of distinct values, in first-occurrence order. To produce the next new value after $k$ have appeared, the nested [list filters](../../../../../list-filter.md) need skip only a finite input prefix: an infinite collection of distinct values cannot all belong to the $k$ already seen. The next new value therefore occurs at a finite position and is reached in finite work. Consequently

$$
\boxed{\text{infinitely many distinct values}\ \Longrightarrow\ \text{productive infinite output}.}
$$

This is a [stream productivity](../../../../../stream-productivity.md) claim, not a bounded-delay claim: arbitrarily long runs of repetitions can make successive delays arbitrarily large. Undefined elements or diverging [equality tests](../../../../../equality-test.md) invalidate the stated assumptions.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
