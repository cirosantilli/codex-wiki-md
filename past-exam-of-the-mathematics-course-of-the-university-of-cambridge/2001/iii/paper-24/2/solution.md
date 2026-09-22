<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [simple predictable process](../../../../../simple-predictable-process.md), define its [stochastic integral](../../../../../stochastic-integral.md) by

$$
(H\mathbin\cdot M)_t=\sum_{k=0}^{n-1}Z_{t_k}\bigl(M_{t\wedge t_{k+1}}-M_{t\wedge t_k}\bigr).
$$

Common refinement of the deterministic partitions makes this definition independent of the representation. Each summand is a [martingale](../../../../../martingale-split.md) increment multiplied by information already available at its left endpoint, so the resulting process is a continuous square-integrable [martingale](../../../../../martingale-split.md) starting at zero. Its terminal value is the same sum with $t$ replaced by $t_n$.

Write $\Delta_kM=M_{t_{k+1}}-M_{t_k}$. If $j<k$, then $Z_{t_j}\Delta_jM\,Z_{t_k}$ is $\mathcal F_{t_k}$-measurable. By the [conditional expectation](../../../../../conditional-expectation.md) identity for increments of a [martingale](../../../../../martingale-split.md),

$$
\mathbb E[Z_{t_j}\Delta_jM\,Z_{t_k}\Delta_kM]=0.
$$

The [conditional bracket isometry for stopped martingale increments](../../../../../conditional-bracket-isometry-for-stopped-martingale-increments.md) gives

$$
\mathbb E[(\Delta_kM)^2\mid\mathcal F_{t_k}]
=\mathbb E([M]_{t_{k+1}}-[M]_{t_k}\mid\mathcal F_{t_k}).
$$

For completeness, this identity follows by applying the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $M$ and $M^2-[M]$ and expanding the square. The latter process is a true uniformly integrable [martingale](../../../../../martingale-split.md) here: the [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) bounds $\mathbb E\sup_t|M_t|^2$, stopped square identities and [Fatou's lemma](../../../../../fatou-s-lemma.md) give $\mathbb E[M]_\infty<\infty$, and its absolute supremum is bounded by $\sup_t|M_t|^2+[M]_\infty$. Consequently all the stopped identities pass to the limit.

Multiplying the conditional identity by $Z_{t_k}^2$, taking [expectations](../../../../../expected-value.md), and using the vanished cross terms proves the [Itô isometry](../../../../../ito-isometry.md):

$$
\boxed{\mathbb E[(H\mathbin\cdot M)_\infty^2]
=\sum_k\mathbb E[Z_{t_k}^2([M]_{t_{k+1}}-[M]_{t_k})]
=\mathbb E\int_0^\infty H_s^2\,d[M]_s.}
$$

To extend the [stochastic integral](../../../../../stochastic-integral.md), use the finite [quadratic-variation measure](../../../../../quadratic-variation-measure.md) $\nu_M(C)=\mathbb E\int\mathbf1_C\,d[M]$ on the [predictable sigma-algebra](../../../../../predictable-sigma-algebra.md). The [density of simple predictable processes for finite measures](../../../../../density-of-simple-predictable-processes-for-finite-measures.md) gives approximations to every $H\in L^2(\nu_M)$. The [Itô isometry](../../../../../ito-isometry.md) makes the corresponding terminal integrals Cauchy in $L^2$, and the [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) makes the whole processes Cauchy in expected squared supremum. Their limit defines a continuous [martingale](../../../../../martingale-split.md), and the isometry persists. For a locally bounded [predictable process](../../../../../predictable-process.md), choose increasing [stopping times](../../../../../stopping-time.md) tending to infinity on which it is bounded, also restrict the time horizon, and perform this construction after stopping. The isometry shows that the stopped definitions agree on overlaps, so they patch into a uniquely defined continuous [local martingale](../../../../../local-martingale.md) $H\mathbin\cdot M$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
