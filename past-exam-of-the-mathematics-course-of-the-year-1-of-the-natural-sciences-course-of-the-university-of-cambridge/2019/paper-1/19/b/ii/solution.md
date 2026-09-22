<h1 id="19/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Newton root-finding iteration](../../../../../../newton-root-finding-iteration.md) for this [quadratic polynomial](../../../../../../quadratic-polynomial.md) is

$$
x_{k+1}=x_k-\frac{x_k^2-2\varepsilon x_k-1}{2(x_k-\varepsilon)}
=\frac{x_k^2+1}{2(x_k-\varepsilon)}.
$$

At $x_0=1$, it gives $x_1=1/(1-\varepsilon)$. Its [geometric series](../../../../../../geometric-series.md) expansion is $1+\varepsilon+\varepsilon^2+\varepsilon^3+O(\varepsilon^4)$. Subtracting the expansion of the [polynomial root](../../../../../../root-of-a-polynomial.md) yields

$$
x_1-x_*=\frac12\varepsilon^2+\varepsilon^3+O(\varepsilon^4),
\qquad\boxed{|x_1-x_*|\sim\frac12|\varepsilon|^2,\qquad n_1=2.}
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [19](../../../19.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
