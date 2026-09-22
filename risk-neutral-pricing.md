# Risk-neutral pricing

↑ **Parent:** [Risk-neutral measure](risk-neutral-measure.md)

In a finite-state discrete-time [financial market](financial-market.md), a replicable terminal [financial payoff](contingent-claim-payoff.md) $X$ has the displayed value under any [equivalent martingale measure](risk-neutral-measure.md) $Q$ for the [bank account](bank-account.md) [numéraire](numeraire.md). Here $\mathcal F_t$ represents current information and [conditional expectation](conditional-expectation.md) averages over future states. The [self-financing portfolio](self-financing-portfolio.md)'s discounted [portfolio wealth](portfolio-wealth.md) is a [martingale](martingale-split.md), so its current value equals the discounted [expectation](expected-value-split.md) of its terminal value. In an [incomplete market](incomplete-market.md), nonreplicable claims need not have a unique price; continuous-time extensions require further conditions on [admissible trading strategies](admissible-trading-strategy.md) and [integrable](integrability.md) discounted wealth.

For the [European call option](european-call-option.md) in the example,

$$
C_0=\frac{(5/8)20+(3/8)0}{21/20}=\frac{250}{21}\approx11.90476.
$$

Discounting the physical [expected value](expected-value-split.md) instead gives $200/21\approx9.52381$ when $p=1/2$, or $320/21\approx15.23810$ when $p=4/5$. Those amounts describe discounted physical [expectations](expected-value-split.md), not the [replicating portfolio](replicating-strategy.md)'s cost. Holding $S_0,u,d,R$ fixed is crucial: changing beliefs can influence traded prices in a richer [financial market](financial-market.md) model.

<a id="image-physical-expectations-vary-with-beliefs-while-the-one-step-replication-price-stays-fixed"></a>
![](pricing-probability-vs-belief.png)

**[Figure 1](#image-physical-expectations-vary-with-beliefs-while-the-one-step-replication-price-stays-fixed). Physical expectations vary with beliefs while the one-step replication price stays fixed**.

## ↑ Ancestors (6)

1. [Risk-neutral measure](risk-neutral-measure.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Black-Scholes equation with claim dividends](black-scholes-equation-with-claim-dividends.md)
- [Convex-payoff delta monotonicity in a binomial market](convex-payoff-delta-monotonicity-in-a-binomial-market.md)
- [Convexity preservation in Black-Scholes pricing](convexity-preservation-in-black-scholes-pricing.md)
- [Exponential claim in a driftless square-root model](exponential-claim-in-a-driftless-square-root-model.md)
- [Gaussian short-rate model with a deterministic shift](gaussian-short-rate-model-with-a-deterministic-shift.md)
- [Logarithmic stock payoff](logarithmic-stock-payoff.md)
- [Mathematical finance](mathematical-finance-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/29j/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/29k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/29k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/29k/iii/solution.md)
- [Power put-call parity](power-put-call-parity.md)
- [Reflected European payoff for an up-and-in option](reflected-european-payoff-for-an-up-and-in-option.md)
- [Risk-neutral measure](risk-neutral-measure.md)
- [Up-and-out power claim](up-and-out-power-claim.md)
