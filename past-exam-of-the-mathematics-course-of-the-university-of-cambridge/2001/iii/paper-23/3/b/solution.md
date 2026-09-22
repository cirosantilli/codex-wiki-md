<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One alternative is a [stochastic volatility model](../../../../../../stochastic-volatility-model.md), such as the [Heston model](../../../../../../heston-model.md):

$$
dS_t=\mu S_tdt+\sqrt{v_t}S_tdW_t^{(1)},\qquad
dv_t=\kappa(\theta-v_t)dt+\xi\sqrt{v_t}\,dW_t^{(2)},\qquad
d\langle W^{(1)},W^{(2)}\rangle_t=\rho\,dt.
$$

The parameters satisfy $\kappa,\theta,\xi>0$ and $|\rho|\le1$, and $v_0\ge0$. The square-root [Itô diffusion](../../../../../../ito-diffusion.md) has a nonnegative solution; $2\kappa\theta\ge\xi^2$ is a standard sufficient condition for the positive initial [variance](../../../../../../variance-split.md) not to hit zero. Mean reversion of $v_t$ allows persistent high- and low-volatility episodes, and negative $\rho$ can produce the empirical association between falling prices and rising volatility. Mixtures of conditional return distributions produce richer tails and option [implied volatility](../../../../../../implied-volatility.md) shapes than constant-volatility [geometric Brownian motion](../../../../../../geometric-brownian-motion.md).

For data showing [volatility clustering](../../../../../../volatility-clustering.md) and option smiles, this is often a more useful fit. It is not universally superior: more parameters create estimation and calibration uncertainty, the model is more expensive to use, and its continuous price paths still exclude price jumps. With two independent noise directions and only a [stock](../../../../../../stock.md) and a [bank account](../../../../../../bank-account.md), the market is generally incomplete, so a volatility [risk premium](../../../../../../risk-premium.md) or an extra traded instrument is needed for unique [contingent claim](../../../../../../contingent-claim.md) pricing. **The alternative improves flexibility at the cost of calibration and hedging complexity.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
