# Put-call parity

↑ **Parent:** [European call option](european-call-option.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Put-call_parity)

[Put-call parity](put-call-parity.md) fixes the price difference between a [European call option](european-call-option.md) and a [European put option](european-put-option.md) on the same underlying [stock](stock.md), with the same [strike price](strike-price.md) $K$ and expiry $T$. Assume no dividends or other payments from the [stock](stock.md) before or at expiry, a known constant continuously compounded [interest rate](interest-rate.md) $r$, and a [frictionless market](frictionless-market.md). Borrowing and lending are available at that same [interest rate](interest-rate.md); [short selling](short-finance.md) of the [stock](stock.md), [European call option](european-call-option.md), [European put option](european-put-option.md), and [zero-coupon bond](zero-coupon-bond.md) is permitted. Settlement is certain, and the buy-and-hold [portfolios](investment-portfolio.md) below may be held until $T$ without interim funding restrictions or forced liquidation. These assumptions exclude transaction costs, taxes, borrowing fees, and execution or settlement risks from the [arbitrage](arbitrage.md) argument.

At expiry, the two [positive parts](positive-part-of-a-real-valued-function.md) cancel their corners:

$$
C_T-P_T=(S_T-K)^+-(K-S_T)^+=S_T-K.
$$

Thus a [European call option](european-call-option.md) and a short [European put option](european-put-option.md) together have the same terminal [financial payoff](contingent-claim-payoff.md) as one [stock](stock.md) share with a debt of $K$. A particularly readable [claim replication](claim-replication.md) uses two [portfolios](investment-portfolio.md) with nonnegative terminal amounts: portfolio A holds one [European call option](european-call-option.md) and a risk-free [zero-coupon bond](zero-coupon-bond.md) paying $K$ at $T$; portfolio B holds one [European put option](european-put-option.md) and one [stock](stock.md) share. The [zero-coupon bond](zero-coupon-bond.md) costs $Ke^{-rT}$ today, since the [discount factor](discount-factor.md) is $e^{-rT}$. There are no intermediate cash flows. For every terminal [stock](stock.md) price,

$$
A_T=C_T+K=\max(S_T,K)=P_T+S_T=B_T.
$$

For the [strike price](strike-price.md) $K=100$, even the following very different outcomes leave the two [portfolios](investment-portfolio.md) equal:

| Terminal [stock](stock.md) price $S_T$ | A: [European call option](european-call-option.md) + [zero-coupon bond](zero-coupon-bond.md) | B: [European put option](european-put-option.md) + [stock](stock.md) |
| --- | --- | --- |
| $80$ | $0+100=100$ | $20+80=100$ |
| $100$ | $0+100=100$ | $0+100=100$ |
| $120$ | $20+100=120$ | $0+120=120$ |

The [law of one price](law-of-one-price.md) forces $A_0=B_0$ in this setting: otherwise buy the cheaper [portfolio](investment-portfolio.md) and sell the more expensive [portfolio](investment-portfolio.md) using [short selling](short-finance.md). Their terminal obligations cancel in every scenario, while the initial price difference can grow in the [bank account](bank-account.md). Hence absence of [arbitrage](arbitrage.md) gives

$$
C_0+Ke^{-rT}=P_0+S_0,\qquad C_0-P_0=S_0-Ke^{-rT}.
$$

With a constant per-period [interest rate](interest-rate.md) $i$ over $N$ discrete periods, the same reasoning gives $C_0-P_0=S_0-K(1+i)^{-N}$. This is a different compounding convention; $i$ is not the continuously compounded [interest rate](interest-rate.md) $r$.

For an illustrative [stock](stock.md) price $S_0=100$, [strike price](strike-price.md) $K=100$, expiry one year away, [interest rate](interest-rate.md) $r=0.05$ per year, and given [European call option](european-call-option.md) price $C_0=10$, [put-call parity](put-call-parity.md) requires

$$
Ke^{-rT}=100e^{-0.05}\approx95.12294245,\qquad P_0=10+100e^{-0.05}-100\approx5.12294245.
$$

