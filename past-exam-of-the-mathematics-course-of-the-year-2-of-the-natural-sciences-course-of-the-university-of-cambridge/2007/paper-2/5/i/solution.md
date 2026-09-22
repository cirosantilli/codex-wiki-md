<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The unilateral [Laplace transform](../../../../../laplace-transform.md) is $\bar f(p)=\int_0^\infty e^{-pt}f(t)dt$ in its [region of absolute convergence of a Laplace transform](../../../../../region-of-absolute-convergence-of-a-laplace-transform.md). Under the usual inversion hypotheses, the [Bromwich inversion formula](../../../../../bromwich-inversion-formula.md) is

$$
f(t)=\frac1{2\pi i}\lim_{R\to\infty}\int_{c-iR}^{c+iR}e^{pt}\bar f(p)dp.
$$

The vertical [Bromwich contour](../../../../../bromwich-contour.md) is directed upward, with $c$ inside the transform's convergence half-plane and to the right of all its singularities. At discontinuities the standard symmetric inversion gives the mean of the one-sided values.

For a piecewise continuously [differentiable](../../../../../differentiable-function.md) $f$ with an integrable transformed [derivative](../../../../../derivative.md), [integration by parts](../../../../../integration-by-parts.md) gives the [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md):

$$
\int_0^\infty e^{-pt}f'(t)dt=\left[e^{-pt}f(t)\right]_0^\infty+p\int_0^\infty e^{-pt}f(t)dt=\boxed{p\bar f(p)-f(0)}.
$$

Here the upper endpoint vanishes by the given decay condition, and right continuity at zero supplies the lower endpoint.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
