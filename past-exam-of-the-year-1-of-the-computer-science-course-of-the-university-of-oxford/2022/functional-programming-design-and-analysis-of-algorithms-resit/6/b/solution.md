<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Capacity alone cannot say which items have already been used. For the [0-1 knapsack problem](../../../../../0-1-knapsack-problem.md), let $D(i,c)$ use only the first $i$ items, each at most once. Then

$$
\boxed{D(0,c)=0,\qquad D(i,c)=\begin{cases}
D(i-1,c),&w_i>c,\\
\max\{D(i-1,c),\ v_i+D(i-1,c-w_i)\},&w_i\le c.
\end{cases}}
$$

The two alternatives omit item $i$ or take it. In the latter case its remaining companions must solve the smaller problem using the first $i-1$ items; otherwise replacing them would improve the whole selection. Both branches reduce the item index, so taking item $i$ cannot take it again. This establishes the [recurrence relation](../../../../../recurrence-relation.md) and [optimal substructure](../../../../../optimal-substructure.md).

Fill rows in increasing $i$ and return $D(n,W)$. There are $O(nW)$ entries with constant work each. Store the decisions for reconstruction; value-only computation uses $O(W)$ space by keeping two rows, or by scanning capacities downwards in a single row. A forward scan in a single row would instead allow repetitions. Nonnegative integral weights suffice for this version, including zero-weight items, because the item index always decreases.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
