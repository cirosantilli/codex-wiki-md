<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use zero-interest cash as the one-period [numéraire](../../../../../../numeraire.md), consistent with the stated expectation-price formula. For $p>1$, differentiate the proposed call-price curve twice. The first derivative and the candidate density are

$$
\begin{aligned}
C'(u)&=u^{p-1}(1+u^p)^{1/p-1}-1,\\
\boxed{f_p(u)=C''(u)}&=\boxed{(p-1)u^{p-2}(1+u^p)^{1/p-2},\qquad u>0.}
\end{aligned}
$$

This is the [power call-curve pricing density](../../../../../../power-call-curve-pricing-density.md). It is strictly positive. Its integral is $C'(\infty)-C'(0+)=1$, and its survival function is $-C'(u)$. Since $C(0+)=1$ and $C(\infty)=0$,

$$
\int_0^\infty u f_p(u)\,du
=\int_0^\infty[-C'(u)]\,du=1.
$$

Likewise, integrating the survival function from $K$ onwards gives

$$
\int_0^\infty(u-K)^+f_p(u)\,du=C(K).
$$

Thus a market whose terminal [stock](../../../../../../stock.md) has this law under an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) prices the [stock](../../../../../../stock.md) at one, every proposed call at $C(K)$, and any [integrable](../../../../../../integrability.md) claim $g(S_1)$ at $\int g(u)f_p(u)du$. The finite-market [fundamental theorem of asset pricing](../../../../../../fundamental-theorem-of-asset-pricing.md) says that an equivalent measure pricing every traded discounted payoff by [expectation](../../../../../../expected-value.md) excludes [arbitrage](../../../../../../arbitrage.md). This proves the intended conclusion when such an equivalent pricing law is part of the model. For example, take the canonical terminal state space $(0,\infty)$ with [stock](../../../../../../stock.md) equal to its coordinate and physical law equivalent to the positive density $f_p$.

There is, however, a genuine insufficiency in the literal finite-strike formulation: a finite list of call prices and no-arbitrage alone do not force this pricing law, nor even a continuous terminal distribution. Here is an explicit counterexample. Take $p=2$, one strike $K=1$, and two terminal [stock](../../../../../../stock.md) values

$$
a=\frac12,\qquad b=2+\sqrt2,
\qquad\mathbb Q(S_1=b)=3-2\sqrt2.
$$

Give the lower [stock](../../../../../../stock.md) value the remaining strictly positive probability and take this as the physical measure too. Direct calculation gives $\mathbb E S_1=1$ and

$$
\mathbb E(S_1-1)^+=\sqrt2-1=C(1),
$$

so the [stock](../../../../../../stock.md)/cash/call market is arbitrage-free. Now let

$$
g(u)=(u-a)^2(u-b)^2e^{-u}.
$$

This bounded nonnegative function is zero at both actual [stock](../../../../../../stock.md) values, so $g(S_1)=0$ almost surely. Yet $\int g(u)f_2(u)du>0$. Charging that positive amount for the identically zero payoff creates an [arbitrage](../../../../../../arbitrage.md) by selling it. In fact no Lebesgue probability density can price every claim correctly on this two-state market.

Therefore **the displayed $f_p$ is the intended continuous pricing density, but the promised no-arbitrage extension requires an equivalent pricing measure with this terminal law; a full call curve identifies that law if such a measure exists, but it does not follow from the printed finite-strike hypotheses alone**. This is the [finite-strike nonidentification of a pricing density](../../../../../../finite-strike-nonidentification-of-a-pricing-density.md). The counterexample and the corrected sufficient hypothesis account for the literal and intended readings separately.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
