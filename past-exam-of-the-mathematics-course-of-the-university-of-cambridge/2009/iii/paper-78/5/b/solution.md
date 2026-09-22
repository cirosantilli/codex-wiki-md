<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\alpha>0$, [Tikhonov regularization](../../../../../../tikhonov-regularization.md) minimizes the strictly convex quadratic

$$
J_\alpha(v)=\|Av-y_\delta\|^2+\alpha\|v\|^2.
$$

Differentiating in every direction gives the [Tikhonov normal equation](../../../../../../tikhonov-normal-equation.md) $(A^TA+\alpha I)v=A^Ty_\delta$. Symmetry of $A$ therefore gives

$$
\boxed{x_\alpha^\delta=R_\alpha y_\delta,\qquad R_\alpha=(A^2+\alpha I)^{-1}A,\qquad
x_\alpha^\delta=\sum_i\frac{\lambda_i}{\lambda_i^2+\alpha}(y_\delta,u_i)u_i.}
$$

The [spectral filter](../../../../../../spectral-filter.md) suppresses unstable division by small [eigenvalues](../../../../../../eigenvalue.md). Put $e_i=(y_\delta-y,u_i)$ and $x_i=(x,u_i)$. The exact [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md) is

$$
\boxed{x_\alpha^\delta-x=\sum_i\left[\frac{\lambda_i e_i}{\lambda_i^2+\alpha}-\frac{\alpha x_i}{\lambda_i^2+\alpha}\right]u_i.}
$$

By orthonormality and the [triangle inequality](../../../../../../triangle-inequality.md),

$$
\|x_\alpha^\delta-x\|\leq\delta\max_i\frac{\lambda_i}{\lambda_i^2+\alpha}
+\frac{\alpha}{\lambda_1^2+\alpha}\|x\|.
$$

The scalar gain satisfies $\lambda/(\lambda^2+\alpha)\leq1/(2\sqrt\alpha)$, because $(\lambda-\sqrt\alpha)^2\geq0$. Hence the [Tikhonov stability bound](../../../../../../tikhonov-stability-bound.md) gives

$$
\boxed{\|x_\alpha^\delta-x\|\leq\frac{\delta}{2\sqrt\alpha}+\frac{\alpha}{\lambda_1^2}\|x\|.}
$$

This explicitly separates data noise from regularization bias. For a known bound $X\geq\|x\|>0$, minimizing this last bound gives an [a priori regularization parameter choice](../../../../../../a-priori-regularization-parameter-choice.md)

$$
\alpha=\left(\frac{\delta\lambda_1^2}{4X}\right)^{2/3},\qquad
\boxed{\|x_\alpha^\delta-x\|\leq\frac{3}{4^{2/3}}\left(\frac X{\lambda_1^2}\right)^{1/3}\delta^{2/3}.}
$$

One data-based bound is $X=(\|y_\delta\|+\delta)/\lambda_1$. More generally, $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$ make the robust estimate converge to zero.

For this fixed finite matrix, the sharper gain bound $\max_i\lambda_i/(\lambda_i^2+\alpha)\leq1/\lambda_1$ is also available. Thus the $\delta^{2/3}$ rate is a consequence of the robust bound, not an optimality claim: choosing $\alpha X/\lambda_1^2\leq C\delta/\lambda_1$ gives an $O(\delta/\lambda_1)$ estimate. No unique statistically optimal parameter is specified without further assumptions on the signal or noise.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
