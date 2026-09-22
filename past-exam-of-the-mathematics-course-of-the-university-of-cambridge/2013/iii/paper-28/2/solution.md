<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an [aggregate claims model](../../../../../aggregate-claims-model.md), let $X$ denote one claim size, with [expected value](../../../../../expected-value.md) $\mu$ and [variance](../../../../../variance-split.md) $\sigma^2$. The total $S$ is zero when the claim count is zero. Given $N=n$, [independence](../../../../../independent-random-variables.md) gives

$$
\mathbb E(S\mid N)=N\mu,\qquad \operatorname{Var}(S\mid N)=N\sigma^2.
$$

The [law of total expectation](../../../../../law-of-total-expectation.md) and [law of total variance](../../../../../law-of-total-variance.md), together with $\mathbb EN=\operatorname{Var}(N)=\lambda$ for a [Poisson distribution](../../../../../poisson-distribution.md), imply

$$
\boxed{\mathbb ES=\lambda\mu,\qquad
\operatorname{Var}(S)=\lambda(\sigma^2+\mu^2)=\lambda\mathbb EX^2.}
$$

The raw second moment appears because the random count itself contributes $\lambda\mu^2$ to the [variance](../../../../../variance-split.md).

Conditional on $N$, the [moment-generating function](../../../../../moment-generating-function.md) of the sum is $M_X(t)^N$. Averaging with the [Poisson distribution](../../../../../poisson-distribution.md) therefore gives the [compound Poisson distribution](../../../../../compound-poisson-distribution.md) transform

$$
\boxed{M_S(t)=\exp\{\lambda(M_X(t)-1)\}.}
$$

This is valid wherever $M_X(t)$ is finite. Finite first and second moments alone do not ensure positive exponential moments; for positive claims the corresponding [Laplace transform](../../../../../laplace-transform.md) always exists.

For the independent portfolios put $\Lambda=\lambda_1+\lambda_2>0$ and $w_i=\lambda_i/\Lambda$. Their [Poisson distribution](../../../../../poisson-distribution.md) counts add to a [Poisson distribution](../../../../../poisson-distribution.md) with parameter $\Lambda$. By [Poisson-multinomial conditioning](../../../../../poisson-multinomial-conditioning.md), conditional on the total count $n$ the first risk count has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,w_1$, and the second is the remaining count. Thus one can generate the same total loss by drawing $n$ independent risk labels with these weights, then drawing each claim from its label's law. The merged severity has [mixture distribution](../../../../../mixture-distribution.md)

$$
f(x)=w_1f_1(x)+w_2f_2(x).
$$

It follows that $T$ has a [compound Poisson distribution](../../../../../compound-poisson-distribution.md) with count parameter $\Lambda$ and this severity law. This is the fixed-year version of [Poisson superposition of insurance portfolios](../../../../../poisson-superposition-of-insurance-portfolios.md). Its [expected value](../../../../../expected-value.md) and [variance](../../../../../variance-split.md) are

$$
\boxed{\mathbb ET=\lambda_1\mu_1+\lambda_2\mu_2,\qquad
\operatorname{Var}(T)=\sum_{i=1}^2\lambda_i(\sigma_i^2+\mu_i^2).}
$$

Alternatively, multiplying the two independent aggregate [Laplace transforms](../../../../../laplace-transform.md) yields $\exp\{\Lambda(w_1M_{X_1}(t)+w_2M_{X_2}(t)-1)\}$ wherever finite, confirming the same [compound Poisson distribution](../../../../../compound-poisson-distribution.md).

For the [retained compound Poisson aggregate](../../../../../retained-compound-poisson-aggregate.md) under per-claim [reinsurance](../../../../../reinsurance.md), replace each claim $X$ by its retained payment $g(X)$. Assume the retention is measurable, with $0\le g(x)\le x$ as usual. The count parameter remains $\Lambda$, and the severity law is the [pushforward measure](../../../../../pushforward-measure.md) of the mixture severity under $g$. Thus the [retained compound Poisson aggregate](../../../../../retained-compound-poisson-aggregate.md) $T_I$ has a [compound Poisson distribution](../../../../../compound-poisson-distribution.md) with that transformed severity and

$$
\boxed{\mathbb ET_I=\sum_{i=1}^2\lambda_i\mathbb E g(X_i),\qquad
\operatorname{Var}(T_I)=\sum_{i=1}^2\lambda_i\mathbb E[g(X_i)^2].}
$$

Its [moment-generating function](../../../../../moment-generating-function.md) is $\exp\{\sum_i\lambda_i(M_{g(X_i)}(t)-1)\}$ on its finite domain. For a general retention $g$, zero retained payments can occur and are allowed as compound-Poisson marks; they may equivalently be removed by [Poisson thinning](../../../../../poisson-thinning.md). The two specified contracts retain strictly positive payments for strictly positive claims.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
