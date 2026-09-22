<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) is a [reversible Markov chain](../../../../../../reversible-markov-chain.md) in equilibrium if, when started in a [stationary distribution](../../../../../../stationary-distribution.md) $\pi$, the process $(X_t:0\leq t\leq T)$ has the same finite-dimensional distributions as $(X_{T-t}:0\leq t\leq T)$ for every $T>0$.

For transition rates $q_{ij}$, the [detailed balance for a continuous-time Markov chain](../../../../../../detailed-balance-for-a-continuous-time-markov-chain.md) equations are

$$
\boxed{\pi_iq_{ij}=\pi_jq_{ji}\qquad(i\ne j).}
$$

They imply invariance directly. For each state $j$,

$$
\begin{aligned}
(\pi Q)_j
&=\sum_{i\ne j}\pi_iq_{ij}+\pi_jq_{jj}\\
&=\pi_j\sum_{i\ne j}q_{ji}
-\pi_j\sum_{k\ne j}q_{jk}=0,
\end{aligned}
$$

because $q_{jj}=-\sum_{k\ne j}q_{jk}$. Thus $\pi Q=0$, so $\pi$ is an [invariant distribution of a continuous-time Markov chain](../../../../../../invariant-distribution-of-a-continuous-time-markov-chain.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
