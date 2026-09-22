# Log-mean-reverting price

↑ **Parent:** [Stock](stock.md)

For $\alpha>0$, $\sigma>0$, this positive [stochastic process](stochastic-process-split.md) is the exponential of an [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md). The [Itô formula](ito-s-lemma.md) gives

$$
d\log S_t=\alpha(\widetilde\mu-\log S_t)dt+\sigma dW_t,\qquad\widetilde\mu=\mu-\frac{\sigma^2}{2\alpha}.
$$

The mean level of the logarithm differs from $\mu$ by the [quadratic variation](quadratic-variation.md) correction. In a [stock](stock.md) model, specifying this under a physical probability measure does not by itself specify [risk-neutral pricing](risk-neutral-pricing.md). A non-dividend-paying traded [stock](stock.md) has drift $rS$ under a [risk-neutral measure](risk-neutral-measure.md); a different drift under that measure would require a corresponding dividend or carry convention.

**Table of contents**

- [Conditional mean of a log-mean-reverting price](conditional-mean-of-a-log-mean-reverting-price.md)

## ↑ Ancestors (6)

1. [Stock](stock.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Conditional mean of a log-mean-reverting price](conditional-mean-of-a-log-mean-reverting-price.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2023/3/a/solution.md)
