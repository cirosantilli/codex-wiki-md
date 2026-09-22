<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Here $x_r$ is the rate per individual active flow, and $n_rx_r$ is its route's aggregate rate. On routes with $n_r>0$, a [proportionally fair allocation](../../../../../proportional-fairness.md) is a feasible positive rate vector satisfying

$$
\sum_{r:n_r>0}n_r\frac{\widetilde x_r-x_r}{x_r}\leq0
$$

for every feasible competitor $\widetilde x$, where feasibility means $\sum_{r:j\in r}n_r\widetilde x_r\leq C_j$. This is equivalent to maximizing [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) $\sum_{r:n_r>0}n_r\log x_r$: its gradient gives the displayed inequality, and the supporting-tangent inequality proves sufficiency. The objective is [strictly concave](../../../../../strictly-concave-function.md) on active rates. Rates assigned to absent flows are irrelevant and may be set to zero.

For the [linear flow network](../../../../../linear-flow-network.md), an active local route can increase its rate if its link constraint has slack, improving the objective without affecting any other link. Thus

$$
\boxed{n_0x_0+n_ix_i=1\qquad(n_i>0).}
$$

Put $m=\sum_{i=1}^In_i$ and $N=n_0+m$. If $n_0>0$ and $m>0$, eliminate the active local rates by $x_i=(1-n_0x_0)/n_i$. Up to constants, the utility becomes

$$
n_0\log x_0+m\log(1-n_0x_0),\qquad 0<x_0<1/n_0.
$$

Its derivative is $n_0/x_0-n_0m/(1-n_0x_0)$, which vanishes exactly at

$$
\boxed{x_0=\frac1N,\qquad x_i=\frac{m}{Nn_i}\quad(n_i>0).}
$$

Strict concavity proves this is the optimum, and unused local links impose no stronger constraint because $n_0x_0\leq1$. If $m=0<n_0$, maximizing $n_0\log x_0$ gives $x_0=1/n_0$, the same formula. If $n_0=0$, each active local route has $x_i=1/n_i$. These are the [proportionally fair allocation on a linear flow network](../../../../../proportionally-fair-allocation-on-a-linear-flow-network.md). When $N=0$, there is no service to allocate.

The [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) of exponential document sizes makes a flow transmitting at rate $x_r$ complete with intensity $\mu_rx_r$. Summing over its $n_r$ flows gives the [flow-level network model](../../../../../flow-level-network-model.md) transition rates

$$
q(n,n+e_r)=\nu_r\quad(0\leq r\leq I),
$$

and, for nonempty states,

$$
\boxed{q(n,n-e_0)=\mu_0\frac{n_0}{N}\quad(n_0>0),\qquad
q(n,n-e_i)=\mu_i\frac{m}{N}\quad(n_i>0).}
$$

All absent-route departure intensities, including those at the empty state, are zero. In particular the local completion rate is the aggregate rate $\mu_im/N$, not $\mu_i/N$. Total rates are bounded by $\sum_r\nu_r+\sum_r\mu_r$, so the [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) is nonexplosive.

Set $\rho_r=\nu_r/\mu_r$ and consider the weights

$$
w(n)=\binom{N}{n_0}\prod_{r=0}^I\rho_r^{n_r}.
$$

The [binomial coefficient](../../../../../binomial-coefficient.md) is the [balance function of a flow-level network](../../../../../balance-function-of-a-flow-level-network.md). For a through-route arrival, its adjacent-weight ratio is

$$
\frac{w(n+e_0)}{w(n)}=\rho_0\frac{N+1}{n_0+1}.
$$

The reverse departure rate is $\mu_0(n_0+1)/(N+1)$, so $w(n+e_0)q(n+e_0,n)=w(n)\nu_0$. For a local-route arrival,

$$
\frac{w(n+e_i)}{w(n)}=\rho_i\frac{N+1}{m+1},
$$

and the reverse departure rate is $\mu_i(m+1)/(N+1)$, giving the same [detailed balance](../../../../../detailed-balance.md) identity. This includes arrivals from the empty state.

To normalize, first fix all local counts and sum over $n_0$. The [negative binomial series](../../../../../negative-binomial-series.md) gives

$$
\sum_{n_0\geq0}\binom{n_0+m}{n_0}\rho_0^{n_0}=(1-\rho_0)^{-m-1}.
$$

The remaining [geometric series](../../../../../geometric-series.md) factor, so

$$
Z=\sum_nw(n)=\frac1{1-\rho_0}\prod_{i=1}^I\frac1{1-\rho_i/(1-\rho_0)}
=\frac{(1-\rho_0)^{I-1}}{\prod_{i=1}^I(1-\rho_0-\rho_i)}.
$$

This is finite precisely under the stated strict load inequalities $\rho_0+\rho_i<1$ for each resource. Thus [detailed balance](../../../../../detailed-balance.md) proves the [stationary law of a linear flow network](../../../../../stationary-law-of-a-linear-flow-network.md):

$$
\boxed{\pi(n)=(1-\rho_0)^{1-I}\prod_{i=1}^I(1-\rho_0-\rho_i)
\binom{\sum_{r=0}^In_r}{n_0}\prod_{r=0}^I\rho_r^{n_r}.}
$$

With positive arrival rates this is the unique [stationary distribution](../../../../../stationary-distribution.md) of the irreducible chain. Zero arrival rates are handled by restricting to the accessible class with their counts zero, interpreting $0^0=1$.

Summing this distribution over $n_0$ gives [local-count independence in a linear flow network](../../../../../local-count-independence-in-a-linear-flow-network.md):

$$
\Pr\{n_1=k_1,\ldots,n_I=k_I\}
=\prod_{i=1}^I\left(1-\frac{\rho_i}{1-\rho_0}\right)
\left(\frac{\rho_i}{1-\rho_0}\right)^{k_i}.
$$

These are independent [geometric distributions](../../../../../geometric-distribution.md). Differentiating a [geometric series](../../../../../geometric-series.md), or summing its mean directly, gives

$$
\boxed{\mathbb E n_i=\frac{\rho_i/(1-\rho_0)}{1-\rho_i/(1-\rho_0)}
=\frac{\rho_i}{1-\rho_0-\rho_i}\quad(1\leq i\leq I).}
$$

This independence concerns the local counts at one stationary time; their evolving processes share the through route and are not independent processes.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
