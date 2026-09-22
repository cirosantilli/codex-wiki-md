# Risk-neutral probability in a binomial market

↑ **Parent:** [Discrete-time binomial market](discrete-time-binomial-market.md)

The [martingale](martingale-split.md) condition for the discounted [stock](stock.md) is $quS_0+(1-q)dS_0=RS_0$. Therefore the up [risk-neutral probability](risk-neutral-probability.md) is

$$
q=\frac{R-d}{u-d},\qquad 1-q=\frac{u-R}{u-d}.
$$

With down factor $d=1+a$, up factor $u=1+b$ and $R=1+r$, this is equivalently $(r-a)/(b-a)$. For $d=0.8$, $u=1.2$, $R=1.05$, it gives $q=0.25/0.4=0.625$. Under the [risk-neutral measure](risk-neutral-measure.md), the terminal [stock](stock.md) price has [expected value](expected-value.md) $(5/8)120+(3/8)80=105$, whose discounted value is 100. The physical [probability](probability.md) $p$ need only satisfy $0<p<1$; it does not enter this calculation.

## ↑ Ancestors (7)

1. [Discrete-time binomial market](discrete-time-binomial-market.md)
2. [Binomial options pricing model](binomial-options-pricing-model.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Backward option pricing](backward-option-pricing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/29k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/29k/b/solution.md)
