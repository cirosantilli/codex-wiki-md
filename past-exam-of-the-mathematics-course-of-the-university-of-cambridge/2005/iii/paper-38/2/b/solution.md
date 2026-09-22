<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [stopping time](../../../../../../stopping-time.md) $T\le s$, [optional sampling](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) for $N$ gives $\mathbb E[N_s\mid\mathcal F_T]=N_T$, hence

$$
\mathbb E[M_TN_s]=\mathbb E[M_TN_T].
$$

This is justified by truncation and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), as in [solution](../a/iv/solution.md). If $MN$ is a [martingale](../../../../../../martingale-split.md), bounded optional sampling gives $\mathbb E[M_TN_T]=\mathbb E[M_0N_0]=0$, proving the required condition.

Conversely suppose the required condition holds. Every bounded [stopping time](../../../../../../stopping-time.md) $T$ lies below some deterministic $s$, so the displayed identity gives $\mathbb E[(MN)_T]=0$. The product is continuous and adapted, and its stopped values are integrable: the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) bounds the product of the two path suprema in $L^1$ by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The [characterization of a martingale by bounded continuous-time stopped expectations](../../../../../../characterization-of-a-martingale-by-bounded-continuous-time-stopped-expectations.md) therefore makes $MN$ a [martingale](../../../../../../martingale-split.md). Thus **orthogonality is equivalent to the backward-stopping [expectation](../../../../../../expected-value.md) test**. In contrast to [weakly orthogonal continuous martingales](../../../../../../weakly-orthogonal-continuous-martingales.md), this tests the product at random times, not only deterministic times.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
