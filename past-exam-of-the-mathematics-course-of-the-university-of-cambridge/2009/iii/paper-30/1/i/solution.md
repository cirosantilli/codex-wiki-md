<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $\mu=\mu_1+\mu_2$. In this [heterogeneous two-server queue](../../../../../../heterogeneous-two-server-queue.md), the total population alone is not a [Markov process](../../../../../../markov-process-split.md): when only one customer is present, its departure rate depends on which server is occupied. Use states $0,a,b,2,3,\ldots$, where $a$ and $b$ distinguish the two single-customer possibilities, and $n\geq2$ records the total population. The [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md) of the [exponential distributions](../../../../../../exponential-distribution.md) gives these nonzero transition rates:

$$
q_{0a}=q_{0b}=\nu/2,\quad q_{a0}=\mu_1,\quad q_{b0}=\mu_2,\quad q_{a2}=q_{b2}=\nu,\quad q_{2a}=\mu_2,\quad q_{2b}=\mu_1,
$$

and $q_{n,n+1}=\nu$ for $n\geq2$, $q_{n,n-1}=\mu$ for $n\geq3$. In particular, a departure from state $2$ leaves the other server occupied.

The [detailed balance equations](../../../../../../detailed-balance.md) suggest

$$
\pi_a=\frac{\nu}{2\mu_1}\pi_0,\qquad
\pi_b=\frac{\nu}{2\mu_2}\pi_0,\qquad
\pi_n=\frac{\nu^2}{2\mu_1\mu_2}\left(\frac{\nu}{\mu}\right)^{n-2}\pi_0\quad(n\geq2).
$$

For example, both $\pi_a\nu=\pi_2\mu_2$ and $\pi_b\nu=\pi_2\mu_1$ hold; these are the two transitions that would be lost by using only population as the state. All other adjacent-state [detailed balance equations](../../../../../../detailed-balance.md) hold as well. Since $\nu/\mu<1$, the [geometric series](../../../../../../geometric-series.md) converges, and normalization gives

$$
\pi_0^{-1}=1+\frac{\nu\mu}{2\mu_1\mu_2}+\frac{\nu^2\mu}{2\mu_1\mu_2(\mu-\nu)}
=1+\frac{\nu\mu^2}{2\mu_1\mu_2(\mu-\nu)}.
$$

Thus the [stationary distribution](../../../../../../stationary-distribution.md) exists, and the requested probability is

$$
\boxed{\Pr\{\text{both busy}\}=\sum_{n\geq2}\pi_n
=\frac{\nu^2\mu}{2\mu_1\mu_2(\mu-\nu)+\nu\mu^2}.}
$$

With equal server rates $\mu_1=\mu_2=m$, this reduces to $\nu^2/[m(2m+\nu)]$, as for an [M-M-s queue](../../../../../../m-m-s-queue.md) with two servers.

To prove the output claim, put the [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) in its [stationary distribution](../../../../../../stationary-distribution.md). The preceding [detailed balance equations](../../../../../../detailed-balance.md) make it a [reversible Markov chain](../../../../../../reversible-markov-chain.md): [time reversal of a continuous-time Markov chain](../../../../../../time-reversal-of-a-continuous-time-markov-chain.md) has the same transition rates. A forward departure becomes a reversed arrival. In every reversed state, the total rate of such arrivals is $\nu$: from $0$ the rates $\nu/2$ add, from $a$ or $b$ the upward rate is $\nu$, and from every $n\geq2$ it is also $\nu$. The reversed process can therefore be constructed with an independent rate-$\nu$ [Poisson process](../../../../../../poisson-process.md) of arrival epochs, choosing the idle server by a fair coin when appropriate. Consequently reversed arrival counts on disjoint time intervals are independent [Poisson random variables](../../../../../../poisson-distribution.md) with the corresponding means. Reversing those intervals proves that **the stationary departure stream is a rate-$\nu$ Poisson process**, rather than merely a stream with mean rate $\nu$.

Stationarity matters here. If the [queue](../../../../../../queue-queueing-theory.md) starts empty, a departure by time $h$ requires both an arrival and a completed [service time](../../../../../../service-time.md), so its probability is $O(h^2)$; a rate-$\nu$ [Poisson process](../../../../../../poisson-process.md) would have probability $\nu h+O(h^2)$. Thus the output assertion is the equilibrium assertion in the context of the preceding stationary calculation.

## ↑ Ancestors (11)

1. [I](../i.md)
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
