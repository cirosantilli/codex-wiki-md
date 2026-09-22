<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $(\tau_n)$ be a [localizing sequence](../../../../../../localizing-sequence.md) for $M$. For $s\leq t$, the [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
\mathbb E[M_{t\wedge\tau_n}\mid\mathcal F_s]=M_{s\wedge\tau_n}.
$$

Both sides converge almost surely to $M_t$ and $M_s$, and $|M_{u\wedge\tau_n}|\leq Z$. Conditional dominated convergence therefore yields $\mathbb E[M_t\mid\mathcal F_s]=M_s$, so $M$ is a [martingale](../../../../../../martingale-split.md). Moreover, the family $(M_t)_{t\geq0}$ is dominated by the integrable random variable $Z$, hence is [uniformly integrable](../../../../../../uniform-integrability.md). Thus **$M$ is a uniformly integrable martingale**.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
