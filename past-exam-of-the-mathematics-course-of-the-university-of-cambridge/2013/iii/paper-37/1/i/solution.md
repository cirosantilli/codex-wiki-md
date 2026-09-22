<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [loss network](../../../../../../loss-network.md) models calls that need several resources simultaneously and are rejected, rather than queued, when insufficient capacity remains. Take finite resource and route sets. Let $A_{jr}\geq0$ be the integer amount of resource $j$ required by a route-$r$ call, $C_j$ its capacity, and

$$
\mathcal S=\{n\in\mathbb Z_+^R:An\leq C\}.
$$

Under [fixed routing](../../../../../../fixed-routing.md), each arriving call has a predetermined resource requirement. Take independent [Poisson processes](../../../../../../poisson-process.md) of rates $\nu_r$ and independent holding times with [exponential distribution](../../../../../../exponential-distribution.md) of rates $\mu_r$. A feasible arrival changes $n$ to $n+e_r$ at rate $\nu_r$; a departure changes it to $n-e_r$ at rate $\mu_rn_r$. Put $\rho_r=\nu_r/\mu_r$ and assume each route uses a finite positive-capacity resource, so the state space is finite.

The [product-form stationary distribution of a loss network](../../../../../../product-form-stationary-distribution-of-a-loss-network.md) is

$$
\boxed{\pi(n)=\frac1{G(C)}\prod_r\frac{\rho_r^{n_r}}{n_r!},\qquad
G(C)=\sum_{n\in\mathcal S}\prod_r\frac{\rho_r^{n_r}}{n_r!}}.
$$

For any feasible adjacent pair,

$$
\pi(n)\nu_r=\pi(n+e_r)\mu_r(n_r+1).
$$

These [detailed balance equations](../../../../../../detailed-balance.md) prove stationarity and make the process a [reversible Markov chain](../../../../../../reversible-markov-chain.md). Equivalently, [Independent random variables](../../../../../../independent-random-variables.md) with [Poisson distributions](../../../../../../poisson-distribution.md) of means $\rho_r$ are conditioned on satisfying the joint capacity constraints. The conditioning makes resource occupancies dependent even though the unconstrained counts are independent.

By [Poisson arrivals see time averages](../../../../../../poisson-arrivals-see-time-averages.md), a route-$r$ arrival sees acceptance [probability](../../../../../../probability.md) $G(C-A_r)/G(C)$, interpreting the numerator as zero for a negative capacity. Hence its blocking [probability](../../../../../../probability.md) is $1-G(C-A_r)/G(C)$ and the [expected value](../../../../../../expected-value.md) of its number in service is $\rho_rG(C-A_r)/G(C)$. This connects a stationary occupancy law to observable rejection and carried traffic.

The [insensitivity of loss networks](../../../../../../insensitivity-of-loss-networks.md) extends this occupancy formula to independent general holding-time distributions with the same [expected values](../../../../../../expected-value.md), under the usual fixed resource requirements and admission rule. Counts alone then need not be a [Markov chain](../../../../../../markov-chain.md); residual holding times belong in a Markov description. The invariant occupancy formula survives. This is useful because detailed call-duration distributions can be difficult to estimate, while their means are much easier to measure.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
