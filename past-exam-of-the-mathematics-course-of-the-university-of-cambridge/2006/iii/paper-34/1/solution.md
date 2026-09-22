<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use finitely many colonies and let $n_i$ be the population of colony $i$. An [open migration process](../../../../../open-migration-process.md) has independent external [Poisson processes](../../../../../poisson-process.md) of rates $\nu_i$, local total departure rates $\phi_i(n_i)$, and fixed routing probabilities $p_{ij}$ to other colonies and $p_{i0}$ out of the system. Here $\phi_i(0)=0$, $0<\phi_i(k)<\infty$ for $k\geq1$, $p_{ii}=0$ and $p_{i0}+\sum_jp_{ij}=1$. The [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) has intensities

$$
q(n,n+e_i)=\nu_i,\qquad q(n,n-e_i)=\phi_i(n_i)p_{i0},\qquad q(n,n-e_i+e_j)=\phi_i(n_i)p_{ij}.
$$

Require the routing matrix $P$ to be transient: every individual eventually exits. For finitely many colonies this is equivalent to every colony having a directed path to an exit. Restrict to colonies reachable from external arrivals, so their traffic rates are positive and the relevant chain is [irreducible](../../../../../irreducible-representation.md). The total population cannot exceed its initial value plus the number of external arrivals, so on any finite time interval it is bounded by a finite random number. There are only finitely many states below that bound and finite rates in each, proving [nonexplosion](../../../../../nonexplosion-of-a-continuous-time-markov-chain.md) even when the departure functions grow rapidly.

The [traffic equations of an open migration process](../../../../../traffic-equation-of-an-open-migration-process.md), in row-vector form, are

$$
\alpha=\nu+\alpha P,\qquad\alpha=\nu(I-P)^{-1}.
$$

Transience makes the inverse $\sum_{k\geq0}P^k$ finite. Define

$$
b_i(k)=\frac{\alpha_i^k}{\prod_{h=1}^k\phi_i(h)},\qquad Z_i=\sum_{k\geq0}b_i(k),\qquad b_i(0)=1.
$$

Provided every $Z_i$ is finite, the candidate [product-form stationary distribution of an open migration process](../../../../../product-form-stationary-distribution-of-an-open-migration-process.md) is

$$
\boxed{\pi(n)=\prod_i Z_i^{-1}\frac{\alpha_i^{n_i}}{\prod_{h=1}^{n_i}\phi_i(h)}.}
$$

The normalizability condition is exactly $Z_i<\infty$ for every active colony. For example, constant total service $\phi_i(k)=\mu_i$ for $k>0$ requires $\alpha_i<\mu_i$ and gives a [geometric distribution](../../../../../geometric-distribution.md); independent individual departures $\phi_i(k)=k\mu_i$ give a [Poisson distribution](../../../../../poisson-distribution.md) of mean $\alpha_i/\mu_i$. In the irreducible case the normalizable invariant law is the unique equilibrium. If the weights cannot be normalized, no stationary probability law exists, by uniqueness up to scale of invariant measures for an irreducible recurrent chain.

We establish both stationarity and the [time reversal of an open migration process](../../../../../time-reversal-of-an-open-migration-process.md) assertion by adjacent-weight calculations. Define

$$
q^*(n,m)=\frac{\pi(m)q(m,n)}{\pi(n)}\qquad(m\ne n).
$$

The identity $b_i(k)\phi_i(k)=\alpha_i b_i(k-1)$ gives

$$
\begin{aligned}
q^*(n,n+e_i)&=\alpha_i p_{i0},\\
q^*(n,n-e_i)&=\phi_i(n_i)\frac{\nu_i}{\alpha_i},\\
q^*(n,n-e_i+e_j)&=\phi_i(n_i)\frac{\alpha_jp_{ji}}{\alpha_i}.
\end{aligned}
$$

Thus the proposed [time reversal of an open migration process](../../../../../time-reversal-of-an-open-migration-process.md) retains the local service functions and has

$$
\boxed{\nu_i^*=\alpha_i p_{i0},\qquad p_{i0}^*=\nu_i/\alpha_i,\qquad p_{ij}^*=\alpha_jp_{ji}/\alpha_i.}
$$

The traffic equation for colony $i$ implies $p_{i0}^*+\sum_jp_{ij}^*=1$. Summing all traffic equations also gives $\sum_i\nu_i^*=\sum_i\nu_i$. Therefore the total outgoing rate from every state is the same for $q^*$ and $q$:

$$
\sum_{m\ne n}q^*(n,m)=\sum_i\nu_i+\sum_i\phi_i(n_i)=\sum_{m\ne n}q(n,m).
$$

Consequently $\sum_{m\ne n}\pi(m)q(m,n)=\pi(n)\sum_{m\ne n}q(n,m)$, proving [global balance for a continuous-time Markov chain](../../../../../global-balance-for-a-continuous-time-markov-chain.md). The same weight recurrence gives $\mathbb E_\pi\phi_i(n_i)=\alpha_i$, so the stationary mean total jump rate is finite. The candidate is a [stationary distribution](../../../../../stationary-distribution.md), and the displayed intensities are indeed its stationary [time reversal of a continuous-time Markov chain](../../../../../time-reversal-of-a-continuous-time-markov-chain.md). Reverse routing is also open: reverse an original arrival-to-colony path to obtain a path to a colony with $p_{i0}^*>0$.

For the last request, let $S$ be all colonies reachable by routing from $k$, including $k$ itself. The no-return-path hypothesis gives $j\notin S$. By construction no routing edge leads from $S$ to its complement $C$. The populations in $C$ therefore evolve autonomously as an [open migration process](../../../../../open-migration-process.md), with moves into $S$ treated as exits. Its stationary marginal is the corresponding product of the factors above. Retain the original destination as a mark on each such exit.

In this autonomous process, a marked exit $j\to k$ has intensity $\phi_j(n_j)p_{jk}$. The same reversed-weight calculation makes its reverse a marked external immigration channel of constant rate $\alpha_jp_{jk}$. External immigration channels can be constructed as independent [Poisson processes](../../../../../poisson-process.md). Stationary reversal of a two-sided [Poisson process](../../../../../poisson-process.md) preserves its law, so reversing this immigration channel gives

$$
\boxed{\text{The stationary }j\to k\text{ stream is Poisson with rate }\alpha_jp_{jk}.}
$$

This [Poisson migration stream without a return path](../../../../../poisson-migration-stream-without-a-return-path.md) argument is needed because a general internal migration stream in a network with feedback is not automatically Poisson. A zero routing probability gives the empty Poisson stream of rate zero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
