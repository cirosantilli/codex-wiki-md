<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Condition on the count and use the [independence of random variables](../../../../../../independent-random-variables.md) of the claim sizes. For $n\ge1$ their joint exponential transform factors, while for $n=0$ the empty sum contributes $1$. Consequently the [law of total expectation](../../../../../../law-of-total-expectation.md) gives

$$
\begin{aligned}
M_S(r)&=\sum_{n=0}^{\infty}\mathbb P(N=n)\,
\mathbb E\left[\exp\left(r\sum_{i=1}^{n}X_i\right)\right]\\
&=\sum_{n=0}^{\infty}\mathbb P(N=n)M_X(r)^n
=\boxed{G_N(M_X(r)).}
\end{aligned}
$$

This [random sum of independent claims](../../../../../../random-sum-of-independent-claims.md) transform uses both independence assumptions: the count must be independent of the entire claim-size sequence, and the sizes must be mutually independent with the same [probability distribution](../../../../../../probability-distribution.md). The [probability generating function](../../../../../../probability-generating-function.md) is interpreted through its defining nonnegative series. The identity holds as a finite [moment-generating function](../../../../../../moment-generating-function.md) wherever that series is finite; outside that domain the expectation and series can agree at $+\infty$. In particular a positive argument may take $M_X(r)$ beyond $1$, so finiteness does not follow merely from the usual unit-disk domain of a [probability generating function](../../../../../../probability-generating-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
