<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $g=x^2+y^2+z^2$. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations are

$$
y=2\lambda x,\qquad x+z=2\lambda y,\qquad y=2\lambda z,
\qquad x^2+y^2+z^2=1.
$$

Taking the [dot product](../../../../../dot-product.md) with $(x,y,z)^T$ gives $2T=2\lambda$, so $\lambda=T$.

If $\lambda\ne0$, the first and third equations give $x=z$. The middle equation then gives $x=\lambda y$, so $2\lambda^2=1$. The norm constraint gives $x^2=z^2=1/4$ and $y^2=1/2$. Thus the hottest points and their temperature are

$$
\boxed{(x,y,z)=\left(\frac\varepsilon2,\frac\varepsilon{\sqrt2},\frac\varepsilon2\right),\quad
T_{\max}=\frac1{\sqrt2},\quad\varepsilon\in\{-1,1\}}.
$$

The coldest points are

$$
\boxed{(x,y,z)=\left(\frac\varepsilon2,-\frac\varepsilon{\sqrt2},\frac\varepsilon2\right),\quad
T_{\min}=-\frac1{\sqrt2},\quad\varepsilon\in\{-1,1\}}.
$$

For $\lambda=0$, the equations give $y=0$, $z=-x$, and hence the other two constrained [stationary points](../../../../../stationary-point.md) are

$$
\boxed{(x,y,z)=\left(\frac\varepsilon{\sqrt2},0,-\frac\varepsilon{\sqrt2}\right),\qquad T=0}.
$$

They are saddle points of the restriction to the [sphere](../../../../../sphere.md): with $u=(x+z)/\sqrt2$ and $v=y$ as local tangent coordinates there, $T=\sqrt2uv$ changes sign in every neighbourhood. The surface is compact and smooth, so the listed extreme temperatures are global. Here “zero gradient on the surface” means zero [surface gradient](../../../../../surface-gradient.md); the ambient [gradient](../../../../../gradient.md) at the hottest and coldest points is normal to the [sphere](../../../../../sphere.md), rather than zero.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
