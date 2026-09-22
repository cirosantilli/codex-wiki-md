<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [open migration process](../../../../../../open-migration-process.md) has finitely many colonies and state $n\in\mathbb N^J$. External arrivals to colony $j$ form independent [Poisson processes](../../../../../../poisson-process.md) with rates $\nu_j$. When $n_j=k>0$, individuals leave that colony at total rate $g_j(k)>0$, with $g_j(0)=0$. A departing individual moves to $k$ with probability $p_{jk}$ or exits with probability $p_{j0}=1-\sum_kp_{jk}$. The routing choices and all arrival and service randomness are independent. The routing [matrix](../../../../../../matrix.md) $P=(p_{jk})$ is substochastic and transient: every individual eventually exits, equivalently its [spectral radius](../../../../../../spectral-radius.md) is less than one. Self-routing is allowed, but creates no state change.

The [traffic equations of an open migration process](../../../../../../traffic-equation-of-an-open-migration-process.md), using row vectors, are

$$
\alpha_j=\nu_j+\sum_k\alpha_kp_{kj},\qquad
\alpha=\nu(I-P)^{-1}.
$$

The [inverse matrix](../../../../../../matrix-inverse.md) exists because $\sum_{m\geq0}P^m$ converges; its $(k,j)$ entry counts expected visits to $j$ by an individual entering at $k$. Thus $\alpha_j$ includes both external arrivals and internal migrations. Restrict first to the accessible colonies with $\alpha_j>0$.

Set

$$
b_j(0)=1,\qquad b_j(k)=\frac{\alpha_j^k}{\prod_{h=1}^kg_j(h)},\qquad Z_j=\sum_{k\geq0}b_j(k).
$$

If each $Z_j<\infty$, the candidate [product-form stationary distribution of an open migration process](../../../../../../product-form-stationary-distribution-of-an-open-migration-process.md) is

$$
\boxed{\pi(n)=\prod_j\frac{b_j(n_j)}{Z_j}.}
$$

Here is a [global balance for a continuous-time Markov chain](../../../../../../global-balance-for-a-continuous-time-markov-chain.md) proof, which does not incorrectly assume that the routing is reversible. The weight ratio is $\pi(n+e_j)/\pi(n)=\alpha_j/g_j(n_j+1)$. After dividing the incoming balance equation at $n$ by $\pi(n)$, external arrivals contribute $\sum_{j:n_j>0}\nu_jg_j(n_j)/\alpha_j$, exits contribute $\sum_j\alpha_jp_{j0}$, and migrations from $k$ to $j\ne k$ contribute $\sum_{j:n_j>0}\sum_{k\ne j}g_j(n_j)\alpha_kp_{kj}/\alpha_j$. Combining the first and third contributions using the [traffic equations of an open migration process](../../../../../../traffic-equation-of-an-open-migration-process.md) yields $\sum_jg_j(n_j)(1-p_{jj})$. Summing those same [traffic equations of an open migration process](../../../../../../traffic-equation-of-an-open-migration-process.md) gives $\sum_j\alpha_jp_{j0}=\sum_j\nu_j$. The incoming rate is therefore exactly the outgoing rate

$$
\sum_j\nu_j+\sum_jg_j(n_j)(1-p_{jj}).
$$

This proves stationarity. With finite arrival rates, finite service rates in each state and transient routing, the process is nonexplosive: only finitely many individuals enter in a finite interval, and each makes finitely many routing transitions before exit, almost surely. On the accessible [irreducible Markov chain](../../../../../../irreducible-markov-chain.md), a finite normalizer gives the unique [stationary distribution](../../../../../../stationary-distribution.md) and [positive recurrence](../../../../../../positive-recurrent-markov-chain.md). Colonies with zero effective arrivals are empty in this equilibrium. For a nonempty accessible colony, a divergent $Z_j$ prevents normalization of the equilibrium weights.

For the single-server specialization, $g_j(k)=\phi_j$ for $k>0$. Each colony has the [stationary distribution of an M-M-1 queue](../../../../../../stationary-distribution-of-an-m-m-1-queue.md):

$$
\Pr\{n_j=k\}=\left(1-\frac{\alpha_j}{\phi_j}\right)\left(\frac{\alpha_j}{\phi_j}\right)^k,\qquad
\mathbb E n_j=\frac{\alpha_j}{\phi_j-\alpha_j},
$$

requiring $\phi_j>\alpha_j$ on every colony with positive traffic. The service rates do not change the [traffic equations of an open migration process](../../../../../../traffic-equation-of-an-open-migration-process.md).

For positive $\alpha_j$, write $B=F-\sum_j\alpha_j$ and $s_j=\phi_j-\alpha_j$. A stable allocation requires $B>0$ and $s_j>0$, with $\sum_js_j=B$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\left(\sum_j\sqrt{\alpha_j}\right)^2
=\left(\sum_j\sqrt{\frac{\alpha_j}{s_j}}\sqrt{s_j}\right)^2
\leq B\sum_j\frac{\alpha_j}{s_j}.
$$

Equality holds precisely when $s_j$ is proportional to $\sqrt{\alpha_j}$. Hence the unique optimal [service-capacity allocation in an open migration process](../../../../../../service-capacity-allocation-in-an-open-migration-process.md) and its mean population are

$$
\boxed{\phi_j=\alpha_j+\frac{(F-\sum_k\alpha_k)\sqrt{\alpha_j}}{\sum_k\sqrt{\alpha_k}},\qquad
\min\mathbb E\sum_jn_j=\frac{(\sum_j\sqrt{\alpha_j})^2}{F-\sum_j\alpha_j}.}
$$

There is no stable allocation when $F\leq\sum_j\alpha_j$ and some traffic is positive. If some $\alpha_j=0$, those empty colonies contribute no population; allocate the spare capacity to the positive-traffic colonies by the same rule. Allowing zero capacity at an unused colony attains this optimum. If strictly positive $\phi_j$ are required even there, the displayed value is only an infimum, approached as their capacities tend to zero. If every $\alpha_j=0$, the equilibrium is empty and any admissible allocation minimizes its mean population at zero.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
