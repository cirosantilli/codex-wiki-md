<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [uniform cover inequality](../../../../../../uniform-covers-theorem.md) states that for a positive-volume body $K\subset\mathbb R^n$ and a multiset $\mathcal A$ in which each coordinate occurs exactly $k$ times, $\boxed{|K|^k\leq\prod_{A\in\mathcal A}|K_A|}$, where $K_A$ is its coordinate projection and volumes use the corresponding dimensions.

To deduce the [box theorem](../../../../../../box-theorem.md), maximize $\sum_i x_i$ subject to $\sum_{i\in A}x_i\leq\log|K_A|$ for every nonempty $A\subseteq[n]$. This [linear program](../../../../../../linear-programming.md) is feasible and bounded above by the full-set constraint. Its dual minimizes $\sum_A\lambda_A\log|K_A|$ over nonnegative weights with $\sum_{A\ni i}\lambda_A=1$. For rational weights, clearing denominators gives an exact uniform cover, so the [uniform cover inequality](../../../../../../uniform-covers-theorem.md) bounds that dual objective below by $\log|K|$. The same holds for all feasible weights by density of rational points in the rational constraint polyhedron. [Strong duality](../../../../../../strong-duality.md) makes the primal optimum at least $\log|K|$, while the full-set constraint makes it at most that value. An optimal solution therefore gives $b_i=e^{x_i}>0$ with

$$
\boxed{\prod_i b_i=|K|,\qquad\prod_{i\in A}b_i\leq|K_A|\quad\text{for every }A.}
$$

The axis-aligned box with these side lengths has the required volume and projection volumes.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
