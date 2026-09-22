<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Construct the strictly positive [rolling one-period bond account](../../../../../../rolling-one-period-bond-account.md) using successive one-period [zero-coupon bonds](../../../../../../zero-coupon-bond.md):

$$
\beta_0=1,\qquad\beta_t=\frac{\beta_{t-1}}{P_{t-1}(t)}.
$$

At time $t-1$, invest the entire account value in the bond maturing at $t$. This gives a positive [self-financing portfolio](../../../../../../self-financing-portfolio.md) usable as a [numéraire](../../../../../../numeraire.md).

We use the finite-discrete-time [fundamental theorem of asset pricing](../../../../../../fundamental-theorem-of-asset-pricing.md): in a frictionless market with finitely many adapted assets and trading dates, no arbitrage is equivalent to existence of an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) for asset prices, including dividends, expressed in a positive traded [numéraire](../../../../../../numeraire.md). Maturing bond payoffs are reinvested in that numéraire. Let $\mathbb Q$ be such a measure and $L_t=\mathbb E[d\mathbb Q/d\mathbb P\mid\mathcal F_t]$ its positive density process. The [martingale](../../../../../../martingale-split.md) pricing relation for a unit [zero-coupon bond](../../../../../../zero-coupon-bond.md) is

$$
\frac{P_t(T)}{\beta_t}=\mathbb E_{\mathbb Q}\left[\frac1{\beta_T}\mid\mathcal F_t\right].
$$

Define $Z_t=L_t/\beta_t$. The [Bayes formula for conditional expectation](../../../../../../bayes-formula-for-conditional-expectation.md) then gives

$$
\boxed{P_t(T)=\frac{\mathbb E(Z_T\mid\mathcal F_t)}{Z_t}.}
$$

The positive expectations are finite because these are the traded finite bond prices; in particular $\mathbb EZ_T=Z_0P_0(T)$ when initial information is trivial. Normalize $Z_0=1$ without changing any ratio. With nontrivial initial information the same identities are conditional on that information. The [state-price density](../../../../../../state-price-density.md) need not be unique when the bond market is incomplete; existence is sufficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
