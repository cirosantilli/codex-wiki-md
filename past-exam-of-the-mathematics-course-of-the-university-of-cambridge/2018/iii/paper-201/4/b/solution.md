<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For any finite list $t_1,\ldots,t_k\in[0,1]$, the [random vector](../../../../../../random-vector.md) $(U_{t_1},\ldots,U_{t_k},B_1)$ has a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md), since it is a linear image of a vector of [Brownian motion](../../../../../../brownian-motion-split.md) coordinates. The [Brownian covariance kernel](../../../../../../brownian-covariance-kernel.md) and [linearity of covariance](../../../../../../linearity-of-covariance.md) give

$$
\operatorname{Cov}(U_t,B_1)=\operatorname{Cov}(B_t,B_1)-t\operatorname{Var}(B_1)=t-t=0.
$$

The [independence of uncorrelated jointly normal variables](../../../../../../independence-of-uncorrelated-jointly-normal-variables.md) implies that $(U_{t_1},\ldots,U_{t_k})$ is [independent](../../../../../../independent-random-variables.md) of $B_1$. Extending from finite-coordinate cylinder [events](../../../../../../event.md) by [independence extended from generating pi-systems](../../../../../../independence-extended-from-generating-pi-systems.md) proves

$$
\boxed{\sigma(U_t:0\leq t\leq1)\ \text{is independent of}\ \sigma(B_1).}
$$

Thus **the [Brownian bridge](../../../../../../brownian-bridge.md) is [independent](../../../../../../independent-random-variables.md) of its endpoint**. Its [covariance kernel](../../../../../../covariance-kernel.md) is $\operatorname{Cov}(U_s,U_t)=\min(s,t)-st$, confirming that $U$ is the standard [Brownian bridge](../../../../../../brownian-bridge.md). This is the [Brownian bridge independence from its endpoint](../../../../../../brownian-bridge-independence-from-its-endpoint.md) property.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
