<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) $x=r\cos\theta$, $y=r\sin\theta$. The [Jacobian determinant](../../../../../jacobian-determinant.md) gives

$$
\boxed{dV=r\,dr\,d\theta\,dz.}
$$

The inequalities imply $-d<z<0$ and $0\le r<a\sqrt{1+z/d}$. Thus the [volume](../../../../../volume.md) is

$$
\begin{aligned}
V&=\int_{-d}^0\int_0^{2\pi}\int_0^{a\sqrt{1+z/d}}r\,dr\,d\theta\,dz\\
&=\pi a^2\int_{-d}^0\left(1+\frac zd\right)dz\\
&=\boxed{\frac12\pi a^2d.}
\end{aligned}
$$

Equivalently, integrating vertically first gives $V=\int_0^{2\pi}\int_0^a\int_{d(r^2/a^2-1)}^0r\,dz\,dr\,d\theta$. The region is bounded by an [elliptic paraboloid](../../../../../elliptic-paraboloid.md) and its top disc; its [volume](../../../../../volume.md) is half that of the cylinder with base radius $a$ and height $d$. Including or excluding the boundary surfaces does not change the [volume](../../../../../volume.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
