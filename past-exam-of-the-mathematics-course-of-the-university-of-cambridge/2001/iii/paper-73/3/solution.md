<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the constant-retry version of [slotted ALOHA](../../../../../slotted-aloha.md). Fresh packets arrive in each slot as independent [Poisson random variables](../../../../../poisson-distribution.md) $Y_t$ of mean $\nu>0$, and each first attempts in the next slot. Every already backlogged packet independently retries with the same fixed probability $0<p<1$ each slot. Transmission choices are independent of arrivals and past choices. Let $N_t$ be the number of old backlogged packets just before the slot $(t,t+1)$, excluding the fresh $Y_{t-1}$ packets about to make their first attempt. The number of attempts is $\operatorname{Bin}(N_t,p)+Y_{t-1}$, and $Z_t$ records zero, one, or at least two attempts. Exactly one attempt succeeds and leaves; otherwise every fresh packet becomes backlogged. Therefore

$$
\boxed{N_{t+1}=N_t+Y_{t-1}-\mathbf1_{\{Z_t=1\}}.}
$$

The arrivals $Y_{t-1}$ are independent of $N_t$, since that backlog depends only on earlier arrivals and choices. This convention explains the displayed one-slot index shift.

A throughput bound or positive drift alone does not prove eventual collisions in every slot. Instead use the [collision-path coupling for slotted ALOHA](../../../../../collision-path-coupling-for-slotted-aloha.md). Set $q=1-p$. Given old backlog $n$, the probability of a noncollision, namely zero or one total attempts, is

$$
h(n)=e^{-\nu}\left[(1+\nu)q^n+npq^{n-1}\right].
$$

The terms represent no fresh attempts and zero old attempts, one fresh attempt and no old attempts, or one old attempt and no fresh attempts. Start from backlog $b$ and couple to a hypothetical process in which no packet is ever removed. Until the first noncollision the two processes agree; after $t$ slots the hypothetical old backlog is $b+A_t$, where $A_t$ is the sum of $t$ independent arrivals and hence has [Poisson distribution](../../../../../poisson-distribution.md) of mean $\nu t$.

A first noncollision of the real process must therefore be a noncollision in this coupled process. The [union bound](../../../../../boole-s-inequality.md) gives

$$
\Pr_b\{\text{some future noncollision}\}\leq\sum_{t=0}^\infty\mathbb E[h(b+A_t)].
$$

Writing $r=e^{-\nu p}<1$, the Poisson generating function gives $\mathbb E[q^{A_t}]=r^t$ and $\mathbb E[A_tq^{A_t}]=\nu tq\,r^t$. Sum the geometric series and its derivative to obtain

$$
\varepsilon(b)=e^{-\nu}q^b\left[\frac{1+\nu+bp/q}{1-r}+\frac{p\nu r}{(1-r)^2}\right],\qquad \Pr_b\{\text{some future noncollision}\}\leq\varepsilon(b).
$$

Since $q^b$ decays exponentially while the bracket grows only linearly, choose a finite threshold $b_0$ such that $\varepsilon(b)\leq\tfrac12$ for every $b\geq b_0$. Thus from any such backlog, there is conditional probability at least $\tfrac12$ that every subsequent slot collides.

It remains to show that opportunities to use this bound recur, without assuming backlog transience. An arrival batch $Y_{t-1}\geq b_0+1$ forces $N_{t+1}\geq b_0$, since at most one packet departs. Such a batch has strictly positive probability independently in each slot; the waiting time for one is finite almost surely, even after a stopping time. At the first visit to backlog at least $b_0$, begin an attempt at permanent collisions. If it fails, its first noncollision occurs at a finite stopping time; after that, another large arrival batch reaches the threshold and we start again. The [Strong Markov property](../../../../../strong-markov-property.md) gives conditional failure probability at most $\tfrac12$ for each attempt. The probability of $k$ consecutive failures is consequently at most $2^{-k}$. Letting $k$ tend to infinity proves

$$
\boxed{\Pr\{\exists J<\infty:\ Z_t=*\text{ for every }t\geq J\}=1.}
$$

For $p=1$, after a slot with at least two fresh packets the next old backlog is at least two, and all old packets retry forever; this gives the same conclusion. For $p=0$ the assertion is false. It also must not be applied to all adaptive protocols: [backlog-aware ALOHA with arrival-adjusted attempt probabilities](../../../../../backlog-aware-aloha-with-arrival-adjusted-attempt-probabilities.md) can be stable for sufficiently small arrival rates. The fixed-retry assumption is part of this mathematical model.

In a standard finite-population model, each of at most $M$ stations holds one pending packet, or at most one packet per station may attempt in a slot. Suppose fresh transmission probabilities are bounded below one and retries use $0<p<1$. There is then a uniform positive conditional probability $\delta$ of no fresh attempts; all old packets stay silent with probability at least $q^M$. Thus a slot is idle with conditional probability at least $\delta q^M>0$, regardless of the past. The chance that the next $k$ slots all collide is at most $(1-\delta q^M)^k$. Let $k\to\infty$ and take the countable union over possible starting slots: **eventual permanent collisions have probability zero**. This is [finite-population exclusion of permanent ALOHA collisions](../../../../../finite-population-exclusion-of-permanent-aloha-collisions.md). Degenerate rules such as retry probability one can instead give absorbing collisions, so this conclusion needs the stated nondegeneracy conditions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
