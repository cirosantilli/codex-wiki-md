<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [0-1 knapsack problem](../../../../../0-1-knapsack-problem.md), item $j$ has weight $w_j$ and value $v_j$. Choose a [subset](../../../../../subset.md) of the $n$ items, using each at most once, whose total weight is at most $W$ and whose total value is as large as possible. For the capacity-indexed [dynamic program](../../../../../dynamic-program.md), take $W$ and the weights to be nonnegative [integers](../../../../../integer-split.md). The empty choice is allowed.

Let $K[j,c]$ be the greatest value attainable using only items $1,\ldots,j$ with capacity $c$. The base case is $K[0,c]=0$. With item $j$ unavailable when it is too heavy, the recurrence is

$$
\boxed{K[j,c]=
\begin{cases}
K[j-1,c],&w_j>c,\\
\max\{K[j-1,c],\ v_j+K[j-1,c-w_j]\},&w_j\leq c.
\end{cases}}
$$

Every feasible optimum either excludes item $j$, giving the first candidate, or includes it exactly once, leaving capacity $c-w_j$ for earlier items. The [principle of optimality](../../../../../principle-of-optimality.md) proves that the remaining earlier items must attain the indicated residual optimum. Conversely, either candidate constructs a feasible solution, so taking the larger is both necessary and sufficient. [Mathematical induction](../../../../../mathematical-induction.md) on $j$ proves the table's meaning and the final answer $\boxed{K[n,W]}$.

Store item weights and values in [arrays](../../../../../array-data-structure.md) and the values in a two-dimensional [array](../../../../../array-data-structure.md) with $(n+1)(W+1)$ entries. Fill rows in increasing $j$; each entry uses at most two values from the previous row. There are $n(W+1)$ constant-work updates, giving

$$
\boxed{\text{time}=\Theta(n(W+1)),\qquad\text{table space}=\Theta((n+1)(W+1)).}
$$

For positive growing capacities this is the familiar $\Theta(nW)$ bound. The $+1$ terms also cover capacity zero and zero-weight items: one must not initialize every $K[j,0]$ to zero if zero-weight, positive-value items are allowed.

To recover an actual [subset](../../../../../subset.md), store the chosen alternative at each entry or compare the two candidates while tracing backward from $(n,W)$. A selected item changes $(j,c)$ to $(j-1,c-w_j)$; an excluded item changes it to $(j-1,c)$. This takes $O(n)$ extra time.

If only the optimal value is needed, keep two rows, using $\Theta(W+1)$ space. With strictly positive weights, a single capacity row updated in decreasing capacity also prevents item reuse. The two-row version handles zero weights without special in-place reasoning. The running time is [pseudopolynomial](../../../../../pseudopolynomial-time.md), since the binary input length of $W$ is only logarithmic in its numerical value.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
