<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the discounted wealth $\widetilde X=X/B$ and the [discounted dividend gains](../../../../../../discounted-dividend-gains.md)

$$
Y_t=\frac{S_t}{B_t}+\int_0^t\frac{D_s}{B_s}\,ds.
$$

The integral uses $ds$: the printed $dt$ inside an integral indexed by $s$ is a differential typo. Since $B$ is a positive [finite-variation process](../../../../../../finite-variation-process.md), the [Itô product rule](../../../../../../ito-product-rule.md) gives

$$
d\widetilde X_t
=\frac{dX_t}{B_t}-\frac{X_t}{B_t^2}\,dB_t
=\pi_t\cdot\left(\frac{dS_t}{B_t}-\frac{S_t}{B_t^2}\,dB_t+\frac{D_t}{B_t}\,dt\right)
=\pi_t\cdot dY_t.
$$

The bank-account terms cancel using $X_t=\phi_tB_t+\pi_t\cdot S_t$.

If $Y$ is a $Q$-[martingale](../../../../../../martingale-split.md), discounted self-financing wealth is a $Q$-[local martingale](../../../../../../local-martingale.md). The [admissible trading strategy](../../../../../../admissible-trading-strategy.md) lower bound makes it a [supermartingale](../../../../../../supermartingale.md), exactly as in the previous no-arbitrage proof. A zero-cost portfolio with nonnegative terminal wealth must therefore have terminal wealth zero $Q$-almost surely and, by equivalence, physically almost surely. Hence **an equivalent martingale measure for discounted dividend gains excludes arbitrage**. It is the gains process, not just the ex-dividend price ratio, that must have zero martingale drift.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
