# Weighted geometric mean

↑ **Parent:** [Geometric mean](geometric-mean.md)

For positive [real numbers](real-number.md) $x_i$ and nonnegative weights with $\sum_iw_i=1$, the weighted geometric mean is

$$
G_w=\prod_i x_i^{w_i}=\exp\left(\sum_iw_i\log x_i\right).
$$

It takes a [weighted mean](weighted-arithmetic-mean.md) of [logarithms](logarithm.md). A zero weight excludes that input; equal weights give the ordinary [geometric mean](geometric-mean.md). If $x_i$ occurs $m_i$ times in a list of total length $M$, its correct weight is $w_i=m_i/M$. For the list $(12,3,3,3)$,

$$
G_w=12^{1/4}3^{3/4}=3\sqrt2\approx4.24264,
$$

and replacing all four entries by $G_w$ preserves the product $324$.

There is also an optimization interpretation. A [logarithmic transformation](logarithmic-transformation.md) turns multiplicative discrepancies into additive ones. For a positive representative $c$, the [weighted mean minimizes squared deviations](weighted-mean-minimizes-squared-deviations.md) identity gives

$$
\sum_iw_i(\log x_i-\log c)^2=\sum_iw_i(\log x_i-\log G_w)^2+(\log c-\log G_w)^2.
$$

Thus $c=G_w$ uniquely minimizes weighted [quadratic loss](squared-error-loss.md) in logarithmic coordinates. The [weighted arithmetic mean](weighted-arithmetic-mean.md) minimizes squared discrepancies in the original coordinates. These two objectives explain why different choices of what constitutes an error select different summaries.

The [strictly concave function](strictly-concave-function.md) $\log x$ and the reversed [Jensen's inequality](jensen-s-inequality.md) give $G_w\leq A_w$, where $A_w=\sum_iw_ix_i$ is the [weighted arithmetic mean](weighted-arithmetic-mean.md). Apply the same reasoning to the [multiplicative inverses](multiplicative-inverse.md) to get $H_w\leq G_w$ for the [weighted harmonic mean](weighted-harmonic-mean.md). Thus $H_w\leq G_w\leq A_w$; equality holds exactly when all positive-weight inputs agree. For this list, $H_w=48/13$, $G_w=3\sqrt2$, and $A_w=21/4$. The weights specify which inputs are represented and must stay the same across the comparison.

## ↑ Ancestors (5)

1. [Geometric mean](geometric-mean.md)
2. [Arithmetic](arithmetic-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
