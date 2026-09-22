<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

One sufficient [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md) [statistical consistency](../../../../../consistency-statistics.md) theorem is the following. Let the observations be [independent random variables](../../../../../independent-random-variables.md) with a common density $f_\theta$ relative to a fixed measure, let $\Theta$ be a compact metric parameter set containing the true value $\theta_0$, and suppose that the expected [log-likelihood](../../../../../log-likelihood.md)

$$
m(\theta)=\mathbb E_{\theta_0}\log f_\theta(Y_1)
$$

is finite, continuous, and uniquely maximized at $\theta_0$. Assume also the [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md)

$$
\sup_{\theta\in\Theta}\left|\frac1n\sum_{i=1}^n\log f_\theta(Y_i)-m(\theta)\right|\xrightarrow{\mathbb P}0,
$$

and assume that a measurable global [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) exists. Then **every such maximum-likelihood estimator converges in probability to the true parameter**. A useful sufficient condition for this [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md) is almost-sure continuity of $\theta\mapsto\log f_\theta(Y_1)$ on the compact parameter set and an integrable envelope $\sup_\theta|\log f_\theta(Y_1)|\le M(Y_1)$, $\mathbb E_{\theta_0}M(Y_1)<\infty$. Under these conditions, [identifiability](../../../../../identifiability.md) supplies uniqueness through the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) identity

$$
m(\theta_0)-m(\theta)=D_{\mathrm{KL}}(f_{\theta_0}\|f_\theta)\ge0,
$$

with equality only at $\theta=\theta_0$.

To see the [statistical consistency](../../../../../consistency-statistics.md) conclusion, fix $\varepsilon>0$. Compactness and the unique maximum give a strictly positive separation gap

$$
\delta_\varepsilon=m(\theta_0)-\sup_{d(\theta,\theta_0)\ge\varepsilon}m(\theta)>0
$$

whenever the set outside the neighbourhood is nonempty. If $\Delta_n$ denotes the supremum discrepancy in the [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md), maximization of the empirical [log-likelihood](../../../../../log-likelihood.md) yields

$$
0\le m(\theta_0)-m(\widehat\theta_n)\le2\Delta_n.
$$

Hence the probability of $d(\widehat\theta_n,\theta_0)\ge\varepsilon$ is at most $\mathbb P(2\Delta_n\ge\delta_\varepsilon)$, which tends to zero. This is the [argmin consistency under uniform convergence in probability](../../../../../argmin-consistency-under-uniform-convergence-in-probability.md) argument applied to the negative [log-likelihood](../../../../../log-likelihood.md). These are sufficient conditions, not necessary ones; parameter-dependent support can require a direct argument, and independent observations need not have a common distribution in other models.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
