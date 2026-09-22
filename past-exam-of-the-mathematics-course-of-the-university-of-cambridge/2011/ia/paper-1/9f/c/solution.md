<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First, for $0<x<1$, the [derivative](../../../../../../derivative.md) of $h(x)=\log(1-x)+x$ is $-x/(1-x)<0$, while $h(0)=0$. Hence $\log(1-x)<-x$.

Choose $N>c$ large enough that the given ratio bound holds for every $n\ge N$. Positivity permits taking [logarithms](../../../../../../logarithm.md), and the preceding inequality gives

$$
\log a_{k+1}-\log a_k\le\log(1-c/k)<-c/k.
$$

Summing, and using the [integral test for convergence](../../../../../../integral-test-for-convergence.md) from part (b), gives for $n>N$

$$
\log a_n\le\log a_N-c\sum_{k=N}^{n-1}\frac1k
\le\log a_N-c\log(n/N).
$$

Thus $a_n\le a_NN^c n^{-c}$. Since $c>1$, the [P-series](../../../../../../p-series.md) $\sum n^{-c}$ converges, so the [comparison test for series](../../../../../../comparison-test-for-series.md) proves

$$
\boxed{\sum_{n=1}^\infty a_n<\infty.}
$$

The finitely many initial terms do not affect convergence. This [power-law comparison from a refined ratio bound](../../../../../../power-law-comparison-from-a-refined-ratio-bound.md) supplies information when the ordinary [ratio test](../../../../../../ratio-test.md) can be inconclusive.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
