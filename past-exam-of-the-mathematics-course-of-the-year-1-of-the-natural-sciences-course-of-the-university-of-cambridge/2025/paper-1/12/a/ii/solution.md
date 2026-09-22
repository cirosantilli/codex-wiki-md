<h1 id="12/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $\ell=\ln2$. Applying the [exponential series](../../../../../../exponential-series.md) and the [Maclaurin series](../../../../../../maclaurin-series.md) of the [sine](../../../../../../sine.md) gives

$$
2^x-2^{-x}=e^{\ell x}-e^{-\ell x}=2\ell x+\frac{\ell^3}{3}x^3+O(x^5),\qquad \sin x=x-\frac{x^3}{6}+O(x^5).
$$

Multiply the two [power series](../../../../../../power-series.md), retaining every contribution through degree four:

$$
(2^x-2^{-x})\sin x=\boxed{2(\ln2)x^2+\frac{(\ln2)^3-\ln2}{3}x^4+O(x^6)}.
$$

Since $0<\ln2<1$, the coefficient of $x^4$ is nonzero, so these are indeed the first two nonzero terms. The remainder is in [Big O notation](../../../../../../big-o-notation.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
