<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For finite, defined [lists](../../../../../list-abstract-data-type.md), [structural induction](../../../../../structural-induction.md) requires $P([])$ and $P(xs)\Rightarrow P(x:xs)$ for every head $x$ and tail $xs$. This proves $P$ for every finite [list](../../../../../list-abstract-data-type.md).

An infinite [list](../../../../../list-abstract-data-type.md) cannot be reached by finitely many constructor steps. For [structural induction on lazy lists](../../../../../structural-induction-on-lazy-lists.md), also check $P(\bot)$, where $\bot$ is the [bottom value](../../../../../bottom-value.md), and require an [admissible predicate on lazy lists](../../../../../admissible-predicate-on-lazy-lists.md): if increasingly defined finite approximations all satisfy $P$, their limit does too. Together with the empty-list and constructor cases this covers finite, partial and infinite [lists](../../../../../list-abstract-data-type.md). Merely asserting the two finite-list cases is insufficient; “the list is finite” itself satisfies those cases but fails on infinite lists.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
