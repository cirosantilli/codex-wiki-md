<h1 id="3f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonnegative integer-valued [random variable](../../../../../../random-variable-split.md), the [probability generating function](../../../../../../probability-generating-function.md) is

$$
G_X(s)=\mathbb E[s^X]=\sum_{n=0}^{\infty}\mathbb P(X=n)s^n,
$$

initially for $|s|\le1$, with $0^0=1$. For the [Poisson distribution](../../../../../../poisson-distribution.md), insert its [probability mass function](../../../../../../probability-mass-function.md) and sum the exponential series:

$$
G_X(s)=e^{-\lambda}\sum_{n=0}^{\infty}\frac{(\lambda s)^n}{n!}.
$$

Thus

$$
\boxed{G_X(s)=e^{\lambda(s-1)}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3F](../../3f.md)
3. [Section I](../../section-i.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
