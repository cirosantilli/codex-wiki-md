<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First justify optional sampling for the square-minus-bracket process. The [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) gives $\mathbb E\sup_{t\geq0}|M_t|^2\leq4\mathbb E|M_\infty|^2<\infty$. Stop the [local martingale](../../../../../../local-martingale.md) $M^2-[M]$ using a localizing sequence and bounded bracket levels. The stopped expectation identity, followed by Fatou, bounds $\mathbb E[M]_\infty$ by the expected squared path supremum. Hence $M^2-[M]$ has an integrable absolute supremum, and localization with conditional dominated convergence makes it a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md). The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) stated in part (b) is therefore applicable to both $M$ and $M^2-[M]$.

For ordered [stopping times](../../../../../../stopping-time.md) $\sigma\leq\tau$, expand the squared increment and condition on $\mathcal F_\sigma$. The mean increment is zero, so

$$
\mathbb E[(M_\tau-M_\sigma)^2\mid\mathcal F_\sigma]=\mathbb E[M_\tau^2-M_\sigma^2\mid\mathcal F_\sigma]=\mathbb E([M]_\tau-[M]_\sigma\mid\mathcal F_\sigma).
$$

This is the [conditional bracket isometry for stopped martingale increments](../../../../../../conditional-bracket-isometry-for-stopped-martingale-increments.md). Apply it with $\sigma=T_j$, $\tau=T_{j+1}$ and multiply by the bounded $\mathcal F_{T_j}$-measurable variable $h_j^2$. The orthogonality proved in part (b) gives the [Itô isometry](../../../../../../ito-isometry.md)

$$
\boxed{\mathbb E(H\cdot M)_\infty^2=\sum_j\mathbb E\bigl[h_j^2([M]_{T_{j+1}}-[M]_{T_j})\bigr]=\mathbb E\int_0^\infty H_s^2\,d[M]_s.}
$$

To identify the whole bracket process, let $N=H\cdot M$ and $C_t=\int_0^tH_s^2\,d[M]_s$. For deterministic $s<t$ and $E\in\mathcal F_s$, apply the proved isometry to the simple integrand $\mathbf1_E\mathbf1_{(s,t]}H$. It yields

$$
\mathbb E[\mathbf1_E(N_t-N_s)^2]=\mathbb E[\mathbf1_E(C_t-C_s)].
$$

Thus $\mathbb E[(N_t-N_s)^2\mid\mathcal F_s]=\mathbb E[C_t-C_s\mid\mathcal F_s]$. Since $N$ is a [martingale](../../../../../../martingale-split.md), the cross term $2N_s(N_t-N_s)$ has conditional mean zero. Consequently $N^2-C$ is a [martingale](../../../../../../martingale-split.md). The process $C$ is continuous, adapted, nondecreasing and starts at zero, so uniqueness in the definition of [quadratic variation](../../../../../../quadratic-variation.md) proves

$$
\boxed{[H\cdot M]_t=\int_0^tH_s^2\,d[M]_s=(H^2\cdot[M])_t.}
$$

This deduction uses only the proved elementary isometry, not a previously assumed formula for the [quadratic variation](../../../../../../quadratic-variation.md) of [stochastic integrals](../../../../../../stochastic-integral.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
