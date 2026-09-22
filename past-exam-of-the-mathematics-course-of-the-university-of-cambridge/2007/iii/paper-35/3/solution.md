<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the standard infinite-population [slotted ALOHA](../../../../../slotted-aloha.md) model with independent [Poisson random variables](../../../../../poisson-distribution.md) $Y_t$ of mean $\nu>0$ giving arrivals during slot $(t,t+1)$. Every new packet makes its first attempt in the next slot. An unsuccessful packet joins the old backlog and independently retries in each subsequent slot with a fixed probability $p$, where $0<p\leq1$. A single transmission succeeds, while two or more transmissions collide and all those packets remain. This constant retry probability is an essential assumption of the instability result; it is not a claim about every adaptive random-access protocol.

At the beginning of slot $(t,t+1)$, let $N_t$ count the previously backlogged packets, excluding the fresh batch $Y_{t-1}$ which now makes its first attempt. Given $N_t=n$, the old attempts have the [binomial distribution](../../../../../binomial-distribution.md) $\operatorname{Bin}(n,p)$, independently of the fresh [Poisson random variable](../../../../../poisson-distribution.md). Let $T_t$ be the total number of attempts. The feedback $Z_t$ records zero attempts, one attempt, or a collision. Adding the fresh packets and subtracting the one departure if there is a success gives

$$
\boxed{N_{t+1}=N_t+Y_{t-1}-\mathbf1_{\{Z_t=1\}}.}
$$

Thus $N_t$ is an old-packet backlog, not the number of transmitters in the slot. Fresh attempts and retry attempts are both included in $T_t$ and hence in the feedback $Z_t$.

First take $0<p<1$ and write $q=1-p$. Conditional on old backlog $n$, a noncollision is either no attempt, or precisely one attempt. Independence and the [Poisson distribution](../../../../../poisson-distribution.md) give its probability as

$$
h(n)=\mathbb P(T_t\leq1\mid N_t=n)=e^{-\nu}\big[(1+\nu)q^n+npq^{n-1}\big],
$$

where the last term is zero for $n=0$. The two contributions to one attempt are one fresh packet with no old attempt, or one old attempt with no fresh packet.

To prove [permanent collisions in constant-probability slotted ALOHA](../../../../../permanent-collisions-in-constant-probability-slotted-aloha.md), consider a process which starts with $b$ old packets and is forced never to remove a packet. Before its $k$th future slot its backlog is $b+A_k$, where $A_k$ is the sum of the first $k$ fresh arrival batches, so $A_k$ has the [Poisson distribution](../../../../../poisson-distribution.md) with mean $\nu k$. Generate its packet-attempt coins and the actual system's coins on the same probability space, using the same coins for the same packets. Until the first noncollision, every actual slot collides and removes nothing, so the two processes agree exactly. In particular, a sample path on which the hypothetical process always collides is a permanent-collision sample path for the actual system. This is the [collision-path coupling for slotted ALOHA](../../../../../collision-path-coupling-for-slotted-aloha.md).

The [union bound](../../../../../boole-s-inequality.md), without any assumption of independence between future noncollision events, bounds the probability of at least one such event by

$$
\sum_{k=0}^{\infty}\mathbb E[h(b+A_k)].
$$

Put $r=e^{-\nu p}<1$. The [moment-generating function](../../../../../moment-generating-function.md) of the [Poisson distribution](../../../../../poisson-distribution.md) and its derivative give

$$
\mathbb E[q^{A_k}]=r^k,\qquad \mathbb E[A_kq^{A_k}]=\nu kq r^k.
$$

Consequently the [collision-path coupling for slotted ALOHA](../../../../../collision-path-coupling-for-slotted-aloha.md) yields the explicit bound

$$
\mathbb P_b(\text{some future noncollision})\leq\varepsilon(b)=e^{-\nu}q^b\left[\frac{1+\nu+bp/q}{1-r}+\frac{p\nu r}{(1-r)^2}\right].
$$

The geometric decay of $q^b$ dominates the linear factor in $b$, so $\varepsilon(b)\to0$. Choose an integer $K$ so that $\varepsilon(b)\leq1/2$ for every $b\geq K$. From every such backlog, the conditional probability that all future slots collide is at least $1/2$.

It remains to show that this positive probability implies an almost-sure eventual escape into permanent collisions. From any finite state, wait for an arrival batch containing at least $K+2$ packets. Its probability in each slot is the strictly positive constant $\mathbb P\{\operatorname{Poisson}(\nu)\geq K+2\}$. Independent arrival batches ensure that the waiting time is almost surely finite. That arrival batch forces a collision, and the next old backlog is at least $K$. Starting there, observe slots until the first noncollision. If none occurs, the desired event has happened. If one occurs, this failure is observed at a finite stopping time; wait for another sufficiently large arrival batch and start another attempt. The [Strong Markov property](../../../../../strong-markov-property.md), or simply the independence of the fresh arrival variables and packet-attempt coins after each such stopping time, gives conditional failure probability at most $1/2$ at every attempt. Therefore the probability that the first $m$ attempts all fail is at most $2^{-m}$. Infinite failures have probability zero, proving

$$
\boxed{\mathbb P\{\exists J<\infty:\ Z_t=*\text{ for every }t\geq J\}=1.}
$$

This argument proves the required almost-sure assertion, rather than merely positive drift or a small one-slot success probability.

If $p=1$, a batch of at least two fresh packets occurs almost surely. The batch collides, leaving at least two old packets; both retry in every subsequent slot, so all subsequent slots collide. Thus the same conclusion holds. At $p=0$ the conclusion fails: old packets never transmit, and fresh batches of size zero or one occur infinitely often. This explains why positive retry probability was included in the model.

A conventional finite-population [slotted ALOHA](../../../../../slotted-aloha.md) model behaves differently. Suppose there are at most $M$ old packets, each retries with probability $0<p<1$, and there is a conditional probability at least $\delta>0$ of no fresh attempts in each slot. The probability of an idle slot, conditional on the entire past, is then at least $\delta(1-p)^M=\eta>0$. Iterating conditional probabilities gives

$$
\mathbb P(Z_t=*\text{ for }t=j,\ldots,j+k-1)\leq(1-\eta)^k.
$$

For each fixed $j$, the probability of collisions forever after $j$ is zero. A countable union over $j$ shows that eventual permanent collisions have probability zero. This is the [finite-population exclusion of permanent ALOHA collisions](../../../../../finite-population-exclusion-of-permanent-aloha-collisions.md). A finite model can still spend long periods in a heavily backlogged state, but its bounded backlog removes the mechanism by which the infinite-population idle and success probabilities tend to zero. Degenerate finite protocols, such as all backlogged stations retrying with probability one, can have absorbing collision states; a finite population alone does not exclude those.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
