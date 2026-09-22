# Collision-path coupling for slotted ALOHA

↑ **Parent:** [Permanent collisions in constant-probability slotted ALOHA](permanent-collisions-in-constant-probability-slotted-aloha.md)

In [slotted ALOHA](slotted-aloha.md), let old packets retry independently with fixed probability $0<p<1$, and let independent [Poisson random variables](poisson-distribution.md) of mean $\nu>0$ transmit once on arrival. Write $q=1-p$ and $r=e^{-\nu p}$. A hypothetical process which never removes a packet has backlog $b+A_t$, where $A_t$ is the cumulative arrival count over $t$ slots. Couple its attempts to those of the actual process until the first noncollision. Its one-slot noncollision probability at backlog $n$ is $h(n)=e^{-\nu}[(1+\nu)q^n+npq^{n-1}]$. The [union bound](boole-s-inequality.md) and the [Poisson distribution](poisson-distribution.md) give

$$
\varepsilon(b)=e^{-\nu}q^b\left[\frac{1+\nu+bp/q}{1-r}+\frac{p\nu r}{(1-r)^2}\right].
$$

Indeed $\mathbb E[q^{A_t}]=r^t$ and $\mathbb E[A_tq^{A_t}]=\nu tq r^t$. Thus $\varepsilon(b)\to0$. From every sufficiently large backlog, permanent collisions have probability at least $1/2$. Independent arrival batches reach that threshold almost surely; after each failed attempt the [Strong Markov property](strong-markov-property.md) permits another attempt. The probability of $k$ consecutive failures is at most $2^{-k}$, proving almost-sure eventual permanent collisions without assuming in advance that the backlog escapes.

## ↑ Ancestors (10)

1. [Permanent collisions in constant-probability slotted ALOHA](permanent-collisions-in-constant-probability-slotted-aloha.md)
2. [Slotted ALOHA](slotted-aloha.md)
3. [Random access network](random-access-network.md)
4. [Stochastic network](stochastic-network.md)
5. [Queueing theory](queueing-theory-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-73/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35/3/solution.md)