Both [portfolios](investment-portfolio.md) therefore cost approximately $105.12294245$. The inputs specify no [stock](stock.md) price dynamics: $C_0=10$ is supplied for illustration, not calculated from the [Black-Scholes model](black-scholes-model.md). [Put-call parity](put-call-parity.md) determines the [European put option](european-put-option.md) price conditional on that [European call option](european-call-option.md) price; it does not determine both prices by itself. At zero [interest rate](interest-rate.md), the same $S_0=K=100$ and $C_0=10$ give the exact result $P_0=10$.

<a id="image-two-portfolios-with-identical-terminal-cash-flows-and-equal-initial-costs-under-put-call-parity"></a>
![](put-call-parity-replication.png)

**[Figure 2](#image-two-portfolios-with-identical-terminal-cash-flows-and-equal-initial-costs-under-put-call-parity). Two portfolios with identical terminal cash flows and equal initial costs under put-call parity**.

To compute both directions of [arbitrage](arbitrage.md), keep all the preceding inputs except the quoted [European put option](european-put-option.md) price. If it is $6$, portfolio B costs $106$ while portfolio A costs $105.12294245$. Buy A, sell B, and place the initial surplus $6-(10+100e^{-0.05}-100)\approx0.87705755$ in the [bank account](bank-account.md). At expiry, A and the obligations from selling B cancel exactly, leaving $96e^{0.05}-100\approx0.92202525$ in every scenario. If the [European put option](european-put-option.md) instead costs $4$, buy B for $104$ and sell A for $105.12294245$; the initial surplus is approximately $1.12294245$, growing to $100-94e^{0.05}\approx1.18051694$. Both constructions start with zero external capital. They are model calculations under the stated [frictionless market](frictionless-market.md) assumptions.

The beauty of [put-call parity](put-call-parity.md) is that uncertain individual [financial payoffs](contingent-claim-payoff.md) produce an exact relation between today's prices. No forecast of the terminal [stock](stock.md) price and no [probability distribution](probability-distribution-split.md) are needed. It provides a consistency check and lets [claim replication](claim-replication.md) exchange one contract for a combination of others. Dividends introduce extra cash flows, and [American put options](american-put-option.md) can be exercised early, so the displayed European equality cannot simply be transferred to those contracts. K. Foster's [CCNY lecture notes on option values (2010), Put-Call Parity section](https://kfoster.ccny.cuny.edu/classes/spring2010/eco275/lecturenotes5.html) explain the matching [portfolios](investment-portfolio.md); Jun Pan's [MIT Financial Markets teaching notes, Arbitrage Pricing and Dynamic Replication section (PDF p. 130)](https://www.mit.edu/~junpan/Jun_Pan_Teaching_Notes.pdf) discuss [put-call parity](put-call-parity.md) and its dividend adjustment.

An original modern research source is Hans R. Stoll's [The Relationship Between Put and Call Option Prices](https://doi.org/10.1111/j.1540-6261.1969.tb01694.x), _The Journal of Finance_ 24(5), 801-824 (December 1969). Stoll studied the relation between contract prices and tested it against market data; this was a relation between prices rather than a formula fixing each price individually. Robert C. Merton's [1973 comment](https://doi.org/10.1111/j.1540-6261.1973.tb01357.x), 28(1), 183-184, highlighted the importance of excluding premature exercise for an exact [arbitrage](arbitrage.md) equality. This distinction explains why the exercise assumption belongs in the statement of [put-call parity](put-call-parity.md).

**Table of contents**

- [Power put-call parity](power-put-call-parity.md)
- [Put-call symmetry in the Black-Scholes model](put-call-symmetry-in-the-black-scholes-model.md)

## ↑ Ancestors (7)

1. [European call option](european-call-option.md)
2. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Chooser option](chooser-option.md)
- [Dupire equation](dupire-equation.md)
- [European put option](european-put-option.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/28j/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/27j/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/27j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/27j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/29k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3/29k/b/solution.md)
- [Power put-call parity](power-put-call-parity.md)
- [Put-call parity](put-call-parity.md)
- [Put-call symmetry in the Black-Scholes model](put-call-symmetry-in-the-black-scholes-model.md)
