<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $x$ and minimize $J_x(y)=f(y)+\|y-x\|^2/(2\tau)$. A proper lower semicontinuous [convex function](../../../../../../convex-function.md) has an [affine minorant](../../../../../../affine-minorant.md) $f(y)\geq a\cdot y+b$, as follows by separating a point below its closed [epigraph](../../../../../../epigraph.md). Hence

$$
J_x(y)\geq a\cdot y+b+\frac1{2\tau}\|y-x\|^2\longrightarrow+\infty
\quad\text{as }\|y\|\to\infty.
$$

The quadratic dominates the linear term, proving [coercivity](../../../../../../coercive-function.md). Properness supplies at least one finite trial value, [lower semicontinuity](../../../../../../lower-semicontinuity.md) passes to limits, and finite-dimensional compactness makes a bounded minimizing sequence converge along a subsequence to a minimizer. Thus the [proximal operator](../../../../../../proximal-operator.md) exists at every $x$.

The [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md) applies because the quadratic is finite and continuous everywhere. The [Fermat rule for convex minimization](../../../../../../fermat-rule-for-convex-minimization.md) gives

$$
0\in\partial J_x(y)=\partial f(y)+\frac{y-x}{\tau}
\quad\Longleftrightarrow\quad x\in y+\tau\partial f(y).
$$

Thus the minimizer lies in $B_{\tau f}(x)$. The uniqueness proved in part (a), or strict [convexity](../../../../../../convex-function.md) of the quadratic sum, now yields

$$
\boxed{B_{\tau f}(x)=\left\{\operatorname{prox}_{\tau f}(x)\right\}\quad
\text{for every }x\in\mathbb R^n.}
$$

This proof displays the separate roles of properness, [lower semicontinuity](../../../../../../lower-semicontinuity.md), [convexity](../../../../../../convex-function.md) and finite dimension. In particular, compactness here is not inferred merely from strict [convexity](../../../../../../convex-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
