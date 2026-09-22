<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the rate convention for the [exponential distribution](../../../../../../exponential-distribution.md). By [convolution of independent random variables](../../../../../../convolution-of-independent-random-variables.md), the [probability density function](../../../../../../probability-density-function.md) of $S=X+Y$ is, for $s\geq0$,

$$
f_S(s)=\int_0^s\lambda e^{-\lambda x}\mu e^{-\mu(s-x)}\,dx
=\boxed{\frac{\lambda\mu}{\mu-\lambda}
\left(e^{-\lambda s}-e^{-\mu s}\right)}.
$$

It is zero for $s<0$. The expression is nonnegative whichever rate is larger, and defines a two-stage [hypoexponential distribution](../../../../../../hypoexponential-distribution.md). As a check, its limit as $\mu\to\lambda$ is $\lambda^2s e^{-\lambda s}$, the shape-two [gamma distribution](../../../../../../gamma-distribution.md).

For $M=\min\{X,Y\}$, [independence](../../../../../../independent-random-variables.md) gives the [survival function](../../../../../../survival-function.md) $\mathbb P(M>s)=e^{-\lambda s}e^{-\mu s}$ for $s\geq0$. Differentiating its complement gives

$$
\boxed{f_M(s)=(\lambda+\mu)e^{-(\lambda+\mu)s}\mathbf1_{\{s\geq0\}}.}
$$

Thus the minimum has an [exponential distribution](../../../../../../exponential-distribution.md) whose rate is the sum of the rates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
