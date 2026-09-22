<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [cubic spline](../../../../../cubic-spline.md) belongs to $C^2[a,b]$ and is a [polynomial](../../../../../polynomial-split.md) of degree at most three on each interval separated by the [spline knots](../../../../../spline-knot.md). A [natural cubic spline](../../../../../natural-cubic-spline.md) is additionally an [affine function](../../../../../affine-function.md) on the exterior intervals $[a,x_1]$ and $[x_n,b]$. On $[x_1,x_n]$ this is equivalent to the endpoint conditions $s''(x_1)=s''(x_n)=0$; these conditions remain part of the definition when an outer knot coincides with $a$ or $b$.

Let $s$ be the [natural cubic spline interpolant](../../../../../natural-cubic-spline-interpolant.md) of the prescribed values, and let $v$ be any other interpolating $C^2$ function. Set $u=v-s$, so $u(x_i)=0$. On the interval $[x_i,x_{i+1}]$, [integration by parts](../../../../../integration-by-parts.md) twice gives

$$
\int_{x_i}^{x_{i+1}}s''u''=[s''u']_{x_i}^{x_{i+1}}-[s'''u]_{x_i}^{x_{i+1}},
$$

because the fourth [derivative](../../../../../derivative.md) of each cubic piece is zero. The second boundary term is zero because $u$ vanishes at the [spline knots](../../../../../spline-knot.md). After summing the first terms, the interior contributions cancel by [continuity](../../../../../continuous-function.md) of $s''$ and $u'$, and the two remaining terms vanish by the natural endpoint conditions. On the exterior intervals $s''=0$. Thus $\int_a^b s''u''=0$, and the [second derivative roughness penalty](../../../../../second-derivative-roughness-penalty.md) satisfies

$$
R(v'')=R(s'')+R(u'')\geq R(s'').
$$

If equality holds, the continuous nonnegative function $(u'')^2$ has zero integral, so $u''=0$ everywhere. Hence $u$ is an [affine function](../../../../../affine-function.md), and its zeros at two distinct [spline knots](../../../../../spline-knot.md) force $u=0$. This proves the [minimum roughness property of the natural cubic spline interpolant](../../../../../minimum-roughness-property-of-the-natural-cubic-spline-interpolant.md) and its equality case: **the unique minimum-roughness interpolant is $s$**.

For the [fixed-design nonparametric regression](../../../../../fixed-design-nonparametric-regression.md) fit, use the [penalized least squares](../../../../../penalized-least-squares.md) criterion

$$
\boxed{S_\lambda(v)=\sum_{i=1}^n\{Y_i-v(x_i)\}^2+\lambda\int_a^b v''(x)^2\,dx.}
$$

Let $s_z$ be the [natural cubic spline interpolant](../../../../../natural-cubic-spline-interpolant.md) with value [vector](../../../../../vector.md) $z=(z_1,\ldots,z_n)^T$. Replacing $v$ by $s_z$ for $z_i=v(x_i)$ leaves the residual sum unchanged and reduces the [second derivative roughness penalty](../../../../../second-derivative-roughness-penalty.md), strictly unless $v=s_z$. It therefore remains to minimize the finite-dimensional [quadratic form](../../../../../quadratic-form.md)

$$
Q_\lambda(z)=\|Y-z\|^2+\lambda z^TKz.
$$

The supplied [spline roughness penalty matrix](../../../../../spline-roughness-penalty-matrix.md) $K$ is [positive semidefinite](../../../../../positive-semidefinite-matrix.md). For every nonzero [vector](../../../../../vector.md) $w$,

$$
w^T(I+\lambda K)w=\|w\|^2+\lambda w^TKw>0.
$$

Consequently $I+\lambda K$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md), and $Q_\lambda$ is [strictly convex](../../../../../strictly-convex-function.md). Its [normal equations for linear least squares](../../../../../normal-equations-for-linear-least-squares.md) have the unique solution

$$
\boxed{\widehat z=(I+\lambda K)^{-1}Y,\qquad \widehat g_\lambda=s_{\widehat z}.}
$$

The preceding strict reduction also proves uniqueness over the whole class $C^2[a,b]$, not just over the [natural cubic splines](../../../../../natural-cubic-spline.md). This is the [cubic smoothing spline](../../../../../cubic-smoothing-spline.md). If the residual criterion is divided by $n$ instead, the corresponding formula is $(I+n\lambda K)^{-1}Y$, reflecting a change in the numerical convention for the [smoothing parameter](../../../../../smoothing-parameter.md).

The [independence](../../../../../independent-random-variables.md) and specified error [mean](../../../../../expected-value.md) and [variance](../../../../../variance-split.md) are not needed for existence or uniqueness of this minimizer. They do imply, with [smoothing matrix](../../../../../smoothing-matrix.md) $A_\lambda=(I+\lambda K)^{-1}$ and $g_X=(g(x_i))_i$, that $\mathbb E\widehat z=A_\lambda g_X$ and $\operatorname{Cov}(\widehat z)=\sigma^2A_\lambda^2$. The [null space](../../../../../kernel-of-a-linear-map.md) of $K$ consists of sampled [affine functions](../../../../../affine-function.md): these have zero roughness, and conversely zero roughness forces their [natural cubic spline interpolant](../../../../../natural-cubic-spline-interpolant.md) to be an [affine function](../../../../../affine-function.md). Thus these functions are reproduced without [bias of an estimator](../../../../../bias-of-an-estimator.md), while other components are smoothed.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
