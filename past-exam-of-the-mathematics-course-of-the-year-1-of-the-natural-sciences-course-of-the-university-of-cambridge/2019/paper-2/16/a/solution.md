<h1 id="16/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each of the three surface pieces is invariant under $y\mapsto-y$, while $y^3$ is an [odd function](../../../../../odd-function.md) under that reflection. Its [surface integral](../../../../../surface-integral.md) therefore vanishes on each piece separately. Only $z$ contributes.

On the cylindrical side, use [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) $x=a\cos\phi$, $y=a\sin\phi$, with [area element](../../../../../area-element-of-a-surface.md) $dS=a\,d\phi\,dz$:

$$
I_{\mathrm{side}}=\int_0^{2\pi}\int_0^b az\,dz\,d\phi=\pi ab^2.
$$

The upper disc has constant $z=b$ and area $\pi a^2$, giving $I_{\mathrm{top}}=\pi a^2b$. On the hemispherical indentation, use [spherical coordinates](../../../../../spherical-coordinate-system.md) with $z=a\cos\theta$ and $dS=a^2\sin\theta\,d\theta\,d\phi$:

$$
I_{\mathrm{hemisphere}}=2\pi a^3\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta=\pi a^3.
$$

Adding the three contributions yields

$$
\boxed{\iint_S(z+y^3)\,dS=\pi a(b^2+ab+a^2)}.
$$

This is a scalar [surface integral](../../../../../surface-integral.md), so the indentation contributes positively through $dS$; an inward or outward orientation does not change its sign.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [16](../../16.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
