<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A random time $\tau$ is a [stopping time](../../../../../../stopping-time.md) for the [natural filtration](../../../../../../natural-filtration.md) $(\mathcal F_n)$ of a [Markov chain](../../../../../../markov-chain.md) when $\{\tau\le n\}\in\mathcal F_n$ for every $n$. The [Strong Markov property](../../../../../../strong-markov-property.md) says that, conditionally on $\tau<\infty$ and $X_\tau=i$, the process after $\tau$ is a fresh copy of the chain started from $i$, independent of the pre-$\tau$ history.

Before capture define the half-separation

$$
D_n=\frac{Z_n-Y_n}{2}.
$$

For $D_n=k\ge2$, independence of the two moves gives the [transition probabilities](../../../../../../transition-probability.md)

$$
\mathbb P(D_{n+1}=k-1\mid D_n=k)=\frac q2,
$$



$$
\mathbb P(D_{n+1}=k\mid D_n=k)=\frac12,
\qquad
\mathbb P(D_{n+1}=k+1\mid D_n=k)=\frac{1-q}{2}.
$$

Ignore the holding steps. The resulting embedded chain is a [biased random walk](../../../../../../biased-random-walk.md) that moves left with probability $q$ and right with probability $1-q$. Its expected number of moves needed to descend one level is $1/(2q-1)$; this follows either from [first-step analysis](../../../../../../first-step-analysis.md) or from its drift $1-2q$. A non-holding move occurs with probability $1/2$ at each time, so its mean waiting time is two. Hence, for every $m\ge2$, the expected time to go from separation $2m$ to $2(m-1)$ is

$$
\boxed{\mu=\frac2{2q-1}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
