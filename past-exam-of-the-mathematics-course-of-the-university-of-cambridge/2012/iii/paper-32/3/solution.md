<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the standard infinite-population [slotted ALOHA](../../../../../slotted-aloha.md) model with independent fresh arrivals with [Poisson distribution](../../../../../poisson-distribution.md) $Y_t\sim\operatorname{Poisson}(\lambda)$, $\lambda>0$. Newly arrived packets attempt in the next slot. Given $N_t=n$ old backlogged packets, each independently attempts with fixed probability $f$, so the retransmission count has [binomial distribution](../../../../../binomial-distribution.md) $R_t\sim\operatorname{Binomial}(n,f)$, independent of $Y_t$ and earlier random choices. Let $Z_t$ record whether $R_t+Y_t$ is zero, one, or at least two. A single transmission succeeds and departs; a collision makes every transmitted packet remain. Therefore

$$
N_{t+1}=N_t+Y_t-S_t,\qquad S_t=\mathbf1\{R_t+Y_t=1\}.
$$

Only the present backlog determines the law of the next independent choices, so $N_t$ is a time-homogeneous [Markov chain](../../../../../markov-chain.md).

For $0<f<1$, put $q=1-f$ and $b_n=n f q^{n-1}$, with $b_0=0$. Its nonzero [transition probabilities](../../../../../transition-probability.md) are

$$
\begin{aligned}
p_{n,n-1}&=e^{-\lambda}b_n\quad(n\geq1),\\
p_{n,n}&=e^{-\lambda}(1-b_n+\lambda q^n),\\
p_{n,n+1}&=e^{-\lambda}\lambda(1-q^n),\\
p_{n,n+k}&=e^{-\lambda}\frac{\lambda^k}{k!}\quad(k\geq2).
\end{aligned}
$$

For example, a single fresh arrival leaves the backlog unchanged only if no old packet transmits; if an old packet also transmits, that fresh arrival becomes a new backlogged packet. These cases explain the extra diagonal term and the suppressed one-step increase at $n=0$. At $f=1$ the same formulas hold with $q^0=1$, $b_1=1$ and $b_n=0$ for $n\ne1$.

Here is an almost-sure proof of [permanent collisions in constant-probability slotted ALOHA](../../../../../permanent-collisions-in-constant-probability-slotted-aloha.md) for $0<f<1$, rather than just a positive-drift heuristic. For $\theta>0$, the conditional exponential increment is

$$
\mathbb E[e^{-\theta(N_{t+1}-N_t)}\mid N_t=n]=e^{\lambda(e^{-\theta}-1)}+(e^{\theta}-1)e^{-\lambda}[b_n+\lambda e^{-\theta}q^n].
$$

As $n\to\infty$ this tends to a number strictly below one. Choose $M\geq1$ so the expression is at most one for $n\geq M$. Stopping $e^{-\theta N_t}$ when the chain first enters $\{0,\ldots,M-1\}$ gives a nonnegative [supermartingale](../../../../../supermartingale.md). Downward jumps have size at most one, so it hits at $M-1$. [Optional sampling theorem for a supermartingale](../../../../../optional-sampling-theorem-for-a-supermartingale.md), first at bounded times and then by a limit, yields the [exponential-supermartingale escape bound](../../../../../exponential-supermartingale-escape-bound.md)

$$
\mathbb P_n\{\text{ever enter }\{0,\ldots,M-1\}\}\leq e^{-\theta(n-M+1)}<1\quad(n\geq M).
$$

This is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md): every positive state can successively decrease to zero, and from zero Poisson batches reach every state at least two, with state one then reached from two. An irreducible [recurrent Markov chain](../../../../../recurrent-markov-chain.md) would hit that finite set with probability one from every state, contradicting the bound. Hence every state is a [transient state](../../../../../transient-state.md), every finite set is visited only finitely often, and $N_t\to\infty$ almost surely.

The conditional success probability is $p(N_t)=e^{-\lambda}(b_{N_t}+\lambda q^{N_t})\to0$. The centered success indicators form a [martingale difference sequence](../../../../../martingale-difference-sequence.md) with bounded increments. The [strong law for martingales with bounded increments](../../../../../strong-law-for-martingales-with-bounded-increments.md) gives

$$
\frac1t\sum_{u<t}[S_u-p(N_u)]\longrightarrow0.
$$

The conditional means have Cesàro average zero, while the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives $t^{-1}\sum_{u<t}Y_u\to\lambda$. Therefore $N_t/t\to\lambda$ almost surely. Finally

$$
\mathbb P(Z_t\ne *\mid N_t)=e^{-\lambda}[(1+\lambda)q^{N_t}+b_{N_t}]
$$

decays exponentially along this linear backlog growth. Its sum over $t$ is almost surely finite. The [Conditional Borel-Cantelli lemma](../../../../../conditional-borel-cantelli-lemma.md) then implies that only finitely many slots have zero or one transmission. **Thus $\boxed{\mathbb P(\exists J:\ Z_t=*\text{ for every }t\geq J)=1}$.** At $f=1$, a fresh batch of size at least two eventually occurs, after which at least two old packets retransmit in every slot, giving the same conclusion directly.

The qualification $f>0$ is essential: if $f=0$, then $Z_t$ depends only on the independent Poisson arrivals, and zero- or one-arrival slots occur infinitely often. Positive mean arrival rate alone, without the Poisson model or another assumption allowing collisions to develop, would also be insufficient: Bernoulli fresh arrivals and initial backlog zero never collide.

One alternative is [binary exponential backoff](../../../../../binary-exponential-backoff.md): after $k$ collisions a packet selects a waiting time uniformly from $\{0,\ldots,2^k-1\}$ and tries when its counter expires. Its attempt behavior depends on its collision history, rather than a common constant $f$. Another possibility, if a backlog estimate $\widehat N_t$ is available, is to set the attempt probability near $1/\widehat N_t$, keeping the offered retransmission count near one. These descriptions illustrate adaptive access rules; they do not assert that every backoff variant is stable at arbitrary load.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
