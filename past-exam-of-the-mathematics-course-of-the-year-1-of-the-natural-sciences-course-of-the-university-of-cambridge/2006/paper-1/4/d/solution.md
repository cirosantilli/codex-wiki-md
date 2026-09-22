<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Orient the triangle by the path $A\to B\to C\to A$. The [cross product](../../../../../cross-product.md) $(B-A)\times(C-A)=(0,1,0)$ gives the positive [normal vector](../../../../../normal-vector.md). In the plane $y=1$, the triangular region is $x,z\geq0$, $x+z\leq1$. The surface integral in [Stokes theorem](../../../../../stokes-theorem.md) is therefore

$$
\int_0^1\int_0^{1-z}4xz^2\,dx\,dz=2\int_0^1z^2(1-z)^2\,dz=\frac1{15}.
$$

For the boundary [line integral](../../../../../line-integral.md), $AB$ has $z=0$, so contributes zero. On $BC$, $x=0$ and only $dz$ is nonzero, so its contribution is also zero. Parametrize $CA$ by $(x,y,z)=(t,1,1-t)$, $0\leq t\leq1$. Its contribution is

$$
\int_0^1[2t(1-t)^3-t^2(1-t)^2]dt=\frac1{15}.
$$

Thus **both oriented integrals equal $1/15$**. Reversing the orientation would reverse both signs.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
