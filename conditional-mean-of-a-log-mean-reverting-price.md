# Conditional mean of a log-mean-reverting price

↑ **Parent:** [Log-mean-reverting price](log-mean-reverting-price.md)

For a [log-mean-reverting price](log-mean-reverting-price.md), set $a=e^{-\alpha(T-t)}$. The [Ornstein-Uhlenbeck transition distribution](ornstein-uhlenbeck-transition-distribution.md) gives conditional log-mean $a\log S_t+(1-a)\widetilde\mu$ and log-variance $\sigma^2(1-a^2)/(2\alpha)$. The [moment-generating function of a normal distribution](moment-generating-function-of-a-normal-distribution.md) therefore gives the displayed formula for $F(t,T)=\mathbb E[S_T\mid\mathcal F_t]$. It is a [martingale](martingale-split.md) in $t$ for fixed $T$, by the [tower property of conditional expectation](law-of-total-expectation.md), and the [Itô formula](ito-s-lemma.md) yields

$$
dF(t,T)=\sigma e^{-\alpha(T-t)}F(t,T)dW_t.
$$

This uses the same probability measure as the specified [conditional expectation](conditional-expectation.md). It describes [futures pricing](futures-pricing.md) only when that measure is an appropriate pricing measure, with the required cash-flow conventions. For a non-dividend-paying traded [stock](stock.md) and constant [interest rate](interest-rate.md), the [forward contract](forward-contract.md) delivery price follows the usual carry relation instead.

## ↑ Ancestors (7)

1. [Log-mean-reverting price](log-mean-reverting-price.md)
2. [Stock](stock.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2023/3/c/solution.md)
