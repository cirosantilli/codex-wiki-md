<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The usual replication argument needs two hypotheses implicit in the pricing conclusion: the strategy must replicate the payoff, $V_N=X$, and its discounted gains must be integrable. Bounded [predictable](../../../../../../predictable-process.md) risky holdings suffice for the latter. Under these conditions, the [equivalent martingale measure](../../../../../../risk-neutral-measure.md) $\mathbb Q$ and part (c) give

$$
\mathbb E_{\mathbb Q}[\widetilde V_n-\widetilde V_{n-1}\mid\mathcal F_{n-1}]
=\phi_n\mathbb E_{\mathbb Q}[\widetilde S_n-\widetilde S_{n-1}\mid\mathcal F_{n-1}]=0.
$$

Thus discounted wealth is a [martingale](../../../../../../martingale-split.md), and repeated conditioning gives

$$
\boxed{V_n=B_n\mathbb E_{\mathbb Q}[X/B_N\mid\mathcal F_n].}
$$

For a normalized initial [bank account](../../../../../../bank-account.md), $B_0=1$, deterministic terminal bank value, and trivial initial information, this reduces to the intended [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) formula

$$
\boxed{V_0=B_N^{-1}\mathbb E_{\mathbb Q}[X].}
$$

If $B_N$ is random it must remain inside the expectation. If a claim is not replicable, the existence of an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) alone does not make its arbitrage-free price unique.

The [discounted wealth martingale integrability condition](../../../../../../discounted-wealth-martingale-integrability-condition.md) cannot simply be dropped. For a concrete counterexample, set $B_n=1$, $S_0=3/2$, $S_1=1+U$, and $S_2=1+U+\varepsilon/2$, where $U$ is uniform on $(0,1)$ and $\varepsilon$ an independent fair sign. These positive bounded prices form a [martingale](../../../../../../martingale-split.md) in the natural filtration. Start with zero holdings; at time one buy $1/U$ shares financed by borrowing $S_1/U$. This is [previsible](../../../../../../predictable-process.md) and [self-financing](../../../../../../self-financing-portfolio.md), but its terminal wealth is $\varepsilon/(2U)$, whose absolute expectation is infinite. It is therefore not a [martingale](../../../../../../martingale-split.md). The stated pricing proof applies to the standard integrable replication class, rather than all unconstrained previsible strategies.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
