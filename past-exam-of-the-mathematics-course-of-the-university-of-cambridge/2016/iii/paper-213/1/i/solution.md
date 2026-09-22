<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [open migration process](../../../../../../open-migration-process.md) is a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) recording the populations $n=(n_1,\ldots,n_J)$ of finitely many colonies. Independent external [Poisson processes](../../../../../../poisson-process.md) bring individuals to colony $j$ at rate $\nu_j$. When that colony contains $k>0$ individuals, a departure opportunity occurs at total rate $\phi_j(k)>0$, with $\phi_j(0)=0$. The departing individual moves to colony $l$ with [probability](../../../../../../probability.md) $p_{jl}$, or leaves the system with [probability](../../../../../../probability.md) $p_{j0}=1-\sum_l p_{jl}$. Routing choices and the clocks are independent. A return to the same colony does not change the state.

The word open means that the routing [matrix](../../../../../../matrix.md) $P=(p_{jl})$ is transient: every individual eventually leaves, or equivalently the [spectral radius](../../../../../../spectral-radius.md) of $P$ is less than one. The [traffic equations of an open migration process](../../../../../../traffic-equation-of-an-open-migration-process.md), with row-vector convention, give the total arrival rates:

$$
\alpha=\nu+\alpha P,\qquad \alpha=\nu(I-P)^{-1}.
$$

These rates include migrations as well as external arrivals. On the active colonies assume $\alpha_j>0$ and the usual [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) condition. Put

$$
b_j(k)=\frac{\alpha_j^k}{\prod_{h=1}^k\phi_j(h)},\qquad b_j(0)=1,
\qquad Z_j=\sum_{k=0}^{\infty}b_j(k).
$$

The **product form and its normalization condition** are

$$
\boxed{\pi(n)=\prod_{j=1}^J\frac{b_j(n_j)}{Z_j},\qquad Z_j<\infty\quad\hbox{for every }j.}
$$

To establish the [product-form stationary distribution of an open migration process](../../../../../../product-form-stationary-distribution-of-an-open-migration-process.md), first use its unnormalized weight $b(n)=\prod_jb_j(n_j)$. Its ratios satisfy $b_j(k)\phi_j(k)=\alpha_jb_j(k-1)$. The incoming external arrivals into $n$, divided by $b(n)$, contribute $\sum_j\nu_j\phi_j(n_j)/\alpha_j$. Incoming exits contribute $\sum_i\alpha_i p_{i0}$. Incoming migrations from $i$ to $j\ne i$ contribute $\alpha_i p_{ij}\phi_j(n_j)/\alpha_j$. Terms involving an empty destination are zero. Thus the full incoming rate divided by $b(n)$ is

$$
\sum_i\alpha_i p_{i0}
+\sum_j\frac{\phi_j(n_j)}{\alpha_j}
\left(\nu_j+\sum_{i\ne j}\alpha_i p_{ij}\right)
=\sum_j\nu_j+\sum_j\phi_j(n_j)(1-p_{jj}).
$$

Here the [traffic equations of an open migration process](../../../../../../traffic-equation-of-an-open-migration-process.md) give the second equality, including $\sum_i\alpha_i p_{i0}=\sum_j\nu_j$. The right side is precisely the total outgoing rate. This proves [global balance for a continuous-time Markov chain](../../../../../../global-balance-for-a-continuous-time-markov-chain.md); pairwise [detailed balance](../../../../../../detailed-balance.md) is not required for general routing.

For finite rates at each finite population, the [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) is [nonexplosive Markov chain](../../../../../../nonexplosive-markov-chain.md): its total population is bounded over a finite time interval by the initial population plus the finitely many external arrivals, so it visits a finite set on which all jump rates are bounded. Consequently finite $Z_j$ normalize the invariant weight to a [stationary distribution](../../../../../../stationary-distribution.md). Under the stated [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) assumptions, this is the unique [stationary distribution](../../../../../../stationary-distribution.md), and it is a [positive recurrent Markov chain](../../../../../../positive-recurrent-markov-chain.md). Conversely, the unique invariant measure of an irreducible recurrent chain is proportional to $b$, so a [positive recurrent Markov chain](../../../../../../positive-recurrent-markov-chain.md) requires its normalization to be finite. A sufficient condition is $\liminf_{k\to\infty}\phi_j(k)>\alpha_j$; the series criterion itself is the exact condition. Colonies with $\alpha_j=0$ have zero stationary population and can be removed from the active class.

For the single-server [M/M/1 queue](../../../../../../m-m-1-queue.md) specialization, $\phi_j(k)=\phi_j$ for $k>0$, each stationary colony has the [geometric distribution](../../../../../../geometric-distribution.md) of an [M/M/1 queue](../../../../../../m-m-1-queue.md):

$$
\rho_j=\frac{\alpha_j}{\phi_j}<1,\qquad
\mathbb E[n_j]=\frac{\rho_j}{1-\rho_j}
=\frac{\alpha_j}{\phi_j-\alpha_j}.
$$

The [traffic equations of an open migration process](../../../../../../traffic-equation-of-an-open-migration-process.md) do not involve the service rates, so the $\alpha_j$ remain fixed during this [service-capacity allocation in an open migration process](../../../../../../service-capacity-allocation-in-an-open-migration-process.md). Write $A=\sum_j\alpha_j$, $B=F-A$ and $b_j=\phi_j-\alpha_j$. A stationary allocation requires $B>0$, with $b_j>0$ and $\sum_jb_j=B$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\left(\sum_j\sqrt{\alpha_j}\right)^2
=\left(\sum_j\sqrt{\frac{\alpha_j}{b_j}}\sqrt{b_j}\right)^2
\leq\left(\sum_j\frac{\alpha_j}{b_j}\right)B.
$$

Equality holds exactly when $b_j$ is proportional to $\sqrt{\alpha_j}$. Hence, for positive arrival rates, the **unique optimal service allocation** and the minimum [expected value](../../../../../../expected-value.md) of the total population are

$$
\boxed{\phi_j^*=\alpha_j+
\frac{(F-\sum_l\alpha_l)\sqrt{\alpha_j}}{\sum_l\sqrt{\alpha_l}},
\qquad
\min\mathbb E\!\left[\sum_jn_j\right]
=\frac{(\sum_j\sqrt{\alpha_j})^2}{F-\sum_j\alpha_j}.}
$$

If $F\leq A$ and some arrival rate is positive, no stable service allocation exists. Zero-arrival colonies need no service in their stationary empty class: allowing zero service there gives the same formula restricted to active colonies. If strictly positive service is demanded even at inactive colonies, the displayed minimum is an infimum approached as that unused allocation tends to zero. If all arrivals vanish, the stationary mean population is zero for every allocation that drains the initial population.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 213](../../../paper-213-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
