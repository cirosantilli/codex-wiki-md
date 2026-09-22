<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a network with [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) $A_{jr}=\mathbf1_{\{j\in r\}}$, a per-flow rate vector $x$ is feasible when $x_r\ge0$ and $\sum_r A_{jr}n_rx_r\le C_j$ for every resource. A [proportionally fair allocation](../../../../../proportional-fairness.md) has strictly positive rates on active routes and satisfies

$$
\sum_{r:n_r>0}n_r\frac{y_r-x_r}{x_r}\le0
$$

for every feasible competing allocation $y$. Equivalently it maximizes the [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) $\sum_{r:n_r>0}n_r\log x_r$ subject to the capacity constraints. The equivalence follows from the first-order condition for this concave objective; strict concavity gives uniqueness on active routes. Rates on absent routes have no operational effect and may be set to zero.

Use labels $1,2,0$ for the routes $\{1\},\{2\},\{1,2\}$, and put $a=n_1$, $b=n_2$, $c=n_0$, $m=a+b$, $T=a+b+c$. The [two-resource linear flow network](../../../../../two-resource-linear-flow-network.md) has constraints

$$
a x_1+c x_0\le1,\qquad b x_2+c x_0\le1.
$$

When $c>0$ and $m>0$, write $v=cx_0$ for aggregate through service. Every active local route uses the remainder $1-v$ of its resource, since increasing its rate increases utility. Up to additive constants, the objective becomes $c\log v+m\log(1-v)$. Its derivative is $c/v-m/(1-v)$, so its unique maximum is $v=c/T$. This argument remains valid if only one local route is active: the unused local resource adds only the constraint $v\le1$. The resulting [proportionally fair allocation on a two-resource linear network](../../../../../proportionally-fair-allocation-on-a-two-resource-linear-network.md) is

$$
\boxed{x_0=\frac1T\ (c>0),\qquad x_1=\frac{m}{aT}\ (a>0),\qquad x_2=\frac{m}{bT}\ (b>0).}
$$

If $c=0$, each active local route receives its resource equally, $x_1=1/a$ or $x_2=1/b$, as the same formulas prescribe. If $m=0<c$, only the through route is active and $x_0=1/c$. At $T=0$ all rates may be set to zero. In particular no displayed expression is applied to an absent route with a zero denominator.

For independent [Poisson processes](../../../../../poisson-process.md) of flow arrivals and independent exponential document sizes of parameters $\mu_r>0$, the [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) makes $n$ a [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md). Each active flow completes with instantaneous rate $\mu_r x_r(n)$, so the [flow-level network model](../../../../../flow-level-network-model.md) has transitions

$$
\boxed{q(n,n+e_r)=\nu_r,\qquad q(n,n-e_r)=\mu_r n_r x_r(n)\quad(n_r>0).}
$$

Thus for $T>0$ the aggregate service rates $\phi_r=n_rx_r$ are

$$
\phi_0(n)=\frac cT,\qquad \phi_1(n)=\frac mT\mathbf1_{\{a>0\}},\qquad\phi_2(n)=\frac mT\mathbf1_{\{b>0\}}.
$$

They vanish at the empty state. The total transition rate is bounded by $\sum_r\nu_r+\sum_r\mu_r$, so the process is nonexplosive.

Put $\rho_r=\nu_r/\mu_r$ and define the [balance function of a flow-level network](../../../../../balance-function-of-a-flow-level-network.md)

$$
\Phi(a,b,c)=\binom{a+b+c}{c}.
$$

The elementary [binomial coefficient](../../../../../binomial-coefficient.md) ratios are

$$
\frac{\Phi(n-e_1)}{\Phi(n)}=\frac{a+b}{T}\quad(a>0),\qquad\frac{\Phi(n-e_2)}{\Phi(n)}=\frac{a+b}{T}\quad(b>0),\qquad\frac{\Phi(n-e_0)}{\Phi(n)}=\frac cT\quad(c>0).
$$

Hence $\phi_r(n)=\Phi(n-e_r)/\Phi(n)$ whenever that departure is possible. Weights $w(n)=\Phi(n)\prod_r\rho_r^{n_r}$ satisfy [detailed balance for a continuous-time Markov chain](../../../../../detailed-balance-for-a-continuous-time-markov-chain.md), since

$$
w(n)\nu_r=w(n+e_r)\mu_r\frac{\Phi(n)}{\Phi(n+e_r)}.
$$

When summable they therefore give the [stationary law of a two-resource linear flow network](../../../../../stationary-law-of-a-two-resource-linear-flow-network.md),

$$
\boxed{\pi(a,b,c)=B\binom{a+b+c}{c}\rho_1^a\rho_2^b\rho_0^c.}
$$

It remains to determine exactly when these weights normalize. First, summing only the terms $a=b=0$ requires $\rho_0<1$. For such $\rho_0$, the [negative binomial series](../../../../../negative-binomial-series.md), or the supplied identity with parameter $a+b+1$, gives

$$
\sum_{c=0}^\infty\binom{a+b+c}{c}\rho_0^c=(1-\rho_0)^{-a-b-1}.
$$

All weights are nonnegative, so the [Tonelli theorem](../../../../../tonelli-theorem.md) permits this order of summation. The normalizing sum is then

$$
Z=\frac1{1-\rho_0}\left[\sum_{a\ge0}\left(\frac{\rho_1}{1-\rho_0}\right)^a\right]\left[\sum_{b\ge0}\left(\frac{\rho_2}{1-\rho_0}\right)^b\right].
$$

The two [geometric series](../../../../../geometric-series.md) converge precisely under the [stability conditions for a two-resource linear flow network](../../../../../stability-conditions-for-a-two-resource-linear-flow-network.md), and evaluating them yields

$$
\boxed{\rho_1+\rho_0<1,\qquad\rho_2+\rho_0<1,\qquad B=\frac{(1-\rho_0-\rho_1)(1-\rho_0-\rho_2)}{1-\rho_0}.}
$$

These are exactly the strict offered-load constraints on the two unit-capacity resources; equality already makes a geometric sum diverge. For positive arrival rates the chain is irreducible, so the normalized law is its unique stationary probability and the chain is positive recurrent. Nonnegative arrival rates are also allowed with $0^0=1$ in the weights: a zero-arrival route is absent in the closed stationary class, and the same normalization conditions and formula remain valid there.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
