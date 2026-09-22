<h1 id="24h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Theorema Egregium](../../../../../../theorema-egregium.md) states that the [Gaussian curvature](../../../../../../gaussian-curvature.md) of a surface in $\mathbb R^3$ is determined entirely by its [first fundamental form](../../../../../../first-fundamental-form.md); in particular a local [isometry](../../../../../../isometry.md) preserves it.

Let $r(u^1,u^2)$ be a regular parametrization, $g_{ij}=r_i\cdot r_j$, $n$ a unit normal, and $b_{ij}=r_{ij}\cdot n$ the [second fundamental form](../../../../../../second-fundamental-form-split.md). Differentiating the metric and decomposing $r_{ij}$ into tangent and normal parts gives the Gauss formula

$$
r_{ij}=\Gamma^k_{ij}r_k+b_{ij}n,\qquad
\Gamma^k_{ij}=\frac12g^{k\ell}(\partial_i g_{j\ell}+\partial_jg_{i\ell}-\partial_\ell g_{ij}).
$$

Differentiating $n\cdot r_j=0$ gives $n_i=-b_i{}^kr_k$, the Weingarten formula. Compute two successive ambient derivatives of a tangent vector and subtract them. Ambient derivatives commute, so their tangential parts yield the [Gauss equation](../../../../../../gauss-equation.md)

$$
R(X,Y)Z=b(Y,Z)SX-b(X,Z)SY,
$$

where $S$ is the shape operator and $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$ is the intrinsic curvature of the connection with the displayed Christoffel symbols. Taking $X=\partial_1,Y=\partial_2,Z=\partial_2$ and the inner product with $\partial_1$ gives

$$
\langle R(\partial_1,\partial_2)\partial_2,\partial_1\rangle=b_{11}b_{22}-b_{12}^2.
$$

But $K=\det S=\det(b)/\det(g)$, so

$$
\boxed{K=\frac{\langle R(\partial_1,\partial_2)\partial_2,\partial_1\rangle}{g_{11}g_{22}-g_{12}^2}.}
$$

Both the connection and its curvature on the right are computed from $g$ and its derivatives alone. This proves the theorem, rather than merely using its name as a substitute for the argument.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24H](../../24h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
