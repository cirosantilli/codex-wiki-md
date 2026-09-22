<h1 id="24k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The random clock is understood to be independent of the discrete-time [Markov chain](../../../../../../markov-chain.md); without this hypothesis its law need not be determined by $K$ alone. Conditional on $N_t=n$, the transition matrix is $K^n$, so

$$
P_t=e^{-\lambda t}\sum_{n\geq0}\frac{(\lambda t)^n}{n!}K^n=e^{\lambda t(K-I)},\qquad\boxed{Q=\lambda(K-I).}
$$

Hence $q_{xy}=\lambda K_{xy}$ for $x\ne y$ and $q_{xx}=-\lambda(1-K_{xx})$. If $\pi K=\pi$, then $\pi P_t=\pi$ by the series, proving that the [invariant distribution](../../../../../../stationary-distribution.md) is unchanged.

Let $\xi_i$ be the independent exponential interarrival times of the [Poisson process](../../../../../../poisson-process.md). The absorption time is $T_a=\sum_{i=1}^{\tau_a}\xi_i$. By independence of the chain and clock and [Tonelli theorem](../../../../../../tonelli-theorem.md),

$$
\mathbb E_xT_a=\sum_{i\geq1}\mathbb E[\xi_i]\mathbb P_x(\tau_a\geq i)=\boxed{\frac1\lambda\mathbb E_x\tau_a.}
$$

This includes infinite expectations and absorption at time zero. The same argument proves the hinted random-sum identity for an independent nonnegative integer-valued count $M$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [24K](../../24k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
