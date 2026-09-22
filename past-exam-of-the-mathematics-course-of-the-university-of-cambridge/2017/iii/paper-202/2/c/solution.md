<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The relevant fact is [uniform convergence on compacts in probability under an absolutely continuous measure change](../../../../../../uniform-convergence-on-compacts-in-probability-under-an-absolutely-continuous-measure-change.md). Write $Z=d\widetilde{\mathbb P}/d\mathbb P$. For any event $E$ and $K>0$,

$$
\widetilde{\mathbb P}(E)\leq K\mathbb P(E)+\mathbb E_{\mathbb P}[Z\mathbf1_{\{Z>K\}}].
$$

The last term tends to zero as $K\to\infty$ because $Z$ is integrable. Consequently, $\mathbb P(E_n)\to0$ implies $\widetilde{\mathbb P}(E_n)\to0$. Apply this to $E_n=\{\sup_{t\leq T}|C_t^n-[M,N]_t|>\varepsilon\}$ for each finite $T$ and $\varepsilon>0$. The given dyadic sums therefore have the same [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md) limit under the new [probability measure](../../../../../../probability-measure.md).

This proves [quadratic covariation under an absolutely continuous measure change](../../../../../../quadratic-covariation-under-an-absolutely-continuous-measure-change.md):

$$
\boxed{[M,N]^{\widetilde{\mathbb P}}=[M,N]^{\mathbb P}\quad\text{up to }\widetilde{\mathbb P}\text{-indistinguishability}.}
$$

Taking $N=M$ proves the corresponding [quadratic variation](../../../../../../quadratic-variation.md) assertion directly; it has not been assumed. The ceiling in the printed sum includes one grid interval extending beyond $t$. This does not affect the limit: on $[0,T]$ the resulting extra product is bounded by the product of the two path oscillations on mesh $2^{-n}$, which tends to zero by [uniform continuity](../../../../../../uniform-continuity.md) on $[0,T+1]$.

The bracket under the new [probability measure](../../../../../../probability-measure.md) must be understood as the [quadratic covariation](../../../../../../quadratic-covariation.md) of continuous [semimartingales](../../../../../../semimartingale.md). [Semimartingale stability under an absolutely continuous measure change](../../../../../../semimartingale-stability-under-an-absolutely-continuous-measure-change.md) ensures this class is preserved; the [local martingale](../../../../../../local-martingale.md) property need not be. For example, on a finite horizon, weighting [Brownian motion](../../../../../../brownian-motion-split.md) by $\exp(\mu B_T-\mu^2T/2)$ makes $B_t-\mu t$ a [Brownian motion](../../../../../../brownian-motion-split.md) by the [Girsanov theorem](../../../../../../girsanov-theorem.md), so $B$ has nonzero drift under the new measure even though its [quadratic variation](../../../../../../quadratic-variation.md) is still $t$. The PDF additionally assumes that $M,N$ remain [local martingales](../../../../../../local-martingale.md) under the new [probability measure](../../../../../../probability-measure.md), so its bracket is also defined directly by the [local martingale](../../../../../../local-martingale.md) characterization.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
