# European call option

↑ **Parent:** [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/European_call_option)

A [European call option](european-call-option.md) gives its holder the right, without an obligation, to buy one unit of an underlying [financial asset](financial-asset.md) at the [strike price](strike-price.md) $K$ on the expiry date $T$. European describes exercise timing, not geography: exercise is allowed only at $T$. Here the underlying is one [stock](stock.md) share, $S_T$ is its price at expiry, and the [financial payoff](contingent-claim-payoff.md) is expressed as a cash amount. Physical exercise delivers a share against payment of $K$; immediate resale gives the same net amount under the assumed [frictionless market](frictionless-market.md).

The holder exercises only when buying at the [strike price](strike-price.md) is advantageous. Writing $x^+=\max(x,0)$ for the [positive part](positive-part-of-a-real-valued-function.md), the terminal [financial payoff](contingent-claim-payoff.md) is

$$
C_T=(S_T-K)^+=\begin{cases}0,&S_T\leq K,\\S_T-K,&S_T>K.\end{cases}
$$

The [European call option](european-call-option.md) is a reusable building block for [claim replication](claim-replication.md): its [financial payoff](contingent-claim-payoff.md) is zero below the [strike price](strike-price.md) and rises by one unit for each unit of [stock](stock.md) price above it. The corner at $K$ lets combinations of [European call options](european-call-option.md) construct other payoff shapes, as in [static replication on a finite terminal support](static-replication-on-a-finite-terminal-support.md).

For [strike price](strike-price.md) $K=100$, the following are deterministic calculations conditional on each displayed terminal [stock](stock.md) price. They assign no [probabilities](probability.md) to the three scenarios. The [European put option](european-put-option.md) has the opposite exercise right and the [financial payoff](contingent-claim-payoff.md) $(K-S_T)^+$.

| Terminal [stock](stock.md) price $S_T$ | [European call option](european-call-option.md) $C_T$ | [European put option](european-put-option.md) $P_T$ | Difference $C_T-P_T$ |
| --- | --- | --- | --- |
| $80$ | $0$ | $20$ | $-20$ |
| $100$ | $0$ | $0$ | $0$ |
| $120$ | $20$ | $0$ | $20$ |

<a id="image-european-call-and-put-terminal-payoffs-at-strike-100-with-their-linear-difference"></a>
![](european-option-payoffs.png)

**[Figure 1](#image-european-call-and-put-terminal-payoffs-at-strike-100-with-their-linear-difference). European call and put terminal payoffs at strike 100, with their linear difference**.

A [financial payoff](contingent-claim-payoff.md) excludes the initial contract price. If the illustrative [European call option](european-call-option.md) costs $C_0=10$, its [financial payoff](contingent-claim-payoff.md) at $S_T=120$ is $20$, and subtracting its initial cost gives $10$. If that cost is instead borrowed for one year at the constant continuously compounded [interest rate](interest-rate.md) $r=0.05$, the terminal net amount is $20-10e^{0.05}\approx9.48728904$. At $S_T=80$ or $100$, the corresponding net amount is $-10e^{0.05}\approx-10.51271096$. Keeping all cash amounts at the same date avoids confusing a [financial payoff](contingent-claim-payoff.md) with a financed gain.

Robert Shiller's [Options Markets lecture, Yale ECON 252 (2011)](https://oyc.yale.edu/economics/econ-252-11/lecture-17) introduces these exercise rights and payoff shapes.

**Table of contents**

- [Down-and-out European call](down-and-out-european-call.md)
  - [Zero-rate barrier-strike call hedge](zero-rate-barrier-strike-call-hedge.md)
- [Convexity of a European call price in strike](convexity-of-a-european-call-price-in-strike.md)
- [Maturity monotonicity of calls with nonnegative strikes](maturity-monotonicity-of-calls-with-nonnegative-strikes.md)
- [Power payoff static call representation](power-payoff-static-call-representation.md)
  - [Sharp power-call inequality](sharp-power-call-inequality.md)
  - [Call-price decay and moment threshold](call-price-decay-and-moment-threshold.md)
- [Call-price density recovery](call-price-density-recovery.md)
  - [Finite-strike nonidentification of a pricing density](finite-strike-nonidentification-of-a-pricing-density.md)
  - [Power call-curve pricing density](power-call-curve-pricing-density.md)
- [Butterfly-spread arbitrage for nonconvex call prices](butterfly-spread-arbitrage-for-nonconvex-call-prices.md)
- [Vertical-spread arbitrage for increasing call prices](vertical-spread-arbitrage-for-increasing-call-prices.md)
- [One-period call price bounds](one-period-call-price-bounds.md)
- [Contour inversion for call prices](contour-inversion-for-call-prices.md)
- [Discrete Dupire equation](discrete-dupire-equation.md)
- [Discrete call-price curvature](discrete-call-price-curvature.md)
- [Monotonicity of a European call price in strike](monotonicity-of-a-european-call-price-in-strike.md)
- [Static replication on a finite terminal support](static-replication-on-a-finite-terminal-support.md)
  - [Discrete realized-variance replication identity](discrete-realized-variance-replication-identity.md)
- [Put-call parity](put-call-parity.md)
  - [Power put-call parity](power-put-call-parity.md)
  - [Put-call symmetry in the Black-Scholes model](put-call-symmetry-in-the-black-scholes-model.md)
- [Binomial call-price recursion](binomial-call-price-recursion.md)
- [Forward-start call option](forward-start-call-option.md)

## ↑ Ancestors (6)

1. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (46)

- [American call option](american-call-option.md)
- [Arbitrage](arbitrage.md)
- [Asian option](asian-option.md)
- [Chooser option](chooser-option.md)
- [Contingent claim payoff](contingent-claim-payoff.md)
- [Convexity of a European call price in strike](convexity-of-a-european-call-price-in-strike.md)
- [Delta jump at activation of a down-and-in call](delta-jump-at-activation-of-a-down-and-in-call.md)
- [Discrete call-price curvature](discrete-call-price-curvature.md)
- [Discrete Dupire equation](discrete-dupire-equation.md)
- [Down-and-out European call](down-and-out-european-call.md)
- [European call option](european-call-option.md)
- [European put option](european-put-option.md)
- [Guaranteed terminal stock floor in the Black-Scholes model](guaranteed-terminal-stock-floor-in-the-black-scholes-model.md)
- [Local volatility](local-volatility.md)
- [Mathematical finance](mathematical-finance-split.md)
- [Option vega](option-vega.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/28j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/28j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/29j/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-40/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/27j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/27j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-211/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/29k/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/29k/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/29k/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/29k/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3/29k/a/solution.md)
- [Put-call parity](put-call-parity.md)
- [Replicating portfolio in a binomial market](replicating-portfolio-in-a-binomial-market.md)
- [Risk-neutral pricing](risk-neutral-pricing.md)
- [Strike price](strike-price.md)
