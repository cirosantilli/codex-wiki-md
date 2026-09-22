<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

For $0\leq u\leq1$, [independence](../../../../../independent-random-variables.md) gives

$$
P(U>u)=P(X>u,Y>u)=(1-u)^2.
$$

Thus $U$ has [probability density function](../../../../../probability-density-function.md) $f_U(u)=2(1-u)$, and its [expected value](../../../../../expected-value.md) is

$$
\boxed{\mathbb EU=\int_0^1 2u(1-u)\,du=\frac13.}
$$

Pointwise, $U+V=X+Y$ and $UV=XY$. By linearity of [expectation](../../../../../expected-value.md), $\mathbb EV=1-1/3=2/3$; by [independence](../../../../../independent-random-variables.md), $\mathbb E(UV)=\mathbb EX\,\mathbb EY=1/4$. Consequently the [covariance of two uniform order statistics](../../../../../covariance-of-two-uniform-order-statistics.md) is

$$
\boxed{\operatorname{Cov}(U,V)=\mathbb E(UV)-\mathbb EU\,\mathbb EV
=\frac14-\frac29=\frac1{36}.}
$$

The [order statistics](../../../../../order-statistic.md) are dependent despite the independence of the original observations.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
