<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Only routes with $n_r>0$ contribute to [proportional fairness](../../../../../proportional-fairness.md) or to the [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md); omit inactive routes from expressions with a rate in the denominator. Active routes have positive rates whenever a positive feasible allocation exists. For a feasible competitor $y$, the elementary [logarithm](../../../../../logarithm.md) inequality $\log u\leq u-1$ gives

$$
\sum_rn_r\log y_r-\sum_rn_r\log x_r
=\sum_rn_r\log\frac{y_r}{x_r}
\leq\sum_rn_r\frac{y_r-x_r}{x_r}\leq0.
$$

A zero competitor rate on an active route has utility $-\infty$ and also cannot improve the objective. Therefore **a proportionally fair allocation maximizes the logarithmic objective**. Conversely, the feasible set is a [convex set](../../../../../convex-set.md), and differentiating the objective along $x+t(y-x)$ at $t=0+$ shows that an optimizer satisfies the [proportional fairness](../../../../../proportional-fairness.md) inequality. Strict [concavity](../../../../../concave-function.md) gives uniqueness on active coordinates; rates assigned to nonexistent flows are immaterial.

In the [linear flow network](../../../../../linear-flow-network.md), put $z_0=n_0x_0$ and $z_i=n_ix_i$ for active routes. A local route $i$ uses only resource $i$. If $n_i>0$ and $z_0+z_i<1$, increasing $x_i$ increases the objective without violating any other constraint. Thus each active local route saturates its resource:

$$
\boxed{n_0x_0+n_ix_i=1\quad(n_i>0).}
$$

Write $L=\sum_{i=1}^In_i$ and $N=n_0+L$. For $n_0>0$ and $L>0$, substitute $z_i=1-z_0$ into the objective. Apart from constants its dependence on $z_0$ is

$$
n_0\log z_0+L\log(1-z_0).
$$

Its derivative vanishes when $n_0/z_0=L/(1-z_0)$, and its second derivative is negative. Hence the **per-flow through-route rate** is

$$
\boxed{z_0=\frac{n_0}{N},\qquad x_0=\frac1N\quad(n_0>0),
\qquad x_i=\frac{L}{Nn_i}\quad(n_i>0).}
$$

If $L=0<n_0$, the optimal through-route aggregate rate is one, so $x_0=1/n_0=1/N$ still holds. If $n_0=0<L$, each active local route has $x_i=1/n_i$, also given by the displayed local formula. When $N=0$ there are no flows and no departures. Inactive coordinates need not be assigned these undefined per-flow formulas.

Independent arrivals and exponential document sizes make this a [flow-level network model](../../../../../flow-level-network-model.md). A document of type $r$ has residual-size hazard $\mu_r$ per unit of data transmitted; when its transmission speed is $x_r(n)$, its completion hazard per unit time is $\mu_rx_r(n)$. Thus the [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) of flow counts has **transition intensities**

$$
\boxed{q(n,n+e_r)=\nu_r,\qquad
q(n,n-e_r)=\mu_r n_rx_r(n)\quad(n_r>0).}
$$

For $N>0$ these departure intensities are $\mu_0n_0/N$ for the through route and $\mu_iL/N$ for an active local route. Total arrival intensity is constant and total departure intensity is bounded by $\sum_r\mu_r$, ensuring a [nonexplosive Markov chain](../../../../../nonexplosive-markov-chain.md).

Set $\rho_r=\nu_r/\mu_r$, the [offered traffic](../../../../../offered-traffic.md), and define the [balance function of a flow-level network](../../../../../balance-function-of-a-flow-level-network.md)

$$
\Phi(n)=\binom{N}{n_0},\qquad \Phi(0)=1.
$$

The [binomial coefficients](../../../../../binomial-coefficient.md) satisfy

$$
\frac{\Phi(n-e_0)}{\Phi(n)}=\frac{n_0}{N}=n_0x_0(n),
\qquad
\frac{\Phi(n-e_i)}{\Phi(n)}=\frac{L}{N}=n_ix_i(n)\quad(n_i>0).
$$

These identities also cover states with only one kind of active route. They show that the weight $a(n)=\Phi(n)\prod_{r=0}^I\rho_r^{n_r}$ satisfies

$$
a(n)q(n,n-e_r)=\nu_ra(n-e_r).
$$

Thus [detailed balance for a continuous-time Markov chain](../../../../../detailed-balance-for-a-continuous-time-markov-chain.md) proves that this is a [reversible Markov chain](../../../../../reversible-markov-chain.md) and reduces the [stationary distribution](../../../../../stationary-distribution.md) calculation to normalization.

Sum over $n_0$ first. The [negative binomial series](../../../../../negative-binomial-series.md) gives, for fixed local counts and $L=\sum_i n_i$,

$$
\sum_{n_0=0}^{\infty}\binom{L+n_0}{n_0}\rho_0^{n_0}
=(1-\rho_0)^{-L-1}.
$$

All summands are nonnegative, so the [Tonelli theorem](../../../../../tonelli-theorem.md) permits exchanging the sums. The partition sum is therefore

$$
Z=\frac1{1-\rho_0}\prod_{i=1}^I
\sum_{n_i=0}^{\infty}\left(\frac{\rho_i}{1-\rho_0}\right)^{n_i}
=\frac{(1-\rho_0)^{I-1}}{\prod_{i=1}^I(1-\rho_0-\rho_i)}.
$$

It is finite exactly when $\rho_0+\rho_i<1$ for every $i$, for $I\geq1$. These are the resource-load conditions: resource $i$ receives the through-route offered traffic plus its local offered traffic. The **normalized stationary distribution** is

$$
\boxed{\pi(n)=(1-\rho_0)^{1-I}
\prod_{i=1}^I(1-\rho_0-\rho_i)
\binom{\sum_{r=0}^In_r}{n_0}\prod_{r=0}^I\rho_r^{n_r}.}
$$

With positive arrival rates this is the unique [stationary distribution](../../../../../stationary-distribution.md) of the irreducible feasible flow-count chain. Zero arrival rates restrict its closed class to the corresponding zero coordinates.

Summing out $n_0$ also shows that the local counts are independent, with [geometric distributions](../../../../../geometric-distribution.md) on $0,1,\ldots$:

$$
\mathbb P(n_1=k_1,\ldots,n_I=k_I)
=\prod_{i=1}^I(1-a_i)a_i^{k_i},
\qquad a_i=\frac{\rho_i}{1-\rho_0}.
$$

Hence their **mean flow counts** are

$$
\boxed{\mathbb E_\pi[n_i]=\frac{a_i}{1-a_i}
=\frac{\rho_i}{1-\rho_0-\rho_i}.}
$$

The binomial balance factor is essential: independent geometric counts for all routes would not give these departure rates or the correct resource-load normalization.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 213](../../paper-213-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
