<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [continuous local martingale](../../../../../../continuous-local-martingale.md) $M$, its **[stochastic exponential](../../../../../../doleans-dade-exponential.md)** is

$$
\boxed{Z_t=\mathcal E(M)_t=\exp\{M_t-M_0-\tfrac12[M]_t\}.}
$$

The [Itô formula](../../../../../../ito-s-lemma.md) gives $dZ_t=Z_t\,dM_t$ and $Z_0=1$, so $Z$ is a strictly positive [local martingale](../../../../../../local-martingale.md). The finite-horizon **[Girsanov theorem](../../../../../../girsanov-theorem.md)** says: if $Z$ is a true [martingale](../../../../../../martingale-split.md) on $[0,T]$ and $d\widetilde{\mathbb P}=Z_T\,d\mathbb P$ on $\mathcal F_T$, then for every [continuous local martingale](../../../../../../continuous-local-martingale.md) $N$ under $\mathbb P$,

$$
\boxed{\widetilde N_t=N_t-[N,M]_t\text{ is a }\widetilde{\mathbb P}\text{-local martingale},\quad 0\leq t\leq T.}
$$

For an infinite-horizon [change of measure](../../../../../../change-of-measure.md), assume $Z$ is a [uniformly integrable](../../../../../../uniform-integrability.md) [martingale](../../../../../../martingale-split.md) and use its terminal density $Z_\infty$. In particular, if $M=\int\theta\,dB$, the process $\widetilde B=B-\int\theta\,ds$ is [Brownian motion](../../../../../../brownian-motion-split.md) under the new [probability measure](../../../../../../probability-measure.md), by the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md).

**The [quadratic variation](../../../../../../quadratic-variation.md) cannot change.** Adding the continuous [finite-variation process](../../../../../../finite-variation-process.md) $-[N,M]$ leaves $[\widetilde N]=[N]$. Also the same pathwise partition sums defining $[N]$ have the same limit under an absolutely continuous [change of measure](../../../../../../change-of-measure.md); convergence in [probability](../../../../../../probability.md) transfers by integrability of the density. Thus the bracket of the unchanged process $N$, now a [semimartingale](../../../../../../semimartingale.md), is also unchanged. The [local martingale](../../../../../../local-martingale.md) property itself need not survive. This is [quadratic covariation under an absolutely continuous measure change](../../../../../../quadratic-covariation-under-an-absolutely-continuous-measure-change.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
