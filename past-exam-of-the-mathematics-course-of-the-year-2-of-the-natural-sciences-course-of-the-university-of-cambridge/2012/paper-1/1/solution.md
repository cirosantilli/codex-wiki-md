<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Using [Cartesian coordinates](../../../../cartesian-coordinate-system.md), the [Levi-Civita symbol](../../../../levi-civita-symbol.md) and the [Einstein summation convention](../../../../einstein-notation.md), the constant-vector assumption gives

$$
\begin{aligned}
[\nabla\times(\mathbf a\times\mathbf F)]_i
&=\epsilon_{ijk}\epsilon_{klm}a_l\partial_jF_m\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})a_l\partial_jF_m\\
&=a_i\partial_jF_j-a_j\partial_jF_i.
\end{aligned}
$$

Recognizing the [divergence](../../../../divergence.md) and [directional derivative](../../../../directional-derivative.md) proves

$$
\boxed{\nabla\times(\mathbf a\times\mathbf F)=\mathbf a(\nabla\cdot\mathbf F)-(\mathbf a\cdot\nabla)\mathbf F.}
$$

Here the contractions use the [Kronecker delta](../../../../kronecker-delta.md).

For an oriented piecewise smooth surface $S$ with boundary $C$, [Stokes theorem](../../../../stokes-theorem.md) states

$$
\oint_C\mathbf Q\cdot d\mathbf l=\int_S(\nabla\times\mathbf Q)\cdot d\mathbf S,
$$

where the orientations obey the [right-hand rule](../../../../right-hand-rule.md) and $\mathbf Q$ is continuously differentiable near $S$. Apply it to $\mathbf Q=\mathbf F\times\mathbf a$. The [scalar triple product](../../../../scalar-triple-product.md) gives

$$
\begin{aligned}
\mathbf a\cdot\oint_Cd\mathbf l\times\mathbf F
&=\oint_C(\mathbf F\times\mathbf a)\cdot d\mathbf l\\
&=\int_S\left[(\mathbf a\cdot\nabla)\mathbf F-\mathbf a(\nabla\cdot\mathbf F)\right]\cdot d\mathbf S.
\end{aligned}
$$

The last integrand is $\mathbf a\cdot[(d\mathbf S\times\nabla)\times\mathbf F]$, as the component formula

$$
[(d\mathbf S\times\nabla)\times\mathbf F]_i=dS_j\partial_iF_j-dS_i\partial_jF_j
$$

shows. Since $\mathbf a$ is arbitrary, the [cross-product form of Stokes theorem](../../../../cross-product-form-of-stokes-theorem.md) follows:

$$
\boxed{\oint_Cd\mathbf l\times\mathbf F=\int_S(d\mathbf S\times\nabla)\times\mathbf F.}
$$

The derivatives in the surface expression act on $\mathbf F$, not on the surface element.

For the specified square, the path is clockwise when viewed from positive $z$, so the compatible [unit normal](../../../../unit-normal.md) is $-\mathbf e_z$. On the first and fourth edges, $d\mathbf l$ and $\mathbf r$ are parallel, giving zero [cross product](../../../../cross-product.md). On the second edge, $y=1$ and $x$ runs from $0$ to $1$, so $d\mathbf l\times\mathbf r=\mathbf e_z\,dx$ contributes $\mathbf e_z$. On the third edge, $x=1$ and $y$ runs from $1$ to $0$, so the contribution is $-\mathbf e_z\int_1^0dy=\mathbf e_z$. Thus the [line integral](../../../../line-integral.md) is $2\mathbf e_z$.

For an independent [surface integral](../../../../surface-integral.md), $\partial_iF_j=\delta_{ij}$ and $\nabla\cdot\mathbf F=3$ for the [position vector](../../../../position-vector.md) field. Its integrand is therefore $d\mathbf S-3d\mathbf S=-2d\mathbf S$. The square has unit area and downward orientation, giving

$$
\boxed{\oint_Cd\mathbf l\times\mathbf r=2\mathbf e_z=\int_S(-2d\mathbf S).}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
