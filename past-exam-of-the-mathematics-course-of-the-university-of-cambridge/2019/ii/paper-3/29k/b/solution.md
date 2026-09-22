<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0\leq t<T$, set $\tau=T-t$ and

$$
d_-(t,S_t)
=\frac{\log(S_t/K)+(r-\sigma^2/2)\tau}
{\sigma\sqrt\tau}.
$$

Under the [equivalent martingale measure](../../../../../../risk-neutral-measure.md), conditional log-normality gives

$$
\mathbb Q(S_T\geq K\mid\mathcal F_t)
=\Phi(d_-(t,S_t)).
$$

The [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) value of the [digital call option](../../../../../../digital-call-option.md) is consequently

$$
\boxed{
D_{\rm call}(t,S_t)
=e^{-r(T-t)}\Phi(d_-(t,S_t)).}
$$

At $t=T$ this converges to the stated payoff away from $S_T=K$, with the payoff convention specifying the boundary value.

The [delta hedge](../../../../../../delta-hedge.md) holds the derivative of the claim value with respect to the current stock price. Since

$$
\frac{\partial d_-}{\partial S}=\frac1{S\sigma\sqrt\tau},
$$

the number of risky-asset units for $t<T$ is

$$
\boxed{
\Delta_t
=\frac{e^{-r(T-t)}\phi(d_-(t,S_t))}
{S_t\sigma\sqrt{T-t}}.}
$$

This is the [Black-Scholes digital option formula](../../../../../../black-scholes-digital-option-formula.md). The hedge becomes singular close to maturity near the strike, reflecting the discontinuity of the payoff.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
