<h1 id="12/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [embedded surface parametrization](../../../../../embedded-surface-parametrization.md)

$$
\mathbf X(r,\theta)=\left(r\cos\theta,r\sin\theta,a\left(1-\frac{r^2}{b^2}\right)\right).
$$

Its tangent vectors have [cross product](../../../../../cross-product.md)

$$
\mathbf X_r\times\mathbf X_\theta
=\left(\frac{2ar^2}{b^2}\cos\theta,
\frac{2ar^2}{b^2}\sin\theta,r\right),
$$

whose magnitude is $r\sqrt{1+4a^2r^2/b^4}$. Thus the [surface area](../../../../../surface-area.md) is

$$
A=\alpha\int_0^R r\sqrt{1+\frac{4a^2r^2}{b^4}}\,dr.
$$

With $u=1+4a^2r^2/b^4$, the radial integral becomes $b^4(8a^2)^{-1}\int u^{1/2}\,du$. Evaluating its endpoints gives

$$
\boxed{A=\frac{\alpha b^4}{12a^2}
\left[\left(1+\frac{4a^2}{b^2}\right)^{3/2}-1\right]}.
$$

This is the scalar-area part of the [paraboloid sector surface measures](../../../../../paraboloid-sector-surface-measures.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [12](../../12.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
