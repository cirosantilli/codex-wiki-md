<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

All specified nearest-neighbour probabilities are positive, making the [birth-death chain](../../../../../birth-death-chain.md) irreducible. The row sums give $p_0+q_0=1$ and $p_i+q_i=1$ for $i\ge1$. Write $T_j$ for the hitting time of $j$, and on $\{0,\ldots,N\}$ let $h_i=\Pr_i(T_N<T_0)$. The first-step equations give

$$
h_0=0,\quad h_N=1,\quad
p_i(h_{i+1}-h_i)=q_i(h_i-h_{i-1})\quad(1\le i<N).
$$

Define $\rho_0=1$ and $\rho_k=\prod_{r=1}^kq_r/p_r$. The successive increments are proportional to $\rho_k$, and normalization at $N$ yields

$$
h_i=\frac{\sum_{k=0}^{i-1}\rho_k}{\sum_{k=0}^{N-1}\rho_k},\qquad
\Pr_1(T_N<T_0)=\frac1{\sum_{k=0}^{N-1}\rho_k}.
$$

The chain cannot remain forever in a fixed finite set avoiding zero: from every state in that set there is a uniformly positive chance to leave or hit zero within finitely many steps, so iterating the [Markov property](../../../../../markov-property.md) makes indefinite confinement have probability zero. Thus avoiding zero is the limit event of hitting every upper boundary before zero. Sending $N\to\infty$ shows that the probability of never hitting zero from one vanishes exactly when $\sum_k\rho_k=\infty$. At zero, return is immediate with probability $q_0$ and otherwise begins an excursion from one; irreducibility then gives

$$
\boxed{\text{recurrence}\iff\sum_{n\ge1}\prod_{r=1}^n\frac{q_r}{p_r}=\infty.}
$$

For [positive recurrence](../../../../../positive-recurrent-markov-chain.md) define $w_0=1$ and $w_n=\prod_{r=1}^np_{r-1}/q_r$. First assume recurrence and let $\tau=T_0^+$ be the first return from zero. For each fixed $i$, the expected number $m_i$ of visits to $i$ before $\tau$ is finite: each visit to $i\ge1$ has a positive chance of following the successive downward steps to zero before another visit, so its visit count has a geometric tail. Also $m_0=1$.

Each finite excursion starts and ends below every edge $(i,i+1)$, so its upward and downward crossing counts of that edge are equal. Their expectations, by the [Markov property](../../../../../markov-property.md), are $m_ip_i$ and $m_{i+1}q_{i+1}$. Hence $m_{i+1}=m_ip_i/q_{i+1}$ and $m_i=w_i$. [Tonelli's theorem](../../../../../tonelli-theorem.md) applied to the nonnegative occupation counts gives the [excursion weights of a reflected birth-death chain](../../../../../excursion-weights-of-a-reflected-birth-death-chain.md) formula

$$
\mathbb E_0\tau=\sum_{i\ge0}m_i=\sum_{i\ge0}w_i.
$$

Consequently [positive recurrence](../../../../../positive-recurrent-markov-chain.md) implies the requested finite sum. Conversely, if $\sum_iw_i<\infty$, then $w_i\to0$. But $\rho_iw_i=p_0/p_i\ge p_0$, so $\rho_i\ge p_0/w_i\to\infty$ and the already proved recurrence criterion holds. The occupation calculation is therefore valid and gives a finite mean return time. Thus

$$
\boxed{\text{positive recurrence}\iff\sum_{n\ge1}\prod_{r=1}^n\frac{p_{r-1}}{q_r}<\infty.}
$$

Adding the finite $w_0=1$ term does not change convergence.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
