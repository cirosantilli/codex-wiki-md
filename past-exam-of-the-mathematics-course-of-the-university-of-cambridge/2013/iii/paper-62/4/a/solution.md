<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [forward subgradient step](../../../../../../forward-subgradient-step.md) and [backward subgradient step](../../../../../../proximal-operator.md) are the set-valued maps

$$
\boxed{
F_{\tau f}(x)=x-\tau\partial f(x)
=\{x-\tau p:p\in\partial f(x)\},\qquad
B_{\tau f}=(I+\tau\partial f)^{-1}.}
$$

Thus $u\in B_{\tau f}(z)$ means $z-u\in\tau\partial f(u)$. They are respectively the explicit and implicit time discretizations of [subgradient flow](../../../../../../subgradient-flow.md) $\dot x\in-\partial f(x)$. At a differentiable point the forward update is $x-\tau\nabla f(x)$, while the backward update evaluates the gradient at the new point. For proper closed convex data the latter is the [proximal operator](../../../../../../proximal-operator.md)

$$
B_{\tau f}(z)=\arg\min_u\left\{f(u)+\frac1{2\tau}\|u-z\|^2\right\}.
$$

To prove at most one output, suppose $u,v\in B_{\tau f}(z)$. Then $(z-u)/\tau\in\partial f(u)$ and $(z-v)/\tau\in\partial f(v)$. The two [subgradient inequalities](../../../../../../subgradient-inequality.md) imply [monotonicity of a convex subdifferential](../../../../../../monotonicity-of-a-convex-subdifferential.md), giving

$$
0\leq\left\langle\frac{z-u}{\tau}-\frac{z-v}{\tau},u-v\right\rangle
=-\frac{\|u-v\|^2}{\tau}.
$$

Since $\tau>0$, $u=v$. Convexity supplies this monotonicity; lower semicontinuity is not needed for this at-most-one argument.

Under the full printed assumptions the output actually exists at every $z$. Properness ensures a finite point and excludes $-\infty$. Proper lower-semicontinuous convex $f$ has an [affine minorant](../../../../../../affine-minorant.md), so the quadratic proximal objective is coercive. Lower semicontinuity makes its minimum attained on a compact sublevel set. Convexity and the positive quadratic curvature make it strongly convex, hence its minimizer is unique. The [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md), with the differentiable quadratic term, is exactly $z-u\in\tau\partial f(u)$. Thus

$$
\boxed{B_{\tau f}\text{ is everywhere defined and single-valued}.}
$$

This also identifies precisely which assumptions provide existence, uniqueness and the update's optimality interpretation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
