<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

Let $X_j$ be the number of failures in mix $j$. The total observed failures are $32+2(12)+3(2)+4(1)=66$ among $600$ blocks. Equal marginal failure [probabilities](../../../../../probability.md) give $E(X_j)=6p$, regardless of dependence within a mix. Thus the [unbiased estimator](../../../../../unbiased-estimator.md) based on [grouped Bernoulli failure counts](../../../../../grouped-bernoulli-failure-counts.md) is

$$
\boxed{\widehat p=\frac{\sum_{j=1}^{100}X_j}{600}=0.11.}
$$

For a conventional binomial [confidence interval](../../../../../confidence-interval.md), additionally assume independent block outcomes. Then the total $S$ has [binomial distribution](../../../../../binomial-distribution.md) $\operatorname{Bin}(600,p)$ and the estimated [standard error](../../../../../standard-error.md) is $\sqrt{\widehat p(1-\widehat p)/600}=0.01277$. The [normal approximation](../../../../../normal-approximation.md) gives the approximate 95 percent interval

$$
\boxed{0.11\pm1.96(0.01277)\simeq(0.0850,0.1350).}
$$

One can instead obtain an exact, generally conservative binomial interval by solving $P_{p_L}(S\ge66)=0.025$ and $P_{p_U}(S\le66)=0.025$ for the two endpoints. These equations invert binomial tail tests.

Equal marginal [probabilities](../../../../../probability.md) alone do not imply independent blocks. If the mixes are independent but blocks within a mix can be dependent, use the [sample variance](../../../../../sample-variance.md) of the 100 counts. Here $\sum X_j^2=114$ and $\overline X=0.66$, so $s_X^2=(114-100(0.66)^2)/99=0.7115$. The estimated [variance](../../../../../variance-split.md) of $\widehat p=\overline X/6$ is $s_X^2/(100\times36)$; its [standard error](../../../../../standard-error.md) is $0.01406$, giving the large-sample interval approximately $(0.0824,0.1376)$. If even between-mix independence is absent, no stated model justifies either numerical coverage claim. The estimate remains unbiased, but the uncertainty calculation needs its sampling assumptions.

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
