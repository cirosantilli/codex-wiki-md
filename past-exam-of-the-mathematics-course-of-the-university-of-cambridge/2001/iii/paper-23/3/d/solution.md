<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume a frictionless market with no taxes or transaction costs, unrestricted [short selling](../../../../../../short-finance.md) and borrowing/lending at the same constant rate $r$, continuous trading, and absence of [arbitrage](../../../../../../arbitrage.md). The non-dividend-paying [stock](../../../../../../stock.md) has [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) dynamics $dS=\mu Sdt+\sigma SdW$ with constant $\sigma>0$, and the [bank account](../../../../../../bank-account.md) satisfies $dB=rBdt$. A [contingent claim](../../../../../../contingent-claim.md) with no interim cash flows has sufficiently regular value $f(t,S)$, meaning $f\in C^{1,2}$ before maturity; terminal [financial payoff](../../../../../../contingent-claim-payoff.md) kinks can be handled by the smooth value for earlier times. Trading strategies are [adapted](../../../../../../adapted-process.md), [self-financing portfolios](../../../../../../self-financing-portfolio.md), and [admissible trading strategies](../../../../../../admissible-trading-strategy.md) so that doubling strategies are excluded.

The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
df=\left(f_t+\mu Sf_S+\frac12\sigma^2S^2f_{SS}\right)dt+\sigma Sf_SdW.
$$

Choose $\Delta=f_S$ shares and put the remaining value $f-Sf_S$ in the [bank account](../../../../../../bank-account.md). Its self-financing gain is

$$
\Delta\,dS+r(f-S\Delta)dt
=\{\mu Sf_S+r(f-Sf_S)\}dt+\sigma Sf_SdW.
$$

Matching the [contingent claim](../../../../../../contingent-claim.md)'s gain to this replicating gain cancels the random increment and equates the drifts:

$$
\boxed{f_t+\frac12\sigma^2S^2f_{SS}+rSf_S-rf=0.}
$$

This is the [Black-Scholes equation](../../../../../../black-scholes-equation.md). The argument uses the self-financing gain $\Delta\,dS$, not a product differential that incorrectly treats a changing $\Delta$ as free cash. Rebalancing purchases are financed from the [bank account](../../../../../../bank-account.md). Conversely, a smooth solution with suitable growth and [boundary conditions](../../../../../../boundary-condition.md) defines a [delta hedge](../../../../../../delta-hedge.md) whose value replicates the [contingent claim](../../../../../../contingent-claim.md); [law of one price](../../../../../../law-of-one-price.md) identifies this value with the [contingent claim](../../../../../../contingent-claim.md) price. Here $S$ is the current [stock](../../../../../../stock.md) price, $t$ is time, $\sigma$ is proportional volatility, $r$ is the risk-free rate, and $f$ is the [contingent claim](../../../../../../contingent-claim.md) price. The physical [expected return](../../../../../../expected-return.md) $\mu$ cancels because exposure to price risk has been hedged.

## ↑ Ancestors (11)

1. [D](../d.md)
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
