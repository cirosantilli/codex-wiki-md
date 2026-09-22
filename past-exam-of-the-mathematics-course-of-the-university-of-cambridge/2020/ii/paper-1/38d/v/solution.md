<h1 id="38d/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Differentiate $B_{\alpha\beta}=\nabla_\beta X_\alpha$ along $X$ and commute the two [covariant derivatives](../../../../../../covariant-derivative.md):

$$
X^\mu\nabla_\mu B_{\alpha\beta}
=X^\mu\nabla_\mu\nabla_\beta X_\alpha
=X^\mu\nabla_\beta\nabla_\mu X_\alpha
-X^\mu R^\nu{}_{\alpha\mu\beta}X_\nu,
$$

where the sign is the covector form of the [Ricci identity](../../../../../../curvature-commutator-on-a-covariant-tensor.md). Apply the [product rule](../../../../../../product-rule.md) to the first term:

$$
X^\mu\nabla_\beta\nabla_\mu X_\alpha
=\nabla_\beta(X^\mu\nabla_\mu X_\alpha)
-(\nabla_\beta X^\mu)(\nabla_\mu X_\alpha).
$$

The first term vanishes by the [geodesic equation](../../../../../../geodesic-equation.md), and the second is

$$
-B^\mu{}_\beta B_{\alpha\mu}.
$$

Finally the pair symmetries and antisymmetries of the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) give

$$
-X^\mu X_\nu R^\nu{}_{\alpha\mu\beta}
=R_{\mu\beta\alpha}{}^\nu X^\mu X_\nu.
$$

Consequently

$$
\boxed{
X^\mu\nabla_\mu B_{\alpha\beta}
=-B^\mu{}_\beta B_{\alpha\mu}
+R_{\mu\beta\alpha}{}^\nu X^\mu X_\nu.
}
$$

This is the [Riccati equation for a timelike geodesic congruence](../../../../../../riccati-equation-for-a-timelike-geodesic-congruence.md); taking its spatial trace is the starting point for the timelike [Raychaudhuri equation](../../../../../../friedmann-acceleration-equation.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [38D](../../38d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
