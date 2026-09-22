<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditionally on $Y_1,\ldots,Y_m$, the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of $X^*$ is the weighted empirical distribution

$$
F_m^*(t)=\mathbb P(X^*\leq t\mid Y_1,\ldots,Y_m)
=\frac{m^{-1}\sum_{i=1}^m w(Y_i)\mathbf1_{\{Y_i\leq t\}}}
{m^{-1}\sum_{i=1}^m w(Y_i)},
\qquad w(y)=\frac{f(y)}{h(y)}.
$$

For fixed $t$, the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives, almost surely,

$$
\frac1m\sum_{i=1}^m w(Y_i)\mathbf1_{\{Y_i\leq t\}}
\longrightarrow
\int_{(-\infty,t]}f(y)\,dy=F(t),
$$

while

$$
\frac1m\sum_{i=1}^m w(Y_i)\longrightarrow\int f(y)\,dy=1.
$$

The ratio therefore converges almost surely to $F(t)$. This is precisely the claimed [convergence in distribution](../../../../../../convergence-in-distribution.md) of the [self-normalized importance sampling](../../../../../../self-normalized-importance-sampling.md) resample.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
