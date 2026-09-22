<h1 id="8/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Sort the two dimension vectors separately into ascending order, $a_1\le\cdots\le a_d$ and $b_1\le\cdots\le b_d$. Then return **true exactly when $a_i<b_i$ for every $i$**. Sorting costs $O(d\log d)$ and the coordinate comparisons cost $O(d)$.

Sufficiency follows by matching corresponding ranks and translating that rank matching back to the original axes. For necessity, suppose $a_k\ge b_k$ for some $k$. The $d-k+1$ dimensions $a_k,\ldots,a_d$ must all be assigned to strictly larger target dimensions. None of the first $k$ sorted target dimensions is large enough, leaving at most $d-k$ eligible slots. The [pigeonhole principle](../../../../../../pigeonhole-principle.md) gives a contradiction. This proves the [sorted-coordinate criterion for box containment](../../../../../../sorted-coordinate-criterion-for-box-containment.md), including ties: equality fails the required strict fit.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [8](../../../8.md)
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
