<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the natural filtration $\mathcal F_t=\sigma(Z_1,\ldots,Z_t)$ and the usual integrable definition of the [Snell envelope](../../../../../snell-envelope.md). Since the factors are positive, its terminal value is $U_T=Y_T$. If $U_{t+1}=Y_{t+1}c_{t+1}$, [independence of random variables](../../../../../independent-random-variables.md) gives

$$
\mathbb E[U_{t+1}\mid\mathcal F_t]=Y_tc_{t+1}\mathbb E Z_{t+1}.
$$

The backward recursion therefore becomes

$$
\boxed{U_t=Y_tc_t,\qquad c_T=1,\qquad c_t=\max\{1,c_{t+1}\mathbb E Z_{t+1}\}.}
$$

This proves the assertion by backward induction. All constants are finite and at least one. More explicitly,

$$
c_t=\max_{t\le u\le T}\prod_{j=t+1}^u\mathbb E Z_j,
$$

where the empty product is one. This is the [Snell envelope of a multiplicative process](../../../../../snell-envelope-of-a-multiplicative-process.md). The standard [Snell envelope](../../../../../snell-envelope.md) hypothesis includes integrable rewards; [independence of random variables](../../../../../independent-random-variables.md) and positivity then give finite first moments of the factors. If that hypothesis is dropped, an infinite-mean factor gives an infinite continuation value, so finite constants need not exist.

For the [discrete-time binomial market](../../../../../discrete-time-binomial-market.md), write $p=(1+r/\varepsilon)/2$. The assumptions give $0<p<1$, positive [bank account](../../../../../bank-account.md) and [stock](../../../../../stock.md) prices, and

$$
\mathbb E R_{t+1}=p\varepsilon-(1-p)\varepsilon=r.
$$

Thus

$$
\mathbb E\left[\frac{S_{t+1}}{B_{t+1}}\mid\mathcal F_t\right]=\frac{S_t}{B_t}.
$$

The finite discrete-time [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md) states that a market with a strictly positive [numéraire](../../../../../numeraire.md) has no [arbitrage](../../../../../arbitrage.md) if there is an equivalent probability measure under which all numéraire-denominated asset prices are [martingales](../../../../../martingale-split.md). The original probability measure is already such an [equivalent martingale measure](../../../../../risk-neutral-measure.md), proving **no [arbitrage](../../../../../arbitrage.md)**.

The complete-market American-option pricing theorem identifies the discounted replication or superhedging value with the [Snell envelope](../../../../../snell-envelope.md) of the discounted exercise rewards. Here

$$
Y_t=\frac{S_t^2}{(1+r)^t}=S_0^2\prod_{j=1}^t\frac{(1+R_j)^2}{1+r}.
$$

The independent factors have common mean

$$
\lambda=\frac{\mathbb E(1+R_j)^2}{1+r}=\frac{1+2r+\varepsilon^2}{1+r}=1+\frac{r+\varepsilon^2}{1+r}>1.
$$

The [Snell envelope](../../../../../snell-envelope.md) recursion consequently gives $c_t=\lambda^{T-t}$. At every time before $T$, the continuation value strictly exceeds immediate exercise, so **optimal exercise is at maturity**. The undiscounted value process is $V_t=S_t^2\lambda^{T-t}$, and the time-zero replication cost is

$$
\boxed{V_0=S_0^2\left(\frac{1+2r+\varepsilon^2}{1+r}\right)^T.}
$$

In fact $V_t/B_t$ is a [martingale](../../../../../martingale-split.md), not just a [supermartingale](../../../../../supermartingale.md), because the [Snell envelope](../../../../../snell-envelope.md) has no exercise compensator before maturity.

To hedge the optimally exercised payoff, subtract the two next-state [portfolio](../../../../../investment-portfolio.md) equations. The first-period [delta hedge](../../../../../delta-hedge.md) is

$$
\Delta_0=\frac{S_0^2(1+\varepsilon)^2\lambda^{T-1}-S_0^2(1-\varepsilon)^2\lambda^{T-1}}{S_0(1+\varepsilon)-S_0(1-\varepsilon)}
=\boxed{2S_0\lambda^{T-1}}.
$$

The corresponding [bank account](../../../../../bank-account.md) holding, since $B_0=1$, is $V_0-\Delta_0S_0=S_0^2\lambda^{T-1}(\lambda-2)$. Substitution into either next-state equation verifies both terminal values at time one. Repeating this two-state calculation at every node gives a [self-financing strategy](../../../../../self-financing-portfolio.md) replicating the maturity payoff. It also covers earlier exercise: $V_t\ge S_t^2$ at all dates, so the seller can meet any earlier payment with the available wealth.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
