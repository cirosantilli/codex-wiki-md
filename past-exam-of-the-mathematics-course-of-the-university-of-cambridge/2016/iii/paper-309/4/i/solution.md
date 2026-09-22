<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $t$ as an [affine parameter](../../../../../../affine-parameter.md) on each member of the [geodesic variation](../../../../../../geodesic-variation.md), so $\nabla_TT=0$. The parameter directions commute, giving $[T,S]=0$ along the variation. The [torsion-free connection](../../../../../../torsion-free-connection.md) then gives

$$
\nabla_TS-\nabla_ST=[T,S]=0.
$$

Consequently the [covariant derivative](../../../../../../covariant-derivative.md) and curvature definition give

$$
\begin{aligned}
\nabla_T\nabla_TS
&=\nabla_T\nabla_ST\\
&=R(T,S)T+\nabla_S\nabla_TT+\nabla_{[T,S]}T\\
&=R(T,S)T.
\end{aligned}
$$

This is **the geodesic-deviation equation with the stated curvature sign**:

$$
\boxed{\nabla_T\nabla_TS=R(T,S)T=R^\alpha{}_{\beta\gamma\delta}T^\beta T^\gamma S^\delta e_\alpha.}
$$

The component expression defines the slot order: $\beta$ is the vector acted on, and $\gamma,\delta$ are the two derivative directions of the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md). Both the commuting parameter directions and affine parametrization are essential; a general connecting [vector field](../../../../../../vector-field.md) or a nonaffine parameter would add terms.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
