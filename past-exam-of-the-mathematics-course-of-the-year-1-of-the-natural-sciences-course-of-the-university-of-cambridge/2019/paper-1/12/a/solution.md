<h1 id="12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The height is constant along each circular ring, whose [area element](../../../../../area-element-of-a-surface.md) after angular integration is $2\pi r\,dr$. The [volume integral](../../../../../volume-integral.md) in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) is therefore

$$
V=2\pi\int_0^R rR e^{-r/R}\,dr=2\pi R^3\int_0^1ue^{-u}\,du.
$$

Here $u=r/R$. Using [integration by parts](../../../../../integration-by-parts.md), $\int_0^1ue^{-u}\,du=[-(u+1)e^{-u}]_0^1=1-2/e$. Hence

$$
\boxed{R=\left[\frac{V}{2\pi(1-2/e)}\right]^{1/3}.}
$$

The dimensionless coefficient is positive, and the cube root of a [volume](../../../../../volume.md) has the required [physical dimension](../../../../../physical-dimension.md) of [length](../../../../../length.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
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
