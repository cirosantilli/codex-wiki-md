<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Three distinct [concatenation tree](../../../../../concatenation-tree.md) representations of the empty [list](../../../../../list-abstract-data-type.md) are `Nil`, `Cat Nil Nil`, and `Cat (Cat Nil Nil) Nil`. For the singleton `[x]`, use `One x`, `Cat Nil (One x)`, and `Cat (One x) Nil`.

An empty branch changes the [data structure](../../../../../data-structure-split.md) without changing its denoted [list](../../../../../list-abstract-data-type.md). Repeating this padding gives arbitrarily many representations of the same [list](../../../../../list-abstract-data-type.md); there is no uniqueness invariant in the stated datatype.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
