<h1 id="3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On a real [Hilbert space](../../../../../../hilbert-space-split.md), for a proper lower-semicontinuous [convex function](../../../../../../convex-function.md) $E$, the [proximal operator](../../../../../../proximal-operator.md) is

$$
\boxed{\operatorname{prox}_E(q)=\arg\min_x\left\{E(x)+\frac12\|x-q\|^2\right\}.}
$$

The quadratic makes this objective [strongly convex](../../../../../../strongly-convex-function.md) and coercive; the affine lower bound available for a proper closed [convex function](../../../../../../convex-function.md) and [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md) give existence. The minimizer is unique. The [subdifferential](../../../../../../subdifferential.md) optimality condition is

$$
\boxed{q-x\in\partial E(x),\qquad x=\operatorname{prox}_E(q).}
$$

For a positive parameter $t$, $\operatorname{prox}_{tE}$ uses $tE(x)$ in the same formula. On a general [Banach space](../../../../../../banach-space-split.md), the analogous norm-squared minimization is [Banach-space proximal minimization](../../../../../../banach-space-proximal-minimization.md); it can be set-valued and the identity-valued Hilbert derivative must be replaced by the [duality mapping](../../../../../../duality-mapping.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
