<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a fixed occupancy $n$, let $x_r>0$ be the per-flow rate on every active route, so feasibility means $\sum_{r:j\in r}n_rx_r\leq C_j$. A [proportionally fair allocation](../../../../../proportional-fairness.md) is a feasible allocation satisfying, for every other feasible $\widetilde x$,

$$
\boxed{\sum_{r:n_r>0}n_r\frac{\widetilde x_r-x_r}{x_r}\leq0.}
$$

The sum counts the proportional changes over individual flows. By the first-order condition for a [concave function](../../../../../concave-function.md), it is exactly the allocation solving

$$
\boxed{\max_{x>0}\sum_{r:n_r>0}n_r\log x_r
\quad\text{subject to}\quad\sum_{r:j\in r}n_rx_r\leq C_j\quad(j\in J).}
$$

This is [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) optimization, and its negative objective is a [strictly convex function](../../../../../strictly-convex-function.md), which gives unique rates on active routes. Routes with $n_r=0$ have no per-flow rate to determine.

Index the four routes by $1=\{1,2\}$, $2=\{2,3\}$, $3=\{3,4\}$, $4=\{4,1\}$, and let $\Lambda_r=n_rx_r$ be each route's total service. Write

$$
P=n_1+n_3,\qquad Q=n_2+n_4,\qquad N=P+Q.
$$

The four capacity constraints say $\Lambda_1+\Lambda_2\leq1$, $\Lambda_2+\Lambda_3\leq1$, $\Lambda_3+\Lambda_4\leq1$, and $\Lambda_4+\Lambda_1\leq1$. Equivalently,

$$
\max(\Lambda_1,\Lambda_3)+\max(\Lambda_2,\Lambda_4)\leq1.
$$

For fixed maxima $u,v$, every active route in the first group optimally takes total service $u$, and every active route in the second takes $v$, because its logarithmic objective is increasing. Up to the constant $-\sum_rn_r\log n_r$, the objective therefore becomes $P\log u+Q\log v$ with $u+v\leq1$. Its maximizer is $u=P/N$, $v=Q/N$ when $N>0$, with the evident endpoint choices when one group is empty. Hence the [proportionally fair allocation on a four-cycle](../../../../../proportionally-fair-allocation-on-a-four-cycle.md) is

$$
\boxed{x_r=\begin{cases}
P/(Nn_r),&r\in\{1,3\},\ n_r>0,\\
Q/(Nn_r),&r\in\{2,4\},\ n_r>0.
\end{cases}}
$$

Set $\Lambda_r=0$ on inactive routes. If $N=0$, all service totals are zero. In particular, for $n_1>0$, $n_1x_1=P/N$, as required. Two disjoint active routes in the same group can each receive the same total service; service totals need not sum to one over the entire network.

With independent document arrivals given by [Poisson processes](../../../../../poisson-process.md) of rates $\rho_r$ and independent unit-mean [exponential distributions](../../../../../exponential-distribution.md) for document sizes, each of the $n_r$ active documents has completion rate $x_r$. The [flow-level network model](../../../../../flow-level-network-model.md) is consequently a [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) with

$$
\boxed{q(n,n+e_r)=\rho_r,\qquad
q(n,n-e_r)=\begin{cases}
P/N,&r\in\{1,3\},\ n_r>0,\\
Q/N,&r\in\{2,4\},\ n_r>0,\\
0,&n_r=0.
\end{cases}}
$$

At $n=0$ all downward rates are zero. The total departure rate is at most four, so the bounded total jump rate ensures no explosion.

The original PDF's displayed factor is a [binomial coefficient](../../../../../binomial-coefficient.md), not the plain quotient produced by the TeX extraction. The candidate [stationary distribution](../../../../../stationary-distribution.md) for this [reversible four-cycle flow model](../../../../../reversible-four-cycle-flow-model.md) is

$$
\boxed{\pi(n)=B^{-1}\binom{N}{P}\prod_{r=1}^4\rho_r^{n_r},\qquad
B=\sum_{n\in\mathbb Z_{\geq0}^4}\binom{N}{P}\prod_r\rho_r^{n_r}.}
$$

Use $\binom00=1$. For $r\in\{1,3\}$ and $n_r>0$,

$$
\frac{\pi(n)}{\pi(n-e_r)}
=\rho_r\frac{\binom NP}{\binom{N-1}{P-1}}
=\rho_r\frac NP,
$$

so $\pi(n)q(n,n-e_r)=\pi(n-e_r)\rho_r$. For $r\in\{2,4\}$ the corresponding ratio is $\rho_rN/Q$. Thus [detailed balance for a continuous-time Markov chain](../../../../../detailed-balance-for-a-continuous-time-markov-chain.md) holds for every adjacent pair, proving the displayed [stationary distribution](../../../../../stationary-distribution.md) whenever $B<\infty$.

For completeness, its existence condition can be made explicit. Put $\alpha=\max(\rho_1,\rho_3)$ and $\beta=\max(\rho_2,\rho_4)$. At fixed $P,Q$,

$$
\sum_{n_1+n_3=P}\rho_1^{n_1}\rho_3^{n_3}\leq(P+1)\alpha^P,\qquad
\sum_{n_2+n_4=Q}\rho_2^{n_2}\rho_4^{n_4}\leq(Q+1)\beta^Q.
$$

Therefore the sum over states with $N=m$ is at most $(m+1)^2(\alpha+\beta)^m$, using the [binomial theorem](../../../../../binomial-theorem.md). This is summable if $\alpha+\beta<1$. Conversely, restricting to the single maximizing route in each group leaves the series $\sum_{m\geq0}(\alpha+\beta)^m$, which diverges if $\alpha+\beta\geq1$. Hence

$$
\boxed{B<\infty\iff\max(\rho_1,\rho_3)+\max(\rho_2,\rho_4)<1
\iff\rho_1+\rho_2,\ \rho_2+\rho_3,\ \rho_3+\rho_4,\ \rho_4+\rho_1<1.}
$$

These are exactly the four strict resource-load inequalities. With positive arrival rates the [Markov chain](../../../../../markov-chain.md) is irreducible, so the normalized [stationary distribution](../../../../../stationary-distribution.md) is unique.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 213](../../paper-213-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
