<h1 id="25g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a positively oriented local parametrization $X(u,v)$ with [first fundamental form](../../../../../../first-fundamental-form.md)

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,
$$

the [area element of a surface](../../../../../../area-element-of-a-surface.md) is

$$
dA=\sqrt{EG-F^2}\,du\wedge dv.
$$

Under an orientation-preserving coordinate change, the Jacobian from $du\wedge dv$ cancels the inverse Jacobian in the square root of the metric determinant. Hence these local expressions agree and define a global two-form.

The [Euler characteristic](../../../../../../euler-characteristic.md) may be defined from any finite triangulation by

$$
\chi(S)=V-E+F,
$$

or equivalently by the alternating sum of the dimensions of the rational [homology](../../../../../../homology-split.md) groups. Subdivision leaves $V-E+F$ unchanged, and the homological formula shows that it is a topological invariant, so the definition does not depend on the triangulation.

Give the boundary its induced orientation and parametrize it by [arc length](../../../../../../arc-length.md). If $T$ is its unit tangent and $N$ is the chosen [unit normal](../../../../../../unit-normal.md) to the surface, its signed [geodesic curvature](../../../../../../geodesic-curvature.md) is

$$
k_g=\langle D_sT,N\times T\rangle,
$$

where $D_s$ is the [surface covariant derivative](../../../../../../surface-covariant-derivative.md). The [Gauss-Bonnet theorem](../../../../../../gauss-bonnet-theorem.md) for a compact oriented surface with smooth boundary and no corners is

$$
\int_S K\,dA+\int_{\partial S}k_g\,ds=2\pi\chi(S),
$$

where $K$ is the [Gaussian curvature](../../../../../../gaussian-curvature.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25G](../../25g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
