<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [loss network](../../../../../../loss-network.md) models calls that require several resources simultaneously and are rejected if any required capacity is unavailable; rejected calls do not queue. For [fixed routing](../../../../../../fixed-routing.md), let $A_{jr}\in\mathbb Z_{\geq0}$ be the number of units of resource $j$ used by a call of type $r$, and let $C_j$ be its capacity. Independent [Poisson processes](../../../../../../poisson-process.md) supply type-$r$ calls at rate $\nu_r$, with independent holding times having an [exponential distribution](../../../../../../exponential-distribution.md) of mean $1/\mu_r$. Write $\alpha_r=\nu_r/\mu_r$ for the [offered traffic](../../../../../../offered-traffic.md), and

$$
\mathcal N(C)=\{n\in\mathbb Z_{\geq0}^R:An\leq C\}.
$$

Assume finitely many resources and call types, with every call using a resource, so this set is finite. The occupancy [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) has rates

$$
q(n,n+e_r)=\nu_r\,\mathbf1_{\{n+e_r\in\mathcal N(C)\}},\qquad
q(n,n-e_r)=\mu_r n_r.
$$

Its [stationary distribution](../../../../../../stationary-distribution.md) is

$$
\boxed{\pi(n)=\frac1{Z(C)}\prod_{r\in R}\frac{\alpha_r^{n_r}}{n_r!},\quad n\in\mathcal N(C),\qquad
Z(C)=\sum_{n\in\mathcal N(C)}\prod_r\frac{\alpha_r^{n_r}}{n_r!}.}
$$

Indeed, for each feasible upward transition,

$$
\pi(n)\nu_r=\pi(n+e_r)\mu_r(n_r+1),
$$

which is [detailed balance for a continuous-time Markov chain](../../../../../../detailed-balance-for-a-continuous-time-markov-chain.md). Thus this is a [reversible Markov chain](../../../../../../reversible-markov-chain.md). With positive arrival rates it is irreducible on $\mathcal N(C)$: departures reach the empty state, and any feasible state can be assembled by arrivals. Its [stationary distribution](../../../../../../stationary-distribution.md) is consequently unique.

The formula is a [product-form stationary distribution of a loss network](../../../../../../product-form-stationary-distribution-of-a-loss-network.md): equivalently, independent [Poisson random variables](../../../../../../poisson-distribution.md) of means $\alpha_r$ conditioned on $An\leq C$. The conditioning couples the occupancies, so the resources are generally not independent. By [Poisson arrivals see time averages](../../../../../../poisson-arrivals-see-time-averages.md), the acceptance probability for a type-$r$ arrival is

$$
\boxed{1-L_r=\frac{Z(C-A_{\cdot r})}{Z(C)},}
$$

because the prearrival state must leave $A_{jr}$ free units at each resource. Set the numerator to zero if its capacity vector has a negative entry. This exact formula is often expensive to evaluate, which motivates the [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md).

The same occupancy [stationary distribution](../../../../../../stationary-distribution.md) extends to independent general holding-time distributions with these means by [insensitivity of loss networks](../../../../../../insensitivity-of-loss-networks.md); the exponential assumption above makes the occupancy process itself a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) and permits the direct [detailed balance](../../../../../../detailed-balance.md) proof.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 213](../../../paper-213-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
