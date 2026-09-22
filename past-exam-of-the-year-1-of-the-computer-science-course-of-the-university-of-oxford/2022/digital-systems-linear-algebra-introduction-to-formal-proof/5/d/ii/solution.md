<h1 id="5/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Evaluate the [recurrence relation](../../../../../../recurrence-relation.md) successively, retaining only the preceding two values. Each of the $n-1$ updates uses three [multiplications](../../../../../../multiplication.md) and one [subtraction](../../../../../../subtraction.md). Hence **$4(n-1)=O(n)$ [arithmetic operations](../../../../../../arithmetic-operation.md) and $O(1)$ auxiliary storage** suffice, excluding the stored input. Naively branching into two recursive calls would repeat work; the sequential computation is essential. This is an arithmetic-operation bound, not a bit-complexity bound for arbitrarily large exact [integers](../../../../../../integer-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
