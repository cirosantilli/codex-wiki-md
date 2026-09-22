<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Only routes with $n_r>0$ need a per-flow rate: absent flows contribute no utility and have no completion events. Interpret the proportional-change sum and the logarithmic objective on these active routes. With positive capacities and finitely many nonempty routes, a strictly positive feasible active-rate vector exists. Define its [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) by $U(x)=\sum_{r:n_r>0}n_r\log x_r$, with value $-\infty$ if an active rate is zero.

For positive feasible $x,y$, the elementary [concavity](../../../../../concave-function.md) inequality $\log u\leq u-1$ gives

$$
U(y)-U(x)=\sum_rn_r\log\frac{y_r}{x_r}\leq\sum_rn_r\frac{y_r-x_r}{x_r}.
$$

The last sum is nonpositive by [proportional fairness](../../../../../proportional-fairness.md). Feasible competitors with a zero active rate have utility $-\infty$, so they cannot improve it either. Thus **a proportionally fair allocation maximizes weighted logarithmic utility**. Conversely, if $x$ maximizes this utility, the feasible line segment $x+\theta(y-x)$ has nonpositive right derivative at $\theta=0$, giving precisely $\sum_rn_r(y_r-x_r)/x_r\leq0$. This also covers a competitor with zero coordinates, since $x+\theta(y-x)$ stays positive for sufficiently small $\theta$. The [strictly concave function](../../../../../strictly-concave-function.md) $U$ makes the active-rate optimizer unique.

For the [linear flow network](../../../../../linear-flow-network.md), put $M=\sum_{i=1}^{I}n_i$ and $N=n_0+M$. If $n_i>0$ and resource $i$ is not saturated, its local per-flow rate could be increased without affecting any other resource. This would strictly increase [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md). Hence

$$
\boxed{n_0x_0+n_ix_i=1\quad\text{whenever }n_i>0.}
$$

If $n_0>0$ and $M>0$, substitute $x_i=(1-n_0x_0)/n_i$ on all active local routes into the utility. The terms depending on $x_0$ are

$$
f(x_0)=n_0\log x_0+M\log(1-n_0x_0),\qquad 0<x_0<1/n_0.
$$

Its derivative vanishes when $1/x_0=M/(1-n_0x_0)$, so $x_0=1/N$. Its second derivative is negative, giving the unique maximizer. If $M=0<n_0$, utility increases up to the capacity endpoint $x_0=1/n_0=1/N$. If $n_0=0$, each active local route uses its entire local resource. Altogether the [proportionally fair allocation on a linear flow network](../../../../../proportionally-fair-allocation-on-a-linear-flow-network.md) is

$$
\boxed{x_0=\frac1N\ (n_0>0),\qquad x_i=\frac{M}{Nn_i}\ (n_i>0).}
$$

Absent-route rates may be set to zero, and departures are zero at the empty state $N=0$. Notice that these are per-flow rates: the aggregate through service is $n_0/N$, while each active local route gets aggregate service $M/N$.

In the document-transfer [flow-level network model](../../../../../flow-level-network-model.md), let $e_r$ be the unit vector for route $r$. Independent [Poisson processes](../../../../../poisson-process.md) of flow arrivals give transitions $n\to n+e_r$ at rate $\nu_r$. An active document on route $r$ receives service at rate $x_r(n)$ and has an [exponential distribution](../../../../../exponential-distribution.md) of size with parameter $\mu_r$. By the [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md), its instantaneous completion rate is $\mu_rx_r(n)$. Summing over the active documents gives the [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) intensities

$$
\boxed{q(n,n+e_r)=\nu_r,\qquad q(n,n-e_r)=\mu_rn_rx_r(n)\quad(n_r>0).}
$$

Thus through-route departures have rate $\mu_0n_0/N$, and active local departures have rate $\mu_iM/N$. All other off-diagonal intensities vanish. The diagonal intensity is the negative of the sum of the outgoing intensities. Each route's aggregate service is at most one, so the total jump rate is bounded by $\sum_r(\nu_r+\mu_r)$; the process is a [nonexplosive continuous-time Markov chain](../../../../../nonexplosive-continuous-time-markov-chain.md).

Set $\rho_r=\nu_r/\mu_r$, assume $\mu_r>0$, and define the [balance function of a flow-level network](../../../../../balance-function-of-a-flow-level-network.md) by

$$
H(n)=\binom{N}{n_0},\qquad H(0)=1.
$$

The adjacent-state ratios of this [binomial coefficient](../../../../../binomial-coefficient.md) are

$$
\frac{H(n-e_0)}{H(n)}=\frac{n_0}{N}\quad(n_0>0),\qquad\frac{H(n-e_i)}{H(n)}=\frac{N-n_0}{N}=\frac{M}{N}\quad(n_i>0).
$$

They equal the aggregate service rates just obtained. Therefore, with $w(n)=H(n)\prod_r\rho_r^{n_r}$,

$$
w(n)\mu_rn_rx_r(n)=w(n-e_r)\mu_r\rho_r=w(n-e_r)\nu_r.
$$

These are the [detailed balance for a continuous-time Markov chain](../../../../../detailed-balance-for-a-continuous-time-markov-chain.md) equations on every adjacent pair. Summing incoming and outgoing pairs proves stationarity whenever the weights can be normalized. Hence the [stationary law of a linear flow network](../../../../../stationary-law-of-a-linear-flow-network.md) is

$$
\boxed{\pi(n)=B^{-1}\binom{\sum_{r=0}^{I}n_r}{n_0}\prod_{r=0}^{I}\left(\frac{\nu_r}{\mu_r}\right)^{n_r}.}
$$

The coefficient here is a [binomial coefficient](../../../../../binomial-coefficient.md), not merely the total number of flows. Both it and the denominator in $x_0=1/N$ are visible in the original PDF but missing from the converted TeX.

We can also determine exactly when the normalizing constant is finite. For $0\leq\rho_0<1$, summing first over $n_0$ with local counts fixed and applying the [negative binomial series](../../../../../negative-binomial-series.md) gives

$$
\sum_{n_0\geq0}\binom{n_0+M}{n_0}\rho_0^{n_0}=(1-\rho_0)^{-M-1}.
$$

The remaining sums are independent [geometric series](../../../../../geometric-series.md). Thus

$$
B=\frac1{1-\rho_0}\prod_{i=1}^{I}\frac1{1-\rho_i/(1-\rho_0)}=\boxed{\frac{(1-\rho_0)^{I-1}}{\prod_{i=1}^{I}(1-\rho_0-\rho_i)}}
$$

provided $\rho_0+\rho_i<1$ for every $i$. These inequalities are also necessary: if $\rho_0\geq1$, the states with every local count zero already give a divergent sum; otherwise any local ratio at least one makes its [geometric series](../../../../../geometric-series.md) diverge. Thus the stationary formula requires **strict offered load below capacity at every resource**. With positive arrival rates, the process is irreducible, and these normalizable [detailed balance](../../../../../detailed-balance.md) weights give its unique [stationary distribution](../../../../../stationary-distribution.md). Outside these inequalities, the displayed weights are not a probability distribution. Zero arrival rates can be handled on the reachable class by setting the corresponding population to zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
