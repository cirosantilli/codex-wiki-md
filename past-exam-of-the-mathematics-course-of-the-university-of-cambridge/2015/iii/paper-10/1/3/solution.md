<h1 id="1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [radial function](../../../../../../radial-function.md), the [Laplacian](../../../../../../laplacian.md) is $\Delta\phi=\phi_{rr}+2\phi_r/r$. Introduce the [retarded and advanced null coordinates](../../../../../../retarded-and-advanced-null-coordinates.md) and the [radial reduction of the three-dimensional wave equation](../../../../../../radial-reduction-of-the-three-dimensional-wave-equation.md):

$$
u=t-r,\qquad v=t+r,\qquad r=\frac{v-u}{2},\qquad w=r\phi.
$$

The [chain rule](../../../../../../chain-rule.md) gives $\partial_t=\partial_u+\partial_v$ and $\partial_r=-\partial_u+\partial_v$. Consequently the inhomogeneous [wave equation](../../../../../../wave-equation-split.md) is

$$
\boxed{-4\phi_{uv}+\frac{4}{v-u}(\phi_v-\phi_u)=F.}
$$

Multiplying the radial [wave equation](../../../../../../wave-equation-split.md) by $r$ removes its first-order radial derivative:

$$
-w_{tt}+w_{rr}=rF.
$$

Thus the particularly useful [retarded and advanced null coordinates](../../../../../../retarded-and-advanced-null-coordinates.md) form is

$$
\boxed{-4w_{uv}=rF,\qquad
\partial_u\partial_v\bigl((v-u)\phi\bigr)=-\frac{v-u}{4}F.}
$$

These formulas hold for $r>0$. At the axis, smooth [spherical symmetry](../../../../../../spherical-symmetry.md) imposes $\phi_r(t,0)=0$ and $w(t,0)=0$; equivalently $w$ has a smooth [odd extension](../../../../../../odd-extension.md) across $r=0$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
