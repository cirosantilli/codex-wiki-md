<h1 id="7/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $|z|<1$, multiply the absolutely convergent [Taylor series](../../../../../../taylor-series.md) of the sine by the [geometric series](../../../../../../geometric-series.md):

$$
\frac{\sin z}{1-z^2}=\left[\sum_{j=0}^\infty\frac{(-1)^jz^{2j+1}}{(2j+1)!}\right]\left[\sum_{k=0}^\infty z^{2k}\right].
$$

The product is odd, so all even coefficients vanish. Collecting the coefficient of $z^{2m+1}$ gives

$$
\boxed{a_{2m}=0,\qquad a_{2m+1}=\sum_{j=0}^m\frac{(-1)^j}{(2j+1)!},\qquad m=0,1,2,\ldots.}
$$

For example, the first terms are $z+5z^3/6+101z^5/120+\cdots$. The denominator vanishes at $z=\pm1$, and the numerator is nonzero there, so these are genuine [simple poles](../../../../../../simple-pole.md). Therefore $\boxed{R=1}$ is the [radius of convergence](../../../../../../radius-of-convergence.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [7](../../../7.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
