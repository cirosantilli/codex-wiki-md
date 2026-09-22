<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [two-bag 0-1 knapsack problem](../../../../../two-bag-0-1-knapsack-problem.md), let $D[j,a,b]$ be the maximum total value using the first $j$ items, with remaining capacity limits $a$ in the first bag and $b$ in the second. Initialize $D[0,a,b]=0$. Item $j$ has exactly three possible decisions: omit it, place it in bag one if it fits, or place it in bag two if it fits. Hence

$$
\boxed{D[j,a,b]=\max\!\left(
\{D[j-1,a,b]\}
\cup\{v_j+D[j-1,a-w_j,b]:w_j\leq a\}
\cup\{v_j+D[j-1,a,b-w_j]:w_j\leq b\}
\right).}
$$

A braced candidate with a false condition is omitted. All candidates refer to layer $j-1$, which prevents the same item from entering both bags. Combining two independently optimized single-bag [knapsacks](../../../../../knapsack-problem.md) would not enforce that restriction.

The [principle of optimality](../../../../../principle-of-optimality.md) proves correctness exactly as in part (b): condition on the location of the final item and replace the earlier items by the optimal feasible residual assignment. Every candidate is realizable, and every feasible assignment belongs to one of the three cases. The final answer is $\boxed{D[n,W_1,W_2]}$.

Fill the three-dimensional [array](../../../../../array-data-structure.md) in increasing item index. Each of its $n(W_1+1)(W_2+1)$ updates inspects at most three candidates:

$$
\boxed{\text{time}=\Theta(n(W_1+1)(W_2+1)),\quad\text{full space}=\Theta((n+1)(W_1+1)(W_2+1)).}
$$

For positive capacities the customary expression is $\Theta(nW_1W_2)$. Keeping only two item layers reduces space to $\Theta((W_1+1)(W_2+1))$ for the optimal value. Full decision storage also permits backward reconstruction of each item's bag assignment. Nonnegative [integer](../../../../../integer-split.md) weights and capacities are the assumptions behind this capacity-indexed [dynamic programming](../../../../../dynamic-programming.md) table.

## ↑ Ancestors (12)

1. [C](../c.md)
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
