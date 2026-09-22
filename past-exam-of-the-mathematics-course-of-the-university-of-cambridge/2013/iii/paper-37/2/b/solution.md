<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When link delays are separable and nondecreasing, [Wardrop equilibria](../../../../../../wardrop-equilibrium.md) minimize the [Beckmann potential](../../../../../../beckmann-potential.md)

$$
\boxed{V(h)=\sum_j\int_0^{(Ah)_j}\ell_j(u)\,du}
$$

over the feasible route-flow polytope. Its [derivative](../../../../../../derivative.md) with respect to $h_r$ is $c_r(h)$. Since the [integrals](../../../../../../integral.md) are convex, the first-order inequality for a global minimum is exactly the [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) inequality in part (a). Alternatively, the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) equate used-route [derivatives](../../../../../../derivative.md) to the multiplier for their demand constraint, with larger [derivatives](../../../../../../derivative.md) on unused routes. Continuity gives existence on the compact feasible set. Strictly increasing link delays give unique link flows, although different route decompositions can still give [route-flow nonuniqueness at a Wardrop equilibrium](../../../../../../route-flow-nonuniqueness-at-a-wardrop-equilibrium.md).

The system objective is instead total travel time,

$$
T(y)=\sum_j y_j\ell_j(y_j).
$$

For differentiable delays its marginal cost is $\ell_j(y_j)+y_j\ell_j'(y_j)$, not simply $\ell_j(y_j)$. Thus an equilibrium optimizing the Beckmann potential generally fails to minimize total delay. A [marginal external cost toll](../../../../../../marginal-external-cost-toll.md) $y_j\ell_j'(y_j)$ makes travelers face the social marginal cost and implements a system optimum under the appropriate convexity assumptions.

These formulations clarify the modeling distinction: nonatomic users optimize their own paths; a planner optimizes total delay. For nonseparable or nonmonotone costs, the variational description can remain applicable while the [Beckmann potential](../../../../../../beckmann-potential.md) argument, existence or uniqueness needs new hypotheses.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
