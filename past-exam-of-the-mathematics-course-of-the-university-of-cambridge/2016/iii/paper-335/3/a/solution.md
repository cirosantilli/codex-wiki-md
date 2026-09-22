<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) replaces the possibly unbounded inverse by a family of continuous reconstruction operators $R_\alpha:Y\to X$. For compatible exact data it must recover the minimum-norm solution $x^\dagger\in(\ker A)^\perp$ as $\alpha\downarrow0$. For noisy data $\|y^\delta-y\|\leq\delta$, a parameter rule $\alpha=\alpha(\delta)$ must make both bias and amplified noise tend to zero. The target is the minimum-norm solution because data cannot determine a component in the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md).

[Tikhonov regularization](../../../../../../tikhonov-regularization.md) minimizes

$$
J_\alpha(x)=\|Ax-y^\delta\|_Y^2+\alpha\|x\|_X^2,\qquad \alpha>0.
$$

The [quadratic norm penalty](../../../../../../quadratic-norm-penalty.md) makes this [functional](../../../../../../functional.md) [strictly convex](../../../../../../strictly-convex-function.md) and a [coercive function](../../../../../../coercive-function.md). Its first variation, applied to arbitrary real and imaginary perturbations, gives

$$
(A^*A+\alpha I)x_\alpha^\delta=A^*y^\delta.
$$

The [positive operator](../../../../../../positive-operator.md) $A^*A+\alpha I$ is bounded below by $\alpha I$ and has a bounded inverse. **The unique [Tikhonov regularization](../../../../../../tikhonov-regularization.md) solution is**

$$
\boxed{x_\alpha^\delta=R_\alpha y^\delta,\qquad
R_\alpha=(A^*A+\alpha I)^{-1}A^*.}
$$

The [Tikhonov stability bound](../../../../../../tikhonov-stability-bound.md) follows from the singular-value gain:

$$
\|R_\alpha\|\leq\sup_{\sigma\geq0}\frac{\sigma}{\sigma^2+\alpha}
=\frac1{2\sqrt\alpha},\qquad
\boxed{\|x_\alpha^\delta-x_\alpha\|\leq\frac{\delta}{2\sqrt\alpha}.}
$$

Thus reconstruction is stable for each fixed positive $\alpha$. Stability is not uniform as $\alpha\downarrow0$: that limit restores the unbounded inverse. For exact compatible data,

$$
x_\alpha-x^\dagger=-\alpha(A^*A+\alpha I)^{-1}x^\dagger\longrightarrow0.
$$

The [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md) makes this strong convergence transparent: each positive singular-value coefficient tends to zero and is bounded by the corresponding coefficient of $x^\dagger$. Consequently

$$
\|x_\alpha^\delta-x^\dagger\|
\leq\|x_\alpha-x^\dagger\|+\frac{\delta}{2\sqrt\alpha}\longrightarrow0
$$

whenever $\alpha(\delta)\downarrow0$ and $\delta/\sqrt{\alpha(\delta)}\to0$, for example $\alpha(\delta)=\delta$. This is a convergent [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md), not merely a bounded formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
