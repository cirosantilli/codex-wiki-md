<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Construct a rate-$\lambda$ [Poisson process](../../../../../../poisson-process.md), for $\lambda>0$, from independent waiting times $E_j$ with [exponential distribution](../../../../../../exponential-distribution.md) $\operatorname{Exp}(\lambda)$. Put $S_k=E_1+\cdots+E_k$, $S_0=0$, and $N_t=\max\{k:S_k\leq t\}$. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $S_k/k\to1/\lambda$, so there are only finitely many arrivals on each finite interval. Consequently the counting paths are [càdlàg](../../../../../../cadlag.md), and $N_0=0$ [almost surely](../../../../../../almost-sure-convergence.md).

At any deterministic time $s$, the [memorylessness of the exponential distribution](../../../../../../memorylessness-of-the-exponential-distribution.md) says that the residual waiting time has again [exponential distribution](../../../../../../exponential-distribution.md) $\operatorname{Exp}(\lambda)$ and is independent of the observed history. Subsequent waiting times are fresh independent copies. Thus the [Poisson process](../../../../../../poisson-process.md) restarts independently at $s$, proving [independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md). Integrating the joint waiting-time densities over $0<s_1<\cdots<s_k\leq t<s_{k+1}$ gives

$$
\mathbb P(N_t=k)=e^{-\lambda t}\frac{(\lambda t)^k}{k!},\qquad k\geq0,
$$

so its time values have the expected [Poisson distribution](../../../../../../poisson-distribution.md).

For $h\downarrow0$,

$$
\mathbb P(N_h\ne0)=1-e^{-\lambda h}\longrightarrow0.
$$

Together with [stationary increments](../../../../../../stationary-increments.md), this gives [stochastic continuity](../../../../../../stochastic-continuity.md) at every time, from either side where applicable. All the [Lévy process](../../../../../../levy-process.md) requirements hold, and

$$
\boxed{\mathbb E e^{i\theta N_t}=\exp\{\lambda t(e^{i\theta}-1)\},\qquad\psi(\theta)=\lambda(e^{i\theta}-1).}
$$

For $\lambda=0$, the identically zero process gives the degenerate case.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
