<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At the origin, the [Poisson kernel](../../../../../poisson-kernel.md) is one, so the [mean value property for harmonic functions](../../../../../mean-value-property-for-harmonic-functions.md) gives

$$
u(0)=\frac1{2\pi}\int_0^{2\pi}f(\phi')\,d\phi'.
$$

For $0<r<1$, the denominator in the [Poisson kernel](../../../../../poisson-kernel.md) satisfies $1-2r\cos\vartheta+r^2\geq(1-r)^2$. Thus

$$
0<P(r,\vartheta)\leq\frac{1-r^2}{(1-r)^2}=\frac{1+r}{1-r}.
$$

The nonnegativity of $f$ allows this upper bound to be inserted under the [Poisson integral on the unit disk](../../../../../poisson-integral-on-the-unit-disk.md):

$$
\boxed{u(r,\phi)\leq\frac{1+r}{1-r}\,u(0)}.
$$

This is the upper bound in the [Harnack inequality on the unit disk](../../../../../harnack-inequality-on-the-unit-disk.md). The same argument with the minimum of the [Poisson kernel](../../../../../poisson-kernel.md) gives the corresponding lower bound $(1-r)u(0)/(1+r)$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
