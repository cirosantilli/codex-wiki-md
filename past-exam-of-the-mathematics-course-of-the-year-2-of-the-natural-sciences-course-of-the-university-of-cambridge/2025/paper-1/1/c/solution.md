<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Close the [hyperboloid](../../../../../hyperboloid.md) segment with the two disks at $z=\pm1$, and let $V$ be its interior. The [flux](../../../../../flux.md) through either disk is zero because $A_z=0$. Thus the desired [surface integral](../../../../../surface-integral.md) is the total outward [flux](../../../../../flux.md) through the closed boundary. Since

$$
\nabla\cdot\mathbf A=3x^2+3y^2,
$$

the [divergence theorem](../../../../../divergence-theorem.md) and [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) give

$$
\begin{aligned}
\int_{\widetilde S}\mathbf A\cdot\hat{\mathbf n}\,dS
&=\int_{-1}^1\int_0^{2\pi}\int_0^{\sqrt{1+z^2}}3r^2\,r\,dr\,d\theta\,dz\\
&=\frac{3\pi}{2}\int_{-1}^1(1+z^2)^2\,dz\\
&=\frac{3\pi}{2}\left(2+\frac43+\frac25\right)
=\boxed{\frac{28\pi}{5}}.
\end{aligned}
$$

The extra factor $r$ is the [volume integral](../../../../../volume-integral.md) measure in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md); omitting it would give the wrong [flux](../../../../../flux.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
