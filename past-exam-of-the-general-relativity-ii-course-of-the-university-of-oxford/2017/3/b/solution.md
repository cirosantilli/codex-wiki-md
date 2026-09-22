<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [metric tensor](../../../../metric-tensor.md) is independent of $t$ and $\phi$, so

$$
\boxed{T=\partial_t,\qquad \Phi=\partial_\phi}
$$

are commuting [Killing vector fields](../../../../killing-vector-field-split.md). For $0<a<M$ they span the continuous [Killing vector field](../../../../killing-vector-field-split.md) algebra; every constant linear combination is also a [Killing vector field](../../../../killing-vector-field-split.md). They express [stationary spacetime](../../../../stationary-spacetime.md) and axial [symmetry](../../../../symmetry-physics.md), respectively. At the allowed endpoint $a=0$ the [spherical symmetry](../../../../spherical-symmetry.md) of [Schwarzschild spacetime](../../../../schwarzschild-spacetime-split.md) enlarges the algebra: in addition to $T$, a basis of rotational [Killing vector fields](../../../../killing-vector-field-split.md) is

$$
J_x=-\sin\phi\,\partial_\theta-\cot\theta\cos\phi\,\partial_\phi,
\qquad
J_y=\cos\phi\,\partial_\theta-\cot\theta\sin\phi\,\partial_\phi,
\qquad
J_z=\partial_\phi.
$$

Their polar-coordinate expressions are singular at the axis, but the rotational fields are smooth there.

Let $U^a=dx^a/ds$ be the tangent to any affinely parametrized [geodesic](../../../../geodesic.md). For a [Killing vector field](../../../../killing-vector-field-split.md) $X$,

$$
\frac{d}{ds}(X_aU^a)
=U^aU^b\nabla_aX_b+X_bU^a\nabla_aU^b
=U^aU^b\nabla_{(a}X_{b)}=0.
$$

This is the [geodesic conserved quantity from a Killing vector](../../../../geodesic-conserved-quantity-from-a-killing-vector.md). With $p_a=g_{ab}U^b$, choose the [energy](../../../../energy-split.md) and axial [angular momentum](../../../../angular-momentum.md) conventions

$$
\boxed{E=-p_t=-g(T,U),\qquad L=p_\phi=g(\Phi,U).}
$$

For a massive particle with [proper time](../../../../proper-time.md) parameter these are per unit rest mass; for a [null geodesic](../../../../null-geodesic.md) their common scale depends on the [affine parameter](../../../../affine-parameter.md) normalization. Expanding in the supplied [Boyer-Lindquist coordinates](../../../../boyer-lindquist-coordinates.md) gives

$$
\begin{aligned}
E&=\left(1-\frac{2Mr}{\Sigma}\right)\dot t
+\frac{2Mar\sin^2\theta}{\Sigma}\dot\phi,\\
L&=-\frac{2Mar\sin^2\theta}{\Sigma}\dot t
+\frac{\sin^2\theta}{\Sigma}
\left[(r^2+a^2)^2-a^2\Delta\sin^2\theta\right]\dot\phi.
\end{aligned}
$$

The factor of two between $g_{t\phi}$ and the coefficient of $dt\,d\phi$ is essential for these signs and coefficients.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
