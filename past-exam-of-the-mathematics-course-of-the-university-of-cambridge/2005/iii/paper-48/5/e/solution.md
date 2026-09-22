<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let annual total loss be $L=\sum_{i=1}^{N_1}X_i$, with an empty sum equal to zero. The assumptions give a [compound Poisson distribution](../../../../../../compound-poisson-distribution.md). Conditioning on the count,

$$
\mathbb E[L\mid N_1]=N_1\mu,\qquad
\operatorname{Var}(L\mid N_1)=N_1\sigma^2.
$$

The [tower property](../../../../../../law-of-total-expectation.md) and total-[variance](../../../../../../variance-split.md) formula therefore give

$$
\boxed{\mathbb EL=\lambda\mu,\qquad\operatorname{Var}L=\lambda(\sigma^2+\mu^2).}
$$

The $\lambda\mu^2$ term is the extra uncertainty in the number of defaults. Replacing it by zero would incorrectly treat that count as deterministic.

For sufficiently many annual events and an adequate [normal approximation](../../../../../../normal-approximation.md), the [value at risk](../../../../../../value-at-risk.md) at confidence level $p$ is the [compound-Poisson annual loss quantile](../../../../../../compound-poisson-annual-loss-quantile.md)

$$
\boxed{\operatorname{VaR}_p(L)\approx\lambda\mu+z_p\sqrt{\lambda(\sigma^2+\mu^2)},\qquad z_p=\Phi^{-1}(p).}
$$

The supplied quantiles give $z_{0.90}=1.282$, $z_{0.95}=1.645$ and $z_{0.99}=2.326$. In particular a one-sided 95% annual loss quantile uses $1.645$, not the $1.96$ from the two-sided 95% rate interval. If the expected loss is covered separately, the approximate unexpected-loss reserve is the second term, rather than the full quantile.

Estimate the rate from a suitable historical count/exposure or gap sample, then insert $\widehat\lambda$ into the loss formula. The interval in part (d) measures rate-estimation uncertainty; for nonnegative loss [mean](../../../../../../expected-value.md) it can be propagated to lower and upper approximate quantiles because the displayed expression is increasing in $\lambda$. Severity parameters also require estimation, so the rate interval alone is not a [confidence interval](../../../../../../confidence-interval.md) accounting for every source of uncertainty.

[Mean](../../../../../../expected-value.md) and [variance](../../../../../../variance-split.md) do not determine the exact loss quantile. The actual distribution is

$$
\mathbb P(L\leq\ell)=e^{-\lambda}\sum_{n=0}^\infty\frac{\lambda^n}{n!}F_X^{*n}(\ell).
$$

For nonnegative losses it has a zero atom at least $e^{-\lambda}$, so if that mass exceeds $p$ its exact [value at risk](../../../../../../value-at-risk.md) is zero. With a small rate or a strongly skewed severity distribution, a [normal approximation](../../../../../../normal-approximation.md) can therefore be poor. A loan book with dependent defaults, rating migration or varying exposures also needs more than the constant-intensity independent-severity model. These are model qualifications, not deductions from the [credit rating](../../../../../../credit-rating.md) alone.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
