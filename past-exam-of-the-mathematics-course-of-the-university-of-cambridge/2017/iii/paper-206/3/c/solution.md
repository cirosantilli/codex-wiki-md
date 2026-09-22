<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\lambda>0$, minimize the [smoothing spline](../../../../../../smoothing-spline.md) objective over the [Sobolev space](../../../../../../sobolev-space-split.md) of functions with square-integrable second derivative on the observed interval:

$$
J(m)=\sum_i\{Y_i-m(X_i)\}^2+\lambda\int_{X_{\min}}^{X_{\max}}\{m''(x)\}^2\,dx.
$$

The [roughness penalty](../../../../../../roughness-penalty.md) measures curvature; its null space consists of [affine functions](../../../../../../affine-function.md). To see why the minimizer is a [natural cubic spline](../../../../../../natural-cubic-spline.md), let $g$ be the natural spline interpolating the values of any competitor $m$ at its distinct observation locations, and put $h=m-g$. [Integration by parts](../../../../../../integration-by-parts.md) twice on each knot interval gives $\int g''h''=0$: $g''''=0$ on each interval, $h$ vanishes at the knots, $g''$ is continuous, and $g''$ vanishes at the outer endpoints. Hence

$$
\int(m'')^2=\int(g'')^2+\int(h'')^2\ge\int(g'')^2,
$$

while both functions have the same residual sum of squares. This proves the reduction to a finite-dimensional spline space.

For distinct $X_i$ and $n\ge2$, use its $n$-dimensional [basis](../../../../../../basis.md), write $B_{ij}=b_j(X_i)$, and define the [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md)

$$
\Omega_{jk}=\int b_j''(x)b_k''(x)\,dx.
$$

The [penalized least squares](../../../../../../penalized-least-squares.md) problem is $\|Y-B\beta\|^2+\lambda\beta^T\Omega\beta$, so

$$
\boxed{\widehat m_\lambda(x)=b(x)^T(B^TB+\lambda\Omega)^{-1}B^TY.}
$$

Use linear continuation outside the observation interval. The fitted-value matrix is $S_\lambda=B(B^TB+\lambda\Omega)^{-1}B^T$; its trace gives the [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md). As $\lambda$ decreases to zero, the natural spline approaches interpolation, with trace $n$; as it grows without bound, the fit approaches [ordinary least squares](../../../../../../ordinary-least-squares.md) on $1,x$, with trace two. For $\lambda=0$ the criterion alone does not determine values between observations; the natural interpolant is the limiting convention. Repeated observation locations are combined by using distinct knots and their multiplicities as weights, rather than pretending the spline design has $n$ independent interpolation values.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
