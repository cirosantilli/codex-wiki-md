<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The PDF diagram includes a solid base of thickness $d$, occupying $-d\leq z\leq0$ and $0\leq r\leq R$. Above it, $0\leq z\leq h$, the metal lies between the two specified curved surfaces. In [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), the [Jacobian determinant](../../../../../jacobian-determinant.md) contributes a factor $r$, so the [mass](../../../../../mass.md) is

$$
\begin{aligned}
M={}&\rho\int_{-d}^0\int_0^{2\pi}\int_0^Rr\,dr\,d\phi\,dz\\
&+\rho\int_0^h\int_0^{2\pi}\int_{(9/10)R(1+z^2/h^2)}^{R(1+z^2/h^2)}r\,dr\,d\phi\,dz.
\end{aligned}
$$

The base contributes $\pi\rho R^2d$. The wall contributes

$$
\pi\rho R^2\left(1-\frac{81}{100}\right)\int_0^h\left(1+\frac{z^2}{h^2}\right)^2dz=\pi\rho R^2\frac{19}{100}h\left(1+\frac23+\frac15\right)=\frac{133}{375}\pi\rho R^2h.
$$

Consequently

$$
\boxed{M=\pi\rho R^2\left(d+\frac{133h}{375}\right).}
$$

The base thickness $d$ comes from the diagram; omitting it would omit part of the cup's [volume](../../../../../volume.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
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
