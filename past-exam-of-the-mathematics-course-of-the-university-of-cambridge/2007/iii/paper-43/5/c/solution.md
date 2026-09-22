<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the convention that the residual term is a sum rather than an average, the [penalised least squares](../../../../../../penalized-least-squares.md) criterion is

$$
\boxed{J_\lambda(g)=\sum_{i=1}^n\{y_i-g(x_i)\}^2+\lambda\int_{x_1}^{x_n}\{g''(x)\}^2\,dx,\qquad\lambda>0.}
$$

Minimize over functions whose first [derivative](../../../../../../derivative.md) is absolutely continuous and whose second [derivative](../../../../../../derivative.md) is square-integrable, that is, the usual [Sobolev space](../../../../../../sobolev-space-split.md) $H^2[x_1,x_n]$. The [cubic smoothing spline](../../../../../../cubic-smoothing-spline.md) $\widehat g_\lambda$ is its minimizer, with natural [boundary conditions](../../../../../../boundary-condition.md) and linear continuation outside the data range. It is a [natural cubic spline](../../../../../../natural-cubic-spline.md) with possible knots at the observed $x_i$, but usually does not interpolate the noisy $y_i$.

To see why the minimizer is a natural [spline](../../../../../../spline-mathematics.md), for any $g$ take the [natural cubic spline interpolant](../../../../../../natural-cubic-spline-interpolant.md) $s$ through its values $g(x_i)$ and write $h=g-s$. Then $h(x_i)=0$. Integrating $\int s''h''$ by parts on every knot interval twice gives zero: the terms involving $h$ vanish at knots, the terms involving $h'$ cancel because $s''$ is continuous there, and the outer terms vanish by the natural [boundary conditions](../../../../../../boundary-condition.md). Hence

$$
\int(g'')^2=\int(s'')^2+\int(h'')^2\ge\int(s'')^2,
$$

while their [residual sums of squares](../../../../../../residual-sum-of-squares.md) agree. Replacing $g$ by $s$ never increases the criterion. This proves the [minimum roughness property of the natural cubic spline interpolant](../../../../../../minimum-roughness-property-of-the-natural-cubic-spline-interpolant.md) needed here.

For fitted values $u_i=s(x_i)$, write $\int(s'')^2=u^TKu$, where $K$ is positive semidefinite and has the sampled affine functions as its two-dimensional nullspace. The finite-dimensional minimization becomes $\|y-u\|^2+\lambda u^TKu$. Its strictly positive definite Hessian is $2(I+\lambda K)$, so it has the unique solution

$$
\boxed{\widehat u=A_\lambda y,\qquad A_\lambda=(I+\lambda K)^{-1}.}
$$

This is the [roughness-matrix formula for a natural cubic smoothing spline](../../../../../../roughness-matrix-formula-for-a-natural-cubic-smoothing-spline.md). Larger $\lambda$ penalizes curvature more strongly. As $\lambda\downarrow0$ the fit approaches interpolation; as $\lambda\to\infty$ it approaches the ordinary least-squares affine line.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
