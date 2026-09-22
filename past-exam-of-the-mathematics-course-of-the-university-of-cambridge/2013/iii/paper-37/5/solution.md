<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $x_r$ be the rate of each individual flow on route $r$, so its aggregate rate is $w_r=n_rx_r$. The feasible allocations satisfy $\sum_{r:j\in r}n_rx_r\leq C_j$. An allocation has [proportional fairness](../../../../../proportional-fairness.md) if, for every feasible $\widetilde x$,

$$
\boxed{\sum_{r:n_r>0}n_r\frac{\widetilde x_r-x_r}{x_r}\leq0}.
$$

Equivalently it maximizes $\sum_{r:n_r>0}n_r\log x_r$ over positive active-route rates. This is the [first-order optimality condition](../../../../../first-order-optimality-condition.md) for a concave objective on a [convex set](../../../../../convex-set.md). Rates for absent flows can be set to zero.

For the [linear flow network](../../../../../linear-flow-network.md), put $N=\sum_{r=0}^I n_r$ and $M=\sum_{i=1}^I n_i$. If $n_i>0$, unused capacity on link $i$ could increase $x_i$, so

$$
\boxed{n_0x_0+n_ix_i=1\quad(n_i>0)}.
$$

When $n_0>0$, write $w_0=n_0x_0$. For active local routes their aggregate rates are $1-w_0$, and the objective, up to constants independent of $w_0$, is

$$
n_0\log w_0+M\log(1-w_0).
$$

For $M>0$, differentiation gives $n_0/w_0=M/(1-w_0)$, hence $w_0=n_0/N$; when $M=0$ the maximizing endpoint is $w_0=1$, giving the same answer. Thus the [proportionally fair allocation on a linear flow network](../../../../../proportionally-fair-allocation-on-a-linear-flow-network.md) is

$$
\boxed{x_0=\frac1N\ (n_0>0),\qquad x_i=\frac{M}{Nn_i}\ (n_i>0)}.
$$

If $n_0=0$ and $N>0$, this gives $x_i=1/n_i$ on every active local route, as expected. No departure occurs at the empty state.

Independent [Poisson processes](../../../../../poisson-process.md) of flow arrivals and independent [exponential distributions](../../../../../exponential-distribution.md) of document sizes make the count vector a [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md). By the [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md), a surviving residual size with [exponential distribution](../../../../../exponential-distribution.md) still has rate $\mu_r$ per unit of transferred data, so each route-$r$ flow completes at instantaneous rate $\mu_rx_r(n)$. The transition intensities are

$$
\boxed{q(n,n+e_r)=\nu_r,\qquad q(n,n-e_r)=\mu_rn_rx_r(n)}.
$$

Hence the through-route departure rate is $\mu_0n_0/N$ and each active local route's rate is $\mu_iM/N$.

To obtain the [stationary law of a linear flow network](../../../../../stationary-law-of-a-linear-flow-network.md), define

$$
H(n)=\binom{N}{n_0},\qquad \rho_r=\nu_r/\mu_r,
\qquad \pi(n)=K H(n)\prod_{r=0}^I\rho_r^{n_r}.
$$

For a through departure $H(n-e_0)/H(n)=n_0/N$; for an active local departure $H(n-e_i)/H(n)=M/N$. These are exactly the aggregate service rates, so the [detailed balance](../../../../../detailed-balance.md) identities $\pi(n-e_r)\nu_r=\pi(n)\mu_rn_rx_r(n)$ hold. This also shows why the [binomial coefficient](../../../../../binomial-coefficient.md) is essential; a factor $N$ would not have the required ratios.

For fixed local counts with total $M$, the [negative binomial series](../../../../../negative-binomial-series.md) gives

$$
\sum_{n_0\geq0}\binom{n_0+M}{n_0}\rho_0^{n_0}=(1-\rho_0)^{-M-1}.
$$

Sum the remaining independent [geometric series](../../../../../geometric-series.md) to find

$$
Z=\sum_nH(n)\prod_r\rho_r^{n_r}
=\frac1{1-\rho_0}\prod_{i=1}^I\frac1{1-\rho_i/(1-\rho_0)}
=\frac{(1-\rho_0)^{I-1}}{\prod_{i=1}^I(1-\rho_0-\rho_i)}.
$$

The given load conditions make every series converge. Setting $K=1/Z$ proves

$$
\boxed{\pi(n)=(1-\rho_0)^{1-I}\prod_{i=1}^I(1-\rho_0-\rho_i)
\binom{\sum_{r=0}^I n_r}{n_0}\prod_{r=0}^I\rho_r^{n_r}}.
$$

The chain has bounded total departure rate, finite arrival rate and no explosion. With positive arrival rates it is irreducible, and this normalized invariant law gives the [positive recurrent Markov chain](../../../../../positive-recurrent-markov-chain.md) property; zero arrival rates restrict the stationary support to the corresponding reachable class.

Summing out $n_0$ shows [local-count independence in a linear flow network](../../../../../local-count-independence-in-a-linear-flow-network.md): the local counts have independent [geometric distributions](../../../../../geometric-distribution.md) on $\mathbb Z_+$ with ratios $q_i=\rho_i/(1-\rho_0)$. Therefore

$$
\boxed{\mathbb E n_i=\frac{q_i}{1-q_i}=\frac{\rho_i}{1-\rho_0-\rho_i},\qquad i=1,\ldots,I}.
$$

They are independent of one another under the stationary marginal, despite sharing the random through-flow population. The through count is generally dependent on them.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
