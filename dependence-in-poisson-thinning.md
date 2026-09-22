# Dependence in Poisson thinning

↑ **Parent:** [Poisson thinning](poisson-thinning.md)

Independent marking is the hypothesis that guarantees the [Poisson thinning theorem](poisson-thinning-theorem.md). Equal marginal retention [probabilities](probability.md) do not guarantee it. Consider one [Bernoulli random variable](bernoulli-distribution.md) $B$ with success [probability](probability.md) $p\in(0,1)$, independent of a [Poisson process](poisson-process-split.md), and retain every arrival when $B=1$ and none when $B=0$. Each arrival is retained with [probability](probability.md) $p$, but the marks share the same coin. In an interval whose original count has [Poisson distribution](poisson-distribution.md) of [mean](expected-value-split.md) $m>0$, the retained count is $R=BN$ and the rejected count is $D=(1-B)N$, so

$$
\mathbb E[R]=pm,\qquad \operatorname{Var}(R)=pm+p(1-p)m^2,\qquad \operatorname{Cov}(R,D)=-p(1-p)m^2.
$$

The extra [variance](variance-split.md) shows that $R$ is not [Poisson distributed](poisson-distribution.md); the negative [covariance](covariance.md) proves dependence. Its no-arrival [probability](probability.md) is $1-p+pe^{-m}$, rather than $e^{-pm}$. For the toy values $p=1/2,m=2$, both rules have retained [mean](expected-value-split.md) $1$, but the common-coin rule has [variance](variance-split.md) $2$ and no-arrival [probability](probability.md) $(1+e^{-2})/2\approx0.567668$, compared with [variance](variance-split.md) $1$ and no-arrival [probability](probability.md) $e^{-1}\approx0.367879$ for independent marking. These formulas follow by conditioning on $B$ and using the [law of total variance](law-of-total-variance.md).

An arrival-dependent or adversarial retention rule can change the law just as strongly. Keeping every second arrival gives $R_t=\lfloor N_t/2\rfloor$. Its successive retained gaps are sums of two [independent](independent-random-variables.md) [exponential random variables](exponential-distribution.md), hence have the [Erlang distribution](erlang-distribution.md) of shape two and rate $\lambda$, not an [exponential distribution](exponential-distribution.md). The resulting [renewal process](renewal-process.md) and its count [variance](variance-split.md) are analyzed in [Every second Poisson arrival has underdispersed counts](every-second-poisson-arrival-has-underdispersed-counts.md), and the two dependent streams in [alternating split of a Poisson process](alternating-split-of-a-poisson-process.md). As an even more restrictive rule, keeping only the first arrival ever gives $R_t=\mathbf1_{\{N_t\geq1\}}$, a [Bernoulli distribution](bernoulli-distribution.md) at each $t>0$, so it cannot have a positive-mean [Poisson distribution](poisson-distribution.md). A thinning rule must specify how decisions depend on arrivals and on one another; the independent-marking conclusion cannot be applied automatically to arbitrary deletion.

## ↑ Ancestors (7)

1. [Poisson thinning](poisson-thinning.md)
2. [Poisson process](poisson-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
