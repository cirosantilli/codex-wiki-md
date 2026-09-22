<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a [localizing sequence](../../../../../../localizing-sequence.md) of discrete-time [stopping times](../../../../../../stopping-time.md) $\tau_j\uparrow\infty$ for $X$. For fixed integer $t$, every stopped value is bounded in absolute value by the finite sum

$$
|X_{t\wedge\tau_j}|\leq\sum_{u=0}^t|X_u|.
$$

That sum is [integrable](../../../../../../integrability.md) under the hypothesis. Since $X^{\tau_j}$ is a [martingale](../../../../../../martingale-split.md),

$$
\mathbb E[X_{t\wedge\tau_j}\mid\mathcal F_{t-1}]
=X_{(t-1)\wedge\tau_j}.
$$

The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), including its conditional version, now removes the stopping. Thus $\mathbb E[X_t\mid\mathcal F_{t-1}]=X_{t-1}$. The process is [adapted](../../../../../../adapted-process.md) and [integrable](../../../../../../integrability.md) by hypothesis, so **$X$ is a true discrete-time [martingale](../../../../../../martingale-split.md)**. This is the [integrable discrete-time local martingale is a martingale](../../../../../../integrable-discrete-time-local-martingale-is-a-martingale.md) criterion. The finite sum dominating stopped values is the crucial discrete-time feature.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
