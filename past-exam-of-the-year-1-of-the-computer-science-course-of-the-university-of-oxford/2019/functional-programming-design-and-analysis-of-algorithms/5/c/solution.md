<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume ascending [sorted arrays](../../../../../sorted-array.md); descending storage can be accessed in reverse index order without copying. Among $2n$ entries, the requested rank is **$k=n+1$ in ascending order**, not $n$. Repeated values occupy repeated ranks.

Choose $i$ entries from the first [array](../../../../../array-data-structure.md) and $j=k-i$ from the second, using their prefixes. The feasible range is $\max(0,k-n)\le i\le\min(n,k)$. Write $A_L=A[i]$, $A_R=A[i+1]$, and similarly $B_L,B_R$ at $j$, with missing left endpoints replaced by $-\infty$ and missing right endpoints by $+\infty$. These are conceptual sentinels, not extra stored entries.

Use [binary search](../../../../../binary-search.md) over the feasible values of $i$:

- If $A_L>B_R$, there are too many entries from $A$ on the left; decrease the upper bound to $i-1$.
- If $B_L>A_R$, there are too few entries from $A$ on the left; increase the lower bound to $i+1$.
- Otherwise return **$\max(A_L,B_L)$**.

For correctness, in the last case every left entry is no greater than every right entry, and exactly $k$ entries lie on the left. Their [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) is therefore the $k$-th smallest entry. The failed inequalities are monotone in the searched index: increasing $i$ raises the $A$ boundary and decreases the $B$ boundary, so it cannot repair $A_L>B_R$; the other case is symmetric. A partition of the first $k$ entries of a merged ordering supplies an admissible solution, including ties. Each step halves an interval with at most $n+1$ choices, giving **$O(\log(n+1))$ [running time](../../../../../running-time.md) and $O(1)$ [auxiliary space](../../../../../auxiliary-space.md)**. This is a [two-sorted-array order statistic](../../../../../two-sorted-array-order-statistic.md) without constructing the merged [array](../../../../../array-data-structure.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
