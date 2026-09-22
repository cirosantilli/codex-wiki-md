<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the shape-rate convention for the [gamma distribution](../../../../../gamma-distribution.md) $\theta\sim\operatorname{Gamma}(\alpha,\beta)$, with [prior distribution](../../../../../prior-probability.md) [probability density function](../../../../../probability-density-function.md) proportional to $\theta^{\alpha-1}e^{-\beta\theta}$. The observations are [independent](../../../../../independent-random-variables.md) conditional on the common parameter $\theta$. Unconditionally a common nondegenerate [prior distribution](../../../../../prior-probability.md) induces [covariance](../../../../../covariance.md) $\alpha/\beta^2$ between distinct observations, so the [Bayesian inference](../../../../../bayesian-statistics.md) model requires conditional [independence](../../../../../independent-random-variables.md).

For unit-exposure counts, the [likelihood](../../../../../likelihood-function.md) is proportional to $\theta^{\sum_i x_i}e^{-n\theta}$. Multiplying by the [prior distribution](../../../../../prior-probability.md) gives

$$
\theta\mid\mathbf x\sim\operatorname{Gamma}\left(\alpha+\sum_{i=1}^n x_i,\ \beta+n\right).
$$

The future count has [conditional expectation](../../../../../conditional-expectation.md) $\theta$, so [posterior distribution](../../../../../bayesian-posterior.md) averaging gives

$$
\boxed{\mathbb E[X_{n+1}\mid\mathbf x]
=\frac{\alpha+\sum_i x_i}{\beta+n}
=\frac{n}{n+\beta}\overline x+\frac{\beta}{n+\beta}\frac\alpha\beta.}
$$

This is an exact [Bayesian credibility](../../../../../bayesian-credibility.md) estimate, with [credibility factor](../../../../../credibility-factor.md) $Z=n/(n+\beta)$ and collective [mean](../../../../../expected-value.md) $\alpha/\beta$.

For the [insurance exposure](../../../../../insurance-exposure.md) and [claims inflation](../../../../../claims-inflation.md) calculation put $c_j=c(1+r)^j$, assuming $c>0$, $1+r>0$ and positive policy counts $n_j$. Let $K_j$ be the total claim count in year $j$. [Conditional independence](../../../../../conditional-independence.md) of the policy counts gives $K_j\mid\theta\sim\operatorname{Pois}(n_j\theta)$, and the observed average amount satisfies

$$
Y_j=\frac{c_jK_j}{n_j},\qquad k_j=\frac{n_jy_j}{c_j}.
$$

For possible observations, the recovered $k_j$ are nonnegative integers. If they are not, the data have zero [likelihood](../../../../../likelihood-function.md) under the model and no conditional [posterior distribution](../../../../../bayesian-posterior.md) is defined for those impossible values.

Write $W=\sum_{j=1}^n n_j$ and $K=\sum_{j=1}^n k_j$. Since $Y_j$ and $K_j$ determine each other, conditioning on the observed average amounts is equivalent to conditioning on these counts. The [independent](../../../../../independent-random-variables.md) yearly count [likelihood](../../../../../likelihood-function.md) is

$$
\prod_{j=1}^n e^{-n_j\theta}\frac{(n_j\theta)^{k_j}}{k_j!}
\propto\theta^K e^{-W\theta}.
$$

The [Poisson-gamma conjugacy with unequal exposures](../../../../../poisson-gamma-conjugacy-with-unequal-exposures.md) therefore gives

$$
\boxed{\theta\mid\mathbf y\sim\operatorname{Gamma}(\alpha+K,\beta+W).}
$$

For the future year, $\mathbb E[Y_{n+1}\mid\theta]=c_{n+1}\theta$; the number of future policies cancels because $Y_{n+1}$ is a per-policy average. Hence

$$
\boxed{\mathbb E[Y_{n+1}\mid\mathbf y]
=c_{n+1}\frac{\alpha+K}{\beta+W}
=Z\,m(\mathbf y)+(1-Z)m,}
$$

with

$$
\boxed{\begin{aligned}
Z&=\frac{W}{W+\beta},\\
m&=c(1+r)^{n+1}\frac\alpha\beta,\\
m(\mathbf y)&=c_{n+1}\frac KW
=\frac1W\sum_{j=1}^n n_j(1+r)^{n+1-j}y_j.
\end{aligned}}
$$

The collective [mean](../../../../../expected-value.md) $m$ is the [prior distribution](../../../../../prior-probability.md) expected claim amount per policy in the future year's monetary units. The experience [mean](../../../../../expected-value.md) $m(\mathbf y)$ first inflates each past per-policy amount to that same future year and then averages with policy-exposure weights. Equivalently, it estimates annual claim frequency by total observed claims divided by total past [insurance exposure](../../../../../insurance-exposure.md) and converts that frequency to the future claim cost. This is [inflation-adjusted Poisson-gamma credibility](../../../../../inflation-adjusted-poisson-gamma-credibility.md).

For fixed [prior distribution](../../../../../prior-probability.md) parameters, $Z$ increases strictly with total past [insurance exposure](../../../../../insurance-exposure.md): $dZ/dW=\beta/(W+\beta)^2>0$, and **$Z\to1$ as $W\to\infty$**. The [prior distribution](../../../../../prior-probability.md) weight decreases to zero; $\beta$ acts as equivalent [prior distribution](../../../../../prior-probability.md) [insurance exposure](../../../../../insurance-exposure.md). With no past [insurance exposure](../../../../../insurance-exposure.md) the appropriate weight is zero and the prediction is $m$, without defining an empirical experience [mean](../../../../../expected-value.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
