<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For nonnegative [integer](../../../../../../integer-split.md) amount $v$, let $M[t]$ be the minimum number of coins making amount $t$. Set $M[0]=0$ and compute, in increasing order of $t$,

$$
M[t]=1+\min_{i:x_i\le t} M[t-x_i],\qquad 1\le t\le v.
$$

An empty candidate [set](../../../../../../set-split.md) has [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md) $\infty$. Here denomination $1$ ensures that every nonnegative amount is attainable. Removing one coin from an optimal nonempty solution gives a smaller amount, and adding any allowed last coin gives a feasible solution; these two directions prove the recurrence by [induction](../../../../../../mathematical-induction.md) on $t$.

Return **whether $M[v]\le k$**. This solves the at-most-$k$ decision without needing a separate dimension for $k$. The table for the [minimum coin change recurrence](../../../../../../minimum-coin-change-recurrence.md) takes **$O(nv)$ [running time](../../../../../../running-time.md) and $O(v)$ [space complexity](../../../../../../space-complexity.md)**. The bound is [pseudopolynomial time](../../../../../../pseudopolynomial-time.md): the amount, rather than its binary encoding length, appears in it. Amount zero needs zero coins.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
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
