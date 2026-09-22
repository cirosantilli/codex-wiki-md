<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

Write $q^1=u$, $q^2=v$, $\sigma_i=\partial_i\sigma$, and let $g_{ij}=\sigma_i\mathbin{\cdot}\sigma_j$ be the [first fundamental form](../../../../../first-fundamental-form.md). Since

$$
\dot\gamma=\sigma_i\dot q^i,
\qquad
\ddot\gamma=\sigma_i\ddot q^i+\sigma_{ij}\dot q^i\dot q^j,
$$

differentiating $\sigma_u\mathbin{\cdot}\dot\gamma$ and $\sigma_v\mathbin{\cdot}\dot\gamma$, or equivalently taking the two [inner products](../../../../../inner-product.md) of the second formula with $\sigma_k$, gives

$$
\sigma_k\mathbin{\cdot}\ddot\gamma
=g_{k\ell}
\left(\ddot q^\ell+\Gamma^\ell_{ij}\dot q^i\dot q^j\right).
$$

The [matrix](../../../../../matrix.md) $(g_{k\ell})$ is invertible because $\sigma$ is a regular [embedded surface parametrization](../../../../../embedded-surface-parametrization.md). Consequently the two [geodesic equations](../../../../../geodesic-equation.md) hold exactly when $\ddot\gamma$ is [orthogonal](../../../../../orthogonal-vectors.md) to both [tangent vectors](../../../../../tangent-vector.md) $\sigma_u$ and $\sigma_v$, which says precisely that $\ddot\gamma$ is a [normal vector](../../../../../normal-vector.md). This is the [ambient acceleration criterion for a surface geodesic](../../../../../ambient-acceleration-criterion-for-a-surface-geodesic.md).

Because $\dot\gamma$ is tangent and $\ddot\gamma$ is normal,

$$
\frac d{dt}|\dot\gamma|^2
=2\dot\gamma\mathbin{\cdot}\ddot\gamma=0.
$$

Thus an affinely parametrized [geodesic](../../../../../geodesic.md) has [constant speed](../../../../../constant-speed.md), as recorded by [constant speed of an affinely parametrized geodesic](../../../../../constant-speed-of-an-affinely-parametrized-geodesic.md).

For a [surface of revolution](../../../../../surface-of-revolution.md), use profile [arc length](../../../../../arc-length.md) $s$ and azimuth $\phi$. Its [Riemannian metric](../../../../../riemannian-metric.md) is

$$
ds^2+\rho(s)^2d\phi^2.
$$

The azimuth is an [ignorable coordinate](../../../../../ignorable-coordinate.md), so the corresponding [geodesic equation](../../../../../geodesic-equation.md) has the [first integral](../../../../../first-integral.md)

$$
\rho^2\dot\phi=C.
$$

If $v=|\dot\gamma|$ and $\theta$ is the oriented angle with the parallel, then the component of velocity along the parallel is

$$
v\cos\theta=\rho\dot\phi.
$$

Since $v$ is constant,

$$
\boxed{\rho\cos\theta=\frac Cv=\text{constant}.}
$$

This is the [Clairaut first integral for a surface of revolution](../../../../../clairaut-first-integral-for-a-surface-of-revolution.md).

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
