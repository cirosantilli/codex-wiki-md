<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A feasible per-flow allocation satisfies $x_r>0$ for each active route and $\sum_rA_{jr}n_rx_r\leq C_j$. It has [proportional fairness](../../../../../proportional-fairness.md) if every feasible competitor obeys

$$
\boxed{\sum_{r:n_r>0}n_r\frac{\widetilde x_r-x_r}{x_r}\leq0.}
$$

By the first-order inequality for the strictly concave [logarithm](../../../../../logarithm.md), this is equivalent to maximizing [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) $\sum_{r:n_r>0}n_r\log x_r$ over the feasible allocations. Inactive-route rates are immaterial; set them to zero as a convention.

Write $a=n_{\{1\}}$, $b=n_{\{2\}}$, $c=n_{\{1,2\}}$, and $N=a+b+c$. The [capacity constraints](../../../../../capacity-constraint.md) are $ax_1+cx_0\leq1$ and $bx_2+cx_0\leq1$. For $c>0$, put $q=cx_0$. Each active local route uses its remaining capacity $1-q$. Omitting constants, the utility is

$$
(a+b)\log(1-q)+c\log q.
$$

Its maximum has $q=c/N$; when $a+b=0$, the maximum is the endpoint $q=1$. Hence for active routes

$$
\boxed{x_1=\frac{a+b}{aN}\ (a>0),\qquad x_2=\frac{a+b}{bN}\ (b>0),\qquad x_0=\frac1N\ (c>0).}
$$

These formulas also give $x_1=1/a$ and $x_2=1/b$ when $c=0$. When $N=0$ there is no allocated service. Equivalently, the aggregate route rates for $N>0$ are

$$
\Lambda_1=\mathbf1_{\{a>0\}}\frac{a+b}{N},\quad
\Lambda_2=\mathbf1_{\{b>0\}}\frac{a+b}{N},\quad
\Lambda_0=\frac cN.
$$

This is the [proportionally fair allocation on a two-resource linear network](../../../../../proportionally-fair-allocation-on-a-two-resource-linear-network.md) for a [two-resource linear flow network](../../../../../two-resource-linear-flow-network.md).

For [independent](../../../../../independent-random-variables.md) [Poisson processes](../../../../../poisson-process.md) of documents and [independent](../../../../../independent-random-variables.md) document sizes with [exponential distribution](../../../../../exponential-distribution.md) of rate $\mu_r$, the [memorylessness of the exponential distribution](../../../../../memorylessness-of-the-exponential-distribution.md) makes the population a [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md). Its transition intensities are

$$
\boxed{q(n,n+e_r)=\nu_r,\qquad q(n,n-e_r)=\mu_r\Lambda_r(n)\quad(n_r>0).}
$$

The departure intensity sums the $n_r$ [independent](../../../../../independent-random-variables.md) completion hazards $\mu_rx_r$. There is no departure on an inactive route. Set $\rho_r=\nu_r/\mu_r$, with $\mu_r>0$.

To prove the proposed [stationary distribution](../../../../../stationary-distribution.md), define the [balance function of a flow-level network](../../../../../balance-function-of-a-flow-level-network.md)

$$
\Psi(a,b,c)=\binom{a+b+c}{c}.
$$

For an active local route, $\Psi(n-e_r)/\Psi(n)=(a+b)/N$, while for the through route this ratio is $c/N$. Thus $\Lambda_r(n)=\Psi(n-e_r)/\Psi(n)$. The weights

$$
\pi(n)=B\Psi(n)\rho_1^a\rho_2^b\rho_0^c
$$

satisfy [detailed balance](../../../../../detailed-balance.md) on every arrival-departure pair:

$$
\pi(n)\nu_r=\pi(n+e_r)\mu_r\frac{\Psi(n)}{\Psi(n+e_r)}.
$$

Each total jump rate is bounded by $\sum_r(\nu_r+\mu_r)$, so the chain is a [nonexplosive Markov chain](../../../../../nonexplosive-markov-chain.md); normalized detailed-balance weights therefore give its [stationary distribution](../../../../../stationary-distribution.md), the [stationary law of a two-resource linear flow network](../../../../../stationary-law-of-a-two-resource-linear-flow-network.md).

Use the [negative binomial series](../../../../../negative-binomial-series.md) to sum first over $c$:

$$
\sum_{c\geq0}\binom{a+b+c}{c}\rho_0^c=(1-\rho_0)^{-a-b-1}.
$$

The remaining two [geometric series](../../../../../geometric-series.md) give

$$
Z=B^{-1}=\frac{1-\rho_0}{(1-\rho_0-\rho_1)(1-\rho_0-\rho_2)}.
$$

All summands are nonnegative. Consequently the sum is finite exactly under the [stability conditions for a two-resource linear flow network](../../../../../stability-conditions-for-a-two-resource-linear-flow-network.md)

$$
\boxed{\rho_1+\rho_0<1,\qquad\rho_2+\rho_0<1,\qquad
B=\frac{(1-\rho_0-\rho_1)(1-\rho_0-\rho_2)}{1-\rho_0}.}
$$

These say that the offered load on each unit-capacity resource is strictly below one. Equality is insufficient: at least one [geometric series](../../../../../geometric-series.md) then diverges. If all arrival rates are positive, the chain is irreducible and the normalizable law is its unique equilibrium law.

Finally put $q_i=\rho_i/(1-\rho_0)$, $i=1,2$. Summing over $c$ yields

$$
\boxed{\mathbb P(a=k,b=\ell)=(1-q_1)q_1^k(1-q_2)q_2^\ell,\qquad k,\ell\geq0.}
$$

Thus **the two local-route counts are [independent](../../../../../independent-random-variables.md)**, each with [geometric distribution](../../../../../geometric-distribution.md) on the nonnegative integers. The conditional through-route count has [negative binomial distribution](../../../../../negative-binomial-distribution.md)

$$
\mathbb P(c=m\mid a,b)=\binom{a+b+m}{m}(1-\rho_0)^{a+b+1}\rho_0^m,\qquad
\mathbb E[c\mid a,b]=\frac{\rho_0(a+b+1)}{1-\rho_0}.
$$

For positive traffic rates this depends on the local counts, so **all three route counts are not [independent](../../../../../independent-random-variables.md)**. More quantitatively, $\operatorname{Cov}(a,c)=\rho_0\operatorname{Var}(a)/(1-\rho_0)>0$, and likewise for $b$. If zero arrival rates are allowed, the exceptional [independent](../../../../../independent-random-variables.md) cases are $\rho_0=0$, or $\rho_1=\rho_2=0$, when the relevant counts are deterministic zero. This distinction is [local-count independence with through-flow dependence](../../../../../local-count-independence-with-through-flow-dependence.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
