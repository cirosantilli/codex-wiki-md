<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [elementary predictable process with stopping-time intervals](../../../../../../elementary-predictable-process-with-stopping-time-intervals.md) has the form $H=\sum_{j=0}^{r-1}h_j\mathbf1_{(\tau_j,\tau_{j+1}]}$, where the [stopping times](../../../../../../stopping-time.md) are ordered and $h_j$ is bounded and $\mathcal F_{\tau_j}$-measurable. Deterministic endpoints give the usual [simple predictable process](../../../../../../simple-predictable-process.md). Define the zero-starting [stochastic integral](../../../../../../stochastic-integral.md) by

$$
\boxed{(H\cdot M)_t=\sum_{j=0}^{r-1}h_j(M_{t\wedge\tau_{j+1}}-M_{t\wedge\tau_j}).}
$$

Common refinement and telescoping show that this definition is independent of the representation. Use $M_\infty$ for an infinite endpoint. The [L2-bounded martingale convergence theorem](../../../../../../l2-bounded-martingale-convergence-theorem.md) gives convergence of $M_t$ in $L^2$ to $M_\infty$ and $M_t=\mathbb E[M_\infty\mid\mathcal F_t]$.

Put $D_j=M_{\tau_{j+1}}-M_{\tau_j}$. The [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $\mathbb E[D_j\mid\mathcal F_{\tau_j}]=0$. For $j<k$, the variable $h_jD_jh_k$ is $\mathcal F_{\tau_k}$-measurable; hence $\mathbb E[h_jD_jh_kD_k]=0$. Applying the same theorem to the assumed [martingale](../../../../../../martingale-split.md) $M^2-[M]$ gives

$$
\mathbb E[D_j^2\mid\mathcal F_{\tau_j}]=\mathbb E[[M]_{\tau_{j+1}}-[M]_{\tau_j}\mid\mathcal F_{\tau_j}].
$$

Consequently the [Itô isometry](../../../../../../ito-isometry.md) follows:

$$
\boxed{\mathbb E[(H\cdot M)_\infty^2]=\sum_j\mathbb E[h_j^2([M]_{\tau_{j+1}}-[M]_{\tau_j})]=\mathbb E\int_0^\infty H_s^2\,d[M]_s.}
$$

The unbounded [stopping times](../../../../../../stopping-time.md) cause no optional-sampling gap. The $L^2$ terminal representation makes $M$ [uniformly integrable](../../../../../../uniform-integrability.md) and makes the family of stopped $M^2$ [uniformly integrable](../../../../../../uniform-integrability.md), by conditional Jensen applied to $M_\infty^2$. Also $\mathbb E[M]_\infty=\mathbb E M_\infty^2-\mathbb E M_0^2<\infty$, from [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) and the assumed square-compensator identity. Thus $M^2-[M]$ has the needed uniform integrability, and truncating [stopping times](../../../../../../stopping-time.md) and passing in $L^1$ is legitimate. Bounded coefficients are part of the simple-integrand convention; more general coefficients require the displayed square-integrability condition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
