<h1 id="5/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Restrict the unknown [function](../../../../../../function-split.md) to the $n$ possibilities $f^{(i)}(x)=1$ if $x_i=1$, and $2$ otherwise. Each has exactly one [essential variable](../../../../../../essential-variable-of-a-function.md), even if the allowed alphabet has more than two values. Every oracle answer in this restricted family is one [bit](../../../../../../bit.md).

A correct adaptive deterministic [algorithm](../../../../../../algorithm-split.md) must distinguish all $n$ possibilities. A binary [decision tree](../../../../../../decision-tree.md) of depth $q$ has at most $2^q$ leaves, so $2^q\ge n$. Therefore **$q\ge\lceil\log_2n\rceil=\Omega(\log n)$**. Restricting the answer family is essential to the argument: unrestricted integer-valued answers need not have binary branching. Combined with part ii, this gives optimal logarithmic [query complexity](../../../../../../query-complexity.md) for fixed $d$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
