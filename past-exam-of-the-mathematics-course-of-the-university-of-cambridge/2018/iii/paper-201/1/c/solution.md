<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $M_n=\sum_{j=0}^nX_j$ and $\mathcal F_n=\sigma(X_0,\ldots,X_n)$. The [independence](../../../../../../independent-random-variables.md) and zero [expected values](../../../../../../expected-value.md) give $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$, so $(M_n)$ is a [martingale](../../../../../../martingale-split.md). The [variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md) gives

$$
\mathbb E[M_n^2]=\sum_{j=0}^n\mathbb E[X_j^2]\leq V:=\sum_{j=0}^\infty\mathbb E[X_j^2]<\infty.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) implies $\sup_n\mathbb E|M_n|\leq\sqrt V$. Applying the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) from (b),

$$
\boxed{\sum_{j=0}^{\infty}X_j\ \text{converges almost surely}.}
$$

In fact the [L2 martingale convergence theorem](../../../../../../l2-martingale-convergence-theorem.md) also gives [convergence in L2](../../../../../../convergence-in-l2.md). Independently, for $n>m$ the same [variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md) yields $\mathbb E|M_n-M_m|^2=\sum_{j=m+1}^n\mathbb E[X_j^2]\to0$, confirming that the partial sums form a [Cauchy sequence](../../../../../../cauchy-sequence.md) in $L^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
