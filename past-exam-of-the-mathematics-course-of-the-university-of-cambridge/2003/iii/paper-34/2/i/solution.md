<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [loss network](../../../../../../loss-network.md) admits a call only when all the resources it requires have available capacity. Calls which fail admission disappear rather than waiting. Under [fixed routing](../../../../../../fixed-routing.md), class $r$ has a fixed nonzero integer resource-requirement vector $a_r$, [Poisson process](../../../../../../poisson-process.md) rate $\nu_r$, and independent [exponential distributions](../../../../../../exponential-distribution.md) with parameter $\mu_r$. Let $A$ have columns $a_r$ and let $C$ be the resource-capacity vector. The feasible call counts are

$$
\mathcal S=\{n\in\mathbb Z_+^R:An\leq C\}.
$$

Write $\alpha_r=\nu_r/\mu_r$ for the [offered load](../../../../../../offered-traffic.md). On $\mathcal S$, the Markov [transition rates](../../../../../../transition-intensity.md) are $q(n,n+e_r)=\nu_r$ if the new state is feasible, and $q(n,n-e_r)=\mu_rn_r$.

The [product-form stationary distribution of a loss network](../../../../../../product-form-stationary-distribution-of-a-loss-network.md) is

$$
\boxed{\pi(n)=Z(C)^{-1}\prod_r\frac{\alpha_r^{n_r}}{n_r!},\qquad
Z(C)=\sum_{n\in\mathcal S}\prod_r\frac{\alpha_r^{n_r}}{n_r!}.}
$$

Indeed, whenever $n+e_r$ is feasible,

$$
\pi(n)\nu_r=\pi(n+e_r)\mu_r(n_r+1).
$$

These pairwise equalities give [detailed balance](../../../../../../detailed-balance.md), including the truncated boundary: there is no transition to an infeasible state in either direction. The finite reachable chain is irreducible under positive arrival and holding rates, so this is its unique [stationary distribution](../../../../../../stationary-distribution.md). It can also be viewed as independent Poisson offered populations conditioned on all [capacity constraints](../../../../../../capacity-constraint.md). Conditioning usually makes the actual resource occupancies dependent.

An arriving call of class $r$ sees this [stationary distribution](../../../../../../stationary-distribution.md) by [Poisson arrivals see time averages](../../../../../../poisson-arrivals-see-time-averages.md). Its acceptance probability is

$$
P_r=\sum_{n\in\mathcal S:\,A(n+e_r)\leq C}\pi(n)
=\frac{Z(C-a_r)}{Z(C)},
$$

where a [partition function](../../../../../../canonical-partition-function.md) with a negative capacity is zero. This is the [blocking partition ratio for a loss network](../../../../../../blocking-partition-ratio-for-a-loss-network.md). Thus its blocking probability is $1-P_r$, admitted arrival rate is $\nu_rP_r$, and mean number present is $\alpha_rP_r$, by balancing admitted births with departures. With a single unit-demand resource, the formula reduces to the [Erlang loss formula](../../../../../../erlang-loss-formula.md)

$$
E(a,C)=\frac{a^C/C!}{\sum_{k=0}^Ca^k/k!}.
$$

The stationary count law is also insensitive to the shape of independent holding-time distributions in the standard fixed-routing model when their means are unchanged. With nonexponential holding times, counts alone need not be Markov; residual holding times are included in the state for this insensitivity assertion. State-dependent admission controls and [alternative routing](../../../../../../alternative-routing.md) do not automatically preserve the same simple product form.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
