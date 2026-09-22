<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the usual finite binary encoding of integer or rational input data. **[NP](../../../../../np-complexity.md)** consists of [decision problems](../../../../../decision-problem.md) whose yes-instances have polynomial-length [certificates in computational complexity](../../../../../certificate-complexity.md) verifiable in [polynomial time](../../../../../polynomial-time.md). A [decision problem](../../../../../decision-problem.md) is **[NP-hard](../../../../../np-hardness.md)** if every problem in [NP](../../../../../np-complexity.md) has a [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) to it. It is **[NP-complete](../../../../../np-completeness.md)** if it is both [NP-hard](../../../../../np-hardness.md) and in [NP](../../../../../np-complexity.md). An optimization problem is [NP-hard](../../../../../np-hardness.md) when computing its optimum would solve every [NP](../../../../../np-complexity.md) decision problem through a polynomial-time reduction and an optimum-value query; membership in [NP](../../../../../np-complexity.md) applies directly to decision problems, not to an unqualified optimization task.

Reduce [subset sum](../../../../../subset-sum-problem.md) to the [0-1 knapsack problem](../../../../../0-1-knapsack-problem.md) by setting $v_i=w_i=s_i$ and $B=t$. Every feasible value is at most $t$, and **the optimum equals $t$ exactly when the [subset sum](../../../../../subset-sum-problem.md) answer is yes**. The transformation and final comparison take [polynomial time](../../../../../polynomial-time.md). Since [subset sum](../../../../../subset-sum-problem.md) is assumed [NP-complete](../../../../../np-completeness.md), exact [knapsack optimization](../../../../../0-1-knapsack-problem.md) is [NP-hard](../../../../../np-hardness.md).

For the **[half-approximation algorithm for knapsack](../../../../../half-approximation-algorithm-for-knapsack.md)**, use nonnegative weights and profits. Delete overweight items and nonpositive-profit items; take all positive-profit zero-weight items for free. On the remaining positive-weight items, sort decreasing $v_i/w_i$. Take the maximal initial prefix fitting the capacity, and stop at the first item that would overflow. Let $G$ be the prefix profit, and let $M$ be the largest profit of any individually feasible remaining item. Return the better of the prefix and that singleton, together with the free items. If every item fits, take them all.

The [fractional knapsack problem](../../../../../fractional-knapsack-problem.md) fills exactly that prefix and a fraction $\alpha\in[0,1)$ of the first excluded item. Its optimum bounds the integer optimum, and without the free items its value is at most $G+\alpha v_{\mathrm{next}}\leq G+M$. Thus

$$
\boxed{\max(G,M)\geq\tfrac12(G+M)\geq\tfrac12\mathrm{OPT}.}
$$

With total free profit $F$, the same inequality is $F+\max(G,M)\geq\frac12(F+G+M)$. This gives an [approximation ratio](../../../../../approximation-ratio.md) of $1/2$ in $O(n\log n)$ sorting time, with polynomial bit complexity for rational data. Nonnegative weights and capacity are the standard [knapsack problem](../../../../../knapsack-problem.md) assumptions; unrestricted negative weights would not support this argument.

For the [quadratic knapsack problem](../../../../../quadratic-knapsack-problem.md) and its [fractional row bound for quadratic knapsack](../../../../../fractional-row-bound-for-quadratic-knapsack.md), multiply the capacity inequality by the binary $x_i$ and use $x_i^2=x_i$:

$$
\boxed{\sum_{j\ne i}x_ix_jw_j=x_i\sum_jx_jw_j-w_ix_i^2\leq(B-w_i)x_i.}
$$

Remove items with $w_i>B$ first. If $x_i=1$, the remaining coordinates $x_j$ are feasible in the fractional problem defining $q_i$, so $\sum_{j\ne i}p_{ij}x_j\leq q_i$. If $x_i=0$, that row's contribution is zero. Hence, with $c_i=v_i+q_i$,

$$
\boxed{\sum_i v_ix_i+\sum_i\sum_{j\ne i}p_{ij}x_ix_j\leq\sum_i c_ix_i.}
$$

The double sum counts each symmetric interaction twice; there is no factor $1/2$ in this problem. Each $q_i$ is a [fractional knapsack problem](../../../../../fractional-knapsack-problem.md), computable by sorting positive $p_{ij}/w_j$ ratios, also handling zero weights separately. This takes [polynomial time](../../../../../polynomial-time.md) even when some interactions are negative, because an optional fractional item with negative profit is omitted.

The resulting [0-1 knapsack problem](../../../../../0-1-knapsack-problem.md) need not be solved exactly. Relax its capacity constraint with a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda\geq0$. Its **[Lagrangian knapsack bound](../../../../../lagrangian-knapsack-bound.md)** is

$$
\boxed{U(\lambda)=\lambda B+\sum_i\max(0,c_i-\lambda w_i),\qquad \mathrm{OPT}_{\mathrm{QKP}}\leq\min_{\lambda\geq0}U(\lambda).}
$$

For feasible $x$, adding $\lambda(B-\sum_iw_ix_i)$ only increases its objective, and maximizing over independent binary choices produces the displayed expression. It is a convex piecewise-linear function with breakpoints at positive $c_i/w_i$. Evaluate those breakpoints and zero, or use the [fractional knapsack problem](../../../../../fractional-knapsack-problem.md) ordering; the best bound is computable in [polynomial time](../../../../../polynomial-time.md). Thus computing all $q_i$ and one additional [Lagrangian relaxation](../../../../../lagrangian-relaxation.md) gives the requested upper bound.

For the numerical example, the $q_1$ problem has capacity $3$ and item ratios $10/2=5$ and $12/3=4$. Select $y_2=1$ and $y_3=1/3$. This gives

$$
\boxed{q_1=10+\frac13\,12=14.}
$$

An exchange argument justifies optimality: capacity used on the lower-ratio item can be transferred to the higher-ratio item until the latter is full. The stated $q_2=20$ and $q_3=15$ similarly follow from residual capacities $2$ and $1$. Therefore $c=(24,40,30)$, with ratios $24,20,10$. The fractional solution takes items $1,2$ and one-third of item $3$, yielding $74$. At $\lambda=10$ the [Lagrangian knapsack bound](../../../../../lagrangian-knapsack-bound.md) gives the same value:

$$
\boxed{\mathrm{OPT}_{\mathrm{QKP}}\leq U(10)=40+14+20+0=74.}
$$

The fractional solution attaining $74$ proves that this is the best bound from this auxiliary [Lagrangian relaxation](../../../../../lagrangian-relaxation.md), though it need not be the exact quadratic optimum.

For [branch and bound](../../../../../branch-and-bound.md), branch on whether an unresolved $x_i$ is zero or one. If the selected set is $S$, subtract its weight from the residual capacity and retain its exact objective as a constant. For each remaining item replace $v_i$ by $v_i+2\sum_{j\in S}p_{ij}$, preserving the original interactions between remaining items. Recompute the fractional row bounds and the [Lagrangian knapsack bound](../../../../../lagrangian-knapsack-bound.md) for that residual problem. Maintain an incumbent from genuine feasible binary solutions evaluated with the quadratic objective; prune infeasible nodes and nodes whose bound is no better than the incumbent. For example, selecting items $1,2$ gives the feasible value $50$. A finite binary branching tree eventually certifies the optimum, but worst-case running time is exponential, as expected for an [NP-hard](../../../../../np-hardness.md) problem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 212](../../paper-212-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
