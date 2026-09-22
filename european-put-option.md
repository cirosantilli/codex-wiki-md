# European put option

↑ **Parent:** [Put option](put-option.md)

A [European put option](european-put-option.md) gives its holder the right, without an obligation, to sell one unit of an underlying [financial asset](financial-asset.md) at the [strike price](strike-price.md) $K$ only on the expiry date $T$. For one [stock](stock.md) share, its terminal [financial payoff](contingent-claim-payoff.md) is the [positive part](positive-part-of-a-real-valued-function.md)

$$
P_T=(K-S_T)^+=\begin{cases}K-S_T,&S_T<K,\\0,&S_T\geq K.\end{cases}
$$

For [strike price](strike-price.md) $K=100$, terminal [stock](stock.md) prices $80$, $100$, and $120$ give [financial payoffs](contingent-claim-payoff.md) $20$, $0$, and $0$, respectively. At $S_T=80$, selling for $100$ rather than the market price $80$ supplies the difference $20$; at $S_T=120$, the holder can let the right expire. Equality at $S_T=100$ gives zero net exercise value. The [European call option](european-call-option.md) example plots both [financial payoffs](contingent-claim-payoff.md) on the same axes.

Combining a [European put option](european-put-option.md) with the underlying [stock](stock.md) share produces the terminal amount $S_T+(K-S_T)^+=\max(S_T,K)$. Its floor at the [strike price](strike-price.md) is why a [European put option](european-put-option.md) can describe protection against a fall in terminal [stock](stock.md) value. The protection has an initial cost and lasts to the specified expiry; the terminal floor alone says nothing about the [financial return](financial-return.md). [Put-call parity](put-call-parity.md) replicates this same amount with a [European call option](european-call-option.md) and a [zero-coupon bond](zero-coupon-bond.md).

Using the [put-call parity](put-call-parity.md) example's price $P_0=10+100e^{-0.05}-100\approx5.12294245$, the cost financed for one year at [interest rate](interest-rate.md) $r=0.05$ grows to $P_0e^{0.05}=100-90e^{0.05}\approx5.38560133$. The terminal net amount is therefore approximately $14.61439867$ when $S_T=80$, and $-5.38560133$ when $S_T=100$ or $120$. These computations use the unrounded price and distinguish the [financial payoff](contingent-claim-payoff.md) from the financed gain. Unlike an [American put option](american-put-option.md), a [European put option](european-put-option.md) supplies no right to exercise before $T$.

## ↑ Ancestors (8)

1. [Put option](put-option.md)
2. [Contingent claim](contingent-claim.md)
3. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Chooser option](chooser-option.md)
- [Contingent claim payoff](contingent-claim-payoff.md)
- [European call option](european-call-option.md)
- [European put option](european-put-option.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/27j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/27j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/27j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/29k/b/solution.md)
- [Put-call parity](put-call-parity.md)
- [Put option](put-option.md)
- [Strike price](strike-price.md)
