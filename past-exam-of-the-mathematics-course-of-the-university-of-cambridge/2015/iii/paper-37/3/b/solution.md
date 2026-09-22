<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [sample autocorrelation function](../../../../../../sample-autocorrelation-function.md) and [sample partial autocorrelation function](../../../../../../sample-partial-autocorrelation-function.md) to look for approximate cutoffs. For a minimal causal [autoregressive model](../../../../../../autoregressive-model.md) of order $p$, the [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) is zero beyond $p$, while the [autocorrelation function](../../../../../../autocorrelation.md) usually tails off, possibly with damped oscillation. For an invertible [moving-average model](../../../../../../moving-average-model.md) of order $q$, the [autocorrelation function](../../../../../../autocorrelation.md) is zero beyond $q$, while the [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) tails off. In a mixed [autoregressive moving-average model](../../../../../../autoregressive-moving-average-model.md), both generally tail off.

Thus the last visibly nonzero partial correlation suggests an autoregressive order, and the last visibly nonzero autocorrelation suggests a moving-average order. Finite samples do not produce exact zeros. Approximate white-noise reference bands can help flag clearly nonzero lags, but they are not universal [confidence intervals](../../../../../../confidence-interval.md) for arbitrary correlated processes. Fit a few suggested orders and check residual [autocorrelation](../../../../../../autocorrelation.md), rather than treating these plots as a proof of the model order. This is [order identification by autocorrelation cutoffs](../../../../../../order-identification-by-autocorrelation-cutoffs.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
