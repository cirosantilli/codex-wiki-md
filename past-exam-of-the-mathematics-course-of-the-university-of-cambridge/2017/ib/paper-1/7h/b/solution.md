<h1 id="7h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $\mathbb P(X_1=0)=e^{-\lambda}$, the indicator $Y$ is an [unbiased estimator](../../../../../../unbiased-estimator.md) of $\theta$. The joint [probability mass function](../../../../../../probability-mass-function.md) is

$$
p_\lambda(x_1,\ldots,x_n)=e^{-n\lambda}\frac{\lambda^{\sum_i x_i}}{\prod_i x_i!}.
$$

The [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) therefore makes $T=\sum_iX_i$ a [sufficient statistic](../../../../../../sufficient-statistic.md). More explicitly, conditioning on $T=t$ gives a [multinomial distribution](../../../../../../multinomial-distribution.md) with $t$ trials and cell probabilities $1/n$, so $X_1\mid T=t$ has the [binomial distribution](../../../../../../binomial-distribution.md) $\operatorname{Bin}(t,1/n)$. Consequently conditioning by the [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md) gives

$$
\boxed{\mathbb E[Y\mid T]=\left(1-\frac1n\right)^T}.
$$

For $n=1$, interpret the value at $T=0$ as $1$ and at $T>0$ as $0$; thus the same expression uses $0^0=1$ in this probability convention. For $\lambda=0$ all observations and $T$ are zero almost surely. For $n>1$ and $\lambda>0$, the reduction in [variance](../../../../../../variance-split.md) is strict: given $T=1$, the event $X_1=0$ still has a nondegenerate conditional probability. Directly, using the [probability generating function](../../../../../../probability-generating-function.md) of $T\sim\operatorname{Poisson}(n\lambda)$, the new [variance](../../../../../../variance-split.md) is $e^{-2\lambda}(e^{\lambda/n}-1)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7H](../../7h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
