<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a piecewise continuous function of exponential order on $t\geq0$, its unilateral [Laplace transform](../../../../laplace-transform.md) is

$$
\boxed{F(p)=\int_0^\infty e^{-pt}f(t)\,dt.}
$$

The [Bromwich inversion formula](../../../../bromwich-inversion-formula.md), at a point of continuity, is

$$
\boxed{f(t)=\frac1{2\pi i}\lim_{T\to\infty}\int_{\gamma-iT}^{\gamma+iT}e^{pt}F(p)\,dp.}
$$

The [Bromwich contour](../../../../bromwich-contour.md) is a straight vertical line, traversed upwards, with $\gamma$ to the right of the abscissa of convergence and hence of all singularities of the transform. Under the usual piecewise smoothness assumptions, at a jump the symmetric inversion limit gives the mean of the two one-sided values.

In the transform in the question, put $\lambda=e^{-t}$. Then $d\lambda=-e^{-t}dt$ and

$$
H(s)=\int_0^\infty e^{-st}h(e^{-t})\,dt.
$$

Thus the [restricted Mellin transform on the unit interval](../../../../restricted-mellin-transform-on-the-unit-interval.md) is the [Laplace transform](../../../../laplace-transform.md) of $f(t)=h(e^{-t})$. Apply the [Bromwich inversion formula](../../../../bromwich-inversion-formula.md) with $t=-\log\lambda$, where $0<\lambda<1$, to obtain

$$
\boxed{h(\lambda)=\frac1{2\pi i}\lim_{T\to\infty}\int_{\gamma-iT}^{\gamma+iT}\lambda^{-s}H(s)\,ds.}
$$

Here $\gamma$ lies in the convergence half-plane of $H$. At a discontinuity this formula has the same mean-value interpretation. The real [natural logarithm](../../../../natural-logarithm.md) defines $\lambda^{-s}$ unambiguously.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
