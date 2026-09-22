<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The exact condition is again **$\sum_ka_k^2<\infty$**, with the terminal almost-sure limit used to define $M_T$ when $T=\infty$. In that case $\sup_n\mathbb EM_n^2<\infty$, and

$$
\mathbb E[|M_n|;|M_n|>R]\leq\frac{\mathbb EM_n^2}{R}
$$

proves [uniform integrability](../../../../../../uniform-integrability.md). The preceding unbounded [optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) argument yields $\boxed{\mathbb E M_T=0}$.

For necessity, suppose $v_n\to\infty$. For every fixed $R>0$, the [normal distribution](../../../../../../normal-distribution.md) of $M_n$ gives $\mathbb P(M_n\geq R)\to1/2$. Hence $\mathbb P(\sup_nM_n\geq R)\geq1/2$, and intersecting over positive integer $R$ shows $\mathbb P(\sup_nM_n=\infty)\geq1/2$. Unboundedness above is unchanged by altering finitely many of the [independent](../../../../../../independent-random-variables.md) $Z_k$, because that changes all sufficiently late sums by one finite constant. It is therefore a [tail event](../../../../../../tail-event.md); the [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) makes its probability one. Consequently $T<\infty$ [almost surely](../../../../../../almost-sure-convergence.md) and $M_T\geq1$. Its [expectation](../../../../../../expected-value.md) is at least one, possibly infinite, and cannot equal zero. This proves the necessity assertion in [threshold stopping of an independent Gaussian series](../../../../../../threshold-stopping-of-an-independent-gaussian-series.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
