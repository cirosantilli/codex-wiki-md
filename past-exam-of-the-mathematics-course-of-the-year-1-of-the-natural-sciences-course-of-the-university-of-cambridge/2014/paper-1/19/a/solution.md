<h1 id="19/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the formal [Maclaurin series](../../../../../maclaurin-series.md) as $\sum_{n\geq0}a_nx^n$, where $a_n=f^{(n)}(0)/n!$. If the successive nonzero coefficient ratios have a limit, the [ratio test](../../../../../ratio-test.md) gives

$$
\left|\frac{a_{n+1}x^{n+1}}{a_nx^n}\right|
=|x|\left|\frac{f^{(n+1)}(0)}{(n+1)f^{(n)}(0)}\right|\longrightarrow\frac{|x|}{R},
$$

so the series converges absolutely for $|x|<R$, where

$$
\boxed{R=\lim_{n\to\infty}\left|\frac{(n+1)f^{(n)}(0)}{f^{(n+1)}(0)}\right|.}
$$

If that ratio does not exist, the [Cauchy-Hadamard theorem](../../../../../cauchy-hadamard-theorem.md) gives the general formula $R^{-1}=\limsup|a_n|^{1/n}$. The [radius of a Maclaurin series from successive derivatives](../../../../../radius-of-a-maclaurin-series-from-successive-derivatives.md) concerns convergence of the series; equality to the original [function](../../../../../function-split.md) additionally requires [analyticity](../../../../../analyticity.md) or a vanishing [Taylor remainder](../../../../../taylor-remainder.md). Mere differentiability, or even smoothness, does not ensure that equality.

For the specified logarithm,

$$
\ln(2+x)=\ln2+\sum_{n=1}^{\infty}\frac{(-1)^{n+1}x^n}{n2^n},\qquad |x|<2.
$$

The absolute successive-term ratio tends to $|x|/2$, so **the interval of [absolute convergence](../../../../../absolute-convergence.md) is $(-2,2)$**. At $x=2$ the nonconstant terms are the alternating harmonic series, which converges conditionally to $\ln2$, giving the full sum $\ln4$. At $x=-2$ all nonconstant terms are $-1/n$, so the series diverges to $-\infty$; the original logarithm is also undefined there. Thus the full real convergence interval is **$(-2,2]$**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
