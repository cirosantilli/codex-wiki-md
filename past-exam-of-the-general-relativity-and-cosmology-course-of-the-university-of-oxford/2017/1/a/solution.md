<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [covariant derivative](../../../../covariant-derivative.md) differentiates a [vector field](../../../../vector-field.md) while accounting for how its [coordinate basis](../../../../coordinate-basis.md) changes between neighboring points. For the [Levi-Civita connection](../../../../levi-civita-connection.md),

$$
\boxed{
v^\beta{}_{;\gamma}
=\nabla_\gamma v^\beta
=\partial_\gamma v^\beta+\Gamma^\beta{}_{\gamma\delta}v^\delta.
}
$$

The [Christoffel symbol](../../../../christoffel-symbol.md) term makes this a [tensor](../../../../tensor.md) with one contravariant and one covariant index; ordinary [partial derivatives](../../../../partial-derivative.md) of vector components do not generally have that transformation law. Equivalently, one compares the neighboring vector with the original after [parallel transport](../../../../parallel-transport.md).

For a curve $x^\gamma(\lambda)$ with tangent $U^\gamma=dx^\gamma/d\lambda$, contraction gives the [covariant derivative along a curve](../../../../covariant-derivative-along-a-curve.md)

$$
\boxed{
\frac{Dv^\beta}{d\lambda}
=U^\gamma\nabla_\gamma v^\beta
=\frac{dv^\beta}{d\lambda}
+\Gamma^\beta{}_{\gamma\delta}U^\gamma v^\delta.
}
$$

It is the rate of change measured relative to a [parallel transport](../../../../parallel-transport.md) frame along the curve. It vanishes precisely when $v$ undergoes [parallel transport](../../../../parallel-transport.md) along that curve. If $v=U$, it is the covariant acceleration, and its vanishing is the [geodesic equation](../../../../geodesic-equation.md) with an [affine parameter](../../../../affine-parameter.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
