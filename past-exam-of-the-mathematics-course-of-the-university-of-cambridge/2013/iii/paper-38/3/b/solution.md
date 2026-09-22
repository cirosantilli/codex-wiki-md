<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [minimum-cost flow](../../../../../../minimum-cost-flow-problem.md) with bounds $0\leq x_{ij}\leq m_{ij}$, the [capacitated flow optimality conditions](../../../../../../capacitated-flow-optimality-conditions.md) consist of primal feasibility and [network dual potentials](../../../../../../network-dual-potential.md) whose [network reduced costs](../../../../../../network-reduced-cost.md) obey

$$
\boxed{\begin{cases}
r_{ij}\geq0,&x_{ij}=0,\\
r_{ij}=0,&0<x_{ij}<m_{ij},\\
r_{ij}\leq0,&x_{ij}=m_{ij}.
\end{cases}}
$$

For a zero-capacity edge both bounds coincide and no sign restriction is needed; all capacities here are positive. These are the bound form of [complementary slackness](../../../../../../complementary-slackness.md). To derive necessity directly, construct the [residual network](../../../../../../residual-network.md): a possible increase has original cost $c_{ij}$ and a possible decrease has reverse cost $-c_{ij}$. An optimal flow cannot admit a negative-cost [directed cycle](../../../../../../directed-cycle.md), since a positive step around it preserves [flow balance](../../../../../../flow-balance.md) and lowers cost. If there is no such cycle, connect a new source by zero-cost edges to every vertex and let $d_i$ be shortest-path distances. They exist because no negative cycle is reachable. For every residual edge $i\to j$, $d_j\leq d_i+c_{ij}^{\rm res}$. Taking $\pi_i=-d_i$ makes every residual [network reduced cost](../../../../../../network-reduced-cost.md) nonnegative, exactly the displayed sign conditions: both directions exist for an interior edge.

Conversely, for any other feasible flow $y$, equal [flow balances](../../../../../../flow-balance.md) give

$$
\sum_{ij}c_{ij}(y_{ij}-x_{ij})
=\sum_{ij}r_{ij}(y_{ij}-x_{ij}).
$$

Each summand is nonnegative at a lower or upper bound, and zero at an interior edge. Hence the sign conditions suffice for optimality as well.

For the final flow, use $\pi=(0,-7,-10,-11,-12)$ in the order $(S,A,B,C,T)$. All four tree edges have zero [network reduced cost](../../../../../../network-reduced-cost.md), while $SB,AB,BC$ have costs $-4,2,1$. More explicitly, every feasible flow satisfies

$$
\sum_{ij}c_{ij}y_{ij}
=\sum_i\pi_i b_i+\sum_{ij}r_{ij}y_{ij}
=300-4y_{SB}+2y_{AB}+y_{BC}\geq300-4(20)=220.
$$

Our flow attains equality. **This gives a direct cost certificate of 220.** The strict signs also force $y_{SB}=20$, $y_{AB}=y_{BC}=0$ at any optimum; [flow balance](../../../../../../flow-balance.md) then fixes all remaining edges, so this flow is unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
