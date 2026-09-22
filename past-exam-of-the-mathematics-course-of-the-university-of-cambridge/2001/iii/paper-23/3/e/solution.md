<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For strike $K>0$ and maturity $T$, a [European call option](../../../../../../european-call-option.md) and a [European put option](../../../../../../european-put-option.md) have [boundary conditions](../../../../../../boundary-condition.md)

$$
C(T,S)=(S-K)^+,\qquad P(T,S)=(K-S)^+.
$$

The [Black-Scholes equation](../../../../../../black-scholes-equation.md) is solved backward from these conditions. At zero [stock](../../../../../../stock.md) price, the zero state is absorbing in [geometric Brownian motion](../../../../../../geometric-brownian-motion.md), so

$$
C(t,0)=0,\qquad P(t,0)=Ke^{-r(T-t)}.
$$

At the other boundary, with $\tau=T-t>0$,

$$
C(t,S)-[S-Ke^{-r\tau}]\longrightarrow0,\qquad P(t,S)\longrightarrow0
\quad(S\to\infty).
$$

These conditions and a suitable growth bound select the financial solution and provide boundary data for numerical truncations. In the constant-coefficient model, under the [risk-neutral measure](../../../../../../risk-neutral-measure.md),

$$
S_T=S\exp\{(r-\sigma^2/2)\tau+\sigma\sqrt{\tau}\,Z\},\qquad Z\sim N(0,1).
$$

For $d_1=[\log(S/K)+(r+\sigma^2/2)\tau]/(\sigma\sqrt{\tau})$ and $d_2=d_1-\sigma\sqrt{\tau}$, the exercise event is $Z>-d_2$. Completing the square in $e^{\sigma\sqrt{\tau}Z}$ times the normal density gives the truncated first moment and hence

$$
\boxed{C=S\Phi(d_1)-Ke^{-r\tau}\Phi(d_2),\qquad
P=Ke^{-r\tau}\Phi(-d_2)-S\Phi(-d_1),}
$$

where $\Phi$ is the standard normal [cumulative distribution function](../../../../../../cumulative-distribution-function.md). These are the [Black-Scholes formula](../../../../../../black-scholes-formula.md) values and satisfy the specified terminal and [boundary conditions](../../../../../../boundary-condition.md).

[Put-call parity](../../../../../../put-call-parity.md) is the relation

$$
\boxed{C-P=S-Ke^{-r(T-t)}.}
$$

A call minus a put has terminal [financial payoff](../../../../../../contingent-claim-payoff.md) $S_T-K$. A [portfolio](../../../../../../investment-portfolio.md) of one share minus a [zero-coupon bond](../../../../../../zero-coupon-bond.md) paying $K$ has the same [financial payoff](../../../../../../contingent-claim-payoff.md), so absence of [arbitrage](../../../../../../arbitrage.md) and [law of one price](../../../../../../law-of-one-price.md) equate their current values. The formula here assumes the same strike and maturity and no dividends; known dividends modify the stock-side value.

## ↑ Ancestors (11)

1. [E](../e.md)
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
