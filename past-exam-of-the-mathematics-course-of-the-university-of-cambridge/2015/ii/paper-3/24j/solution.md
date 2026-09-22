<h1 id="24j/solution">Solution</h1>

↑ **Parent:** [24J](../24j.md)

An [estimator](../../../../../estimator.md) $\hat\theta_n$ is [consistent](../../../../../consistency-statistics.md) if, for every parameter value $\theta$ and every $\epsilon>0$, $\mathbb P_\theta(|\hat\theta_n-\theta|>\epsilon)\to0$.

For the proposed root criterion, fix $\epsilon>0$. [Convergence in probability](../../../../../convergence-in-probability.md) at the two points gives

$$
\mathbb P(S_n(\theta_0-\epsilon)<0<S_n(\theta_0+\epsilon))\to1.
$$

On this event the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives a zero between the two points. Since the zero is unique, it is $\hat\theta_n$. Therefore **$\boxed{\hat\theta_n\xrightarrow{P}\theta_0}$**, without needing uniform convergence of $S_n$.

For independent $N(\theta_0,1)$ observations, the [log-likelihood](../../../../../log-likelihood.md) has derivative $n(\bar X_n-\theta)$ and negative second derivative $-n$. Its unique maximizer is $\hat\theta_n=\bar X_n$. Apply the criterion to $S_n(\theta)=\theta-\bar X_n$: the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives the limit $S(\theta)=\theta-\theta_0$, with the required signs. Hence the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is consistent.

In the bivariate model the log-likelihood, apart from constants, is

$$
\ell(\mu,\sigma^2)=-n\log\sigma^2-\frac1{2\sigma^2}\sum_{i=1}^n[(X_{1i}-\mu_i)^2+(X_{2i}-\mu_i)^2].
$$

Minimizing each squared pair gives $\boxed{\hat\mu_i=(X_{1i}+X_{2i})/2}$. Maximizing the resulting likelihood in the variance gives

$$
\boxed{\hat\sigma^2=\frac1n\sum_{i=1}^ns_i^2=\frac1{4n}\sum_{i=1}^n(X_{1i}-X_{2i})^2.}
$$

Each difference is $N(0,2\sigma^2)$, independently of the others and independently of its unknown mean parameter. Thus the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives $\hat\sigma^2\to\sigma^2/2$ in probability, not $\sigma^2$. This is the [Neyman-Scott incidental parameter problem](../../../../../neyman-scott-incidental-parameter-problem.md): the number of nuisance means grows with the sample size, but each mean is estimated from only two observations. The usual fixed-dimensional likelihood consistency theory therefore does not apply. The corrected estimator $2\hat\sigma^2$ is consistent.

## ↑ Ancestors (10)

1. [24J](../24j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
