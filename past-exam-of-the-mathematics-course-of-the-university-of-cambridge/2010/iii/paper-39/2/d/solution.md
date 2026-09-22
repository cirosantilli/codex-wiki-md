<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix the horizon $T$ and define the [half-volatility measure for a square-root stock claim](../../../../../../half-volatility-measure-for-a-square-root-stock-claim.md) by

$$
Z_s=\exp\left(\frac12\int_0^s\sigma_u\,dW_u-\frac18\int_0^s\sigma_u^2du\right),\qquad
\frac{dQ}{dP}\bigg|_{\mathcal F_T}=Z_T.
$$

The [Novikov condition](../../../../../../novikov-s-condition.md) makes $Z$ a true [martingale](../../../../../../martingale-split.md) with $\mathbb EZ_T=1$, and $Z_T>0$ makes $Q$ equivalent to $P$. The [Girsanov theorem](../../../../../../girsanov-theorem.md) identifies $W_s^Q=W_s-\frac12\int_0^s\sigma_u du$ as a [Brownian motion](../../../../../../brownian-motion-split.md) under $Q$.

The exact factorization from the previous part is

$$
\sqrt{S_T}=\sqrt{S_t}\,\frac{Z_T}{Z_t}e^{-I_{t,T}/8}.
$$

Using the [Bayes formula for conditional expectation](../../../../../../bayes-formula-for-conditional-expectation.md) therefore gives

$$
\boxed{C(t,T)=\sqrt{S_t}\,\mathbb E_Q[e^{-I_{t,T}/8}\mid\mathcal F_t].}
$$

The random integrated variance need not have any independence property under $Q$. Its pathwise bounds still imply $e^{-b^2\tau/8}\leq\mathbb E_Q[e^{-I_{t,T}/8}\mid\mathcal F_t]\leq e^{-a^2\tau/8}$. Inverting the same price function proves **$a\leq\Sigma(t,T)\leq b$ even for volatility adapted to the Brownian motion**, on the positive-price event. The zero-price convention is as above. The auxiliary measure here is not asserted to be an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) for the stock.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
