<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\lambda=\sum_i\lambda_i$, and suppose first that $\lambda>0$. Let $T_i$ be policy $i$'s aggregate, and $M_i$ the [moment-generating function](../../../../../../moment-generating-function.md) of its claim sizes. The [Poisson distribution](../../../../../../poisson-distribution.md) count has [probability generating function](../../../../../../probability-generating-function.md) $G_i(z)=\exp(\lambda_i(z-1))$, so the [random-sum transform identity](../../../../../../random-sum-transform-identity.md) and [independence](../../../../../../independent-random-variables.md) of the policies give

$$
M_T(u)=\prod_i\exp(\lambda_i(M_i(u)-1))
=\exp\left[\lambda\left(\sum_i\frac{\lambda_i}{\lambda}M_i(u)-1\right)\right].
$$

The expression in the weighted sum is the [moment-generating function](../../../../../../moment-generating-function.md) of a [mixture distribution](../../../../../../mixture-distribution.md) with claim [cumulative distribution function](../../../../../../cumulative-distribution-function.md)

$$
F_*(x)=\sum_i\frac{\lambda_i}{\lambda}F_i(x).
$$

Thus **the aggregate has a [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) with intensity $\lambda$ and severity law $F_*$**. This identification remains valid without positive [exponential moments](../../../../../../exponential-moment.md), using the same calculation for [Laplace transforms of nonnegative random variables](../../../../../../laplace-transform-of-a-nonnegative-random-variable.md) and their uniqueness. It is the [Poisson superposition of insurance portfolios](../../../../../../poisson-superposition-of-insurance-portfolios.md).

For common unit-rate [exponential distribution](../../../../../../exponential-distribution.md) severities, the merged count $K$ is [Poisson distributed](../../../../../../poisson-distribution.md) with mean $\lambda$. Because each severity is strictly positive, $T=0$ exactly when $K=0$, giving

$$
\boxed{a=e^{-\lambda}.}
$$

For $k\ge1$, the sum of $k$ unit-rate [exponential distribution](../../../../../../exponential-distribution.md) claims has [Erlang distribution](../../../../../../erlang-distribution.md) density $x^{k-1}e^{-x}/(k-1)!$. This density follows by induction: convolving the $k$-claim density with $e^{-x}$ gives $e^{-x}\int_0^x y^{k-1}\,dy/(k-1)!=e^{-x}x^k/k!$. Conditional on a positive aggregate, the count weights are

$$
\mathbb P(K=k\mid K>0)=\frac{e^{-\lambda}\lambda^k/k!}{1-e^{-\lambda}}=\frac{\lambda^k}{(e^\lambda-1)k!}.
$$

Therefore the [hurdle decomposition of a positive random sum](../../../../../../hurdle-decomposition-of-a-positive-random-sum.md) has positive-component [probability density function](../../../../../../probability-density-function.md)

$$
\boxed{\widetilde f_T(x)=\sum_{k=1}^{\infty}\frac{\lambda^k}{(e^\lambda-1)k!}\frac{x^{k-1}e^{-x}}{(k-1)!},\qquad x>0.}
$$

Each density integrates to one and the weights sum to one. Hence $F_T(x)=a+(1-a)\widetilde F_T(x)$ for $x\ge0$, where $\widetilde F_T$ is the conditional [cumulative distribution function](../../../../../../cumulative-distribution-function.md) given $T>0$. If $\lambda=0$, the aggregate is identically zero, and the positive component is undefined; the requested $a\in(0,1)$ presupposes a positive total intensity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
