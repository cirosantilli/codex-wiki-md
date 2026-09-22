<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Integrating the [Dirac delta distribution](../../../../../../dirac-delta-function.md) in $x_3$ reduces the inertia integral to the planar lamina. Use $u=x_1-x_2$, $v=x_2$, so $x_1=u+v$ and the parallelogram becomes the square $-D\leq u,v\leq D$, with unit [Jacobian determinant](../../../../../../jacobian-determinant.md). The mass is $M=4\sigma D^2$, and symmetry gives a [centre of mass](../../../../../../center-of-mass.md) at the origin.

Odd rectangular integrals vanish. The required second moments are

$$
\begin{aligned}
\int x_1^2dm&=\sigma\int_{-D}^D\!\int_{-D}^D(u+v)^2du\,dv=\frac83\sigma D^4,\\
\int x_2^2dm&=\sigma\int_{-D}^D\!\int_{-D}^D v^2du\,dv=\frac43\sigma D^4,\\
\int x_1x_2dm&=\sigma\int_{-D}^D\!\int_{-D}^D(u+v)v\,du\,dv=\frac43\sigma D^4.
\end{aligned}
$$

The mixed moments involving $x_3$ vanish. Hence the [inertia tensor](../../../../../../inertia-tensor.md) is

$$
\boxed{I=\frac{4\sigma D^4}{3}\begin{pmatrix}1&-1&0\\-1&2&0\\0&0&3\end{pmatrix}=\frac{MD^2}{3}\begin{pmatrix}1&-1&0\\-1&2&0\\0&0&3\end{pmatrix}.}
$$

The off-diagonal entries are minus the product moment, not the product moment itself. This is the unit-shear case of the [inertia tensor of a sheared rectangular lamina](../../../../../../inertia-tensor-of-a-sheared-rectangular-lamina.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
