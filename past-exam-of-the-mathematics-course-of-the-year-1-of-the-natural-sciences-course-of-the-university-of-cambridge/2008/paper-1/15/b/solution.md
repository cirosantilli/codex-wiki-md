<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an integrable [discrete random variable](../../../../../discrete-random-variable.md), its [expectation](../../../../../expected-value-split.md) and [variance](../../../../../variance-split.md) are $\mu=\sum_{n\in\mathbb Z}np_n$ and $\sum_{n\in\mathbb Z}(n-\mu)^2p_n$, respectively. The first formula requires $\sum|n|p_n<\infty$ for a finite ordinary mean; the variance may be infinite. A [probability density function](../../../../../probability-density-function.md) gives $P(\alpha<Y<\beta)=\int_\alpha^\beta f(y)\,dy$.

Conditioning on $X$ and using [independence](../../../../../independent-random-variables.md) gives

$$
P(\alpha<X+Y<\beta)=\sum_{n\in\mathbb Z}p_n\int_{\alpha-n}^{\beta-n}f(y)\,dy
=\int_\alpha^\beta\sum_{n\in\mathbb Z}p_nf(z-n)\,dz.
$$

The interchange is justified by [Tonelli's theorem](../../../../../tonelli-theorem.md), since all integrands are nonnegative. Consequently $Z$ has an absolutely continuous distribution, with

$$
\boxed{g(z)=\sum_{n\in\mathbb Z}p_nf(z-n).}
$$

Its integral is $\sum_np_n=1$. This is the [convolution of independent random variables](../../../../../convolution-of-independent-random-variables.md), specifically a [Gaussian smoothing of an integer-valued distribution](../../../../../gaussian-smoothing-of-an-integer-valued-distribution.md) for the given normal density. The specified weights are normalized because $2(3/\pi^2)\sum_{n\geq1}n^{-2}=1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
