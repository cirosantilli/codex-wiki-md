<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The event $Y_n\leq z$ occurs precisely when every one of the first $n$ levels is at most $z$. Their [independence](../../../../../../independent-random-variables.md) gives the [cumulative distribution function](../../../../../../cumulative-distribution-function.md)

$$
\boxed{P(Y_n\leq z)=F(z)^n,\qquad z\geq0.}
$$

For any nonnegative [random variable](../../../../../../random-variable-split.md), the pointwise identity $Y_n=\int_0^\infty\mathbf1_{\{Y_n>z\}}\,dz$ and the [Tonelli theorem](../../../../../../tonelli-theorem.md) allow interchange of [expectation](../../../../../../expected-value.md) and integral. Hence

$$
\boxed{EY_n=\int_0^\infty P(Y_n>z)\,dz
=\int_0^\infty[1-F(z)^n]\,dz.}
$$

This identity holds as an extended nonnegative integral; finiteness of the mean is not guaranteed by continuity of $F$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
