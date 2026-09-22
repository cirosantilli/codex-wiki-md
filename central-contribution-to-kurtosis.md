# Central contribution to kurtosis

↑ **Parent:** [Kurtosis](kurtosis.md)

For a [standard score](standard-score.md) $Z$ and $h>0$, split [kurtosis](kurtosis.md) into the contribution $C_h$ from within $h$ [standard deviations](standard-deviation.md) of the [mean](expected-value.md) and the contribution $T_h$ from outside:

$$
\kappa=C_h+T_h,\qquad C_h=\mathbb E[Z^4\mathbf1_{\{|Z|\leq h\}}],\qquad 0\leq C_h\leq h^4.
$$

The [indicator function](indicator-function.md) selects the central outcomes. The bound follows directly from $Z^4\leq h^4$ there. Thus $C_h/\kappa\leq h^4/\kappa$: when [kurtosis](kurtosis.md) is large, any fixed central range contributes a small fraction. This is a precise reason to emphasize extreme [standard scores](standard-score.md) rather than peak height.[§5, Why Tails Mostly Determine Kurtosis, inequality (1) and following fixed-h argument](kurtosis-as-peakedness-1905-2014-r-i-p-by-peter-h-westfall.md)

For the [rare-outlier three-point distribution](rare-outlier-three-point-distribution.md) with $q=1/100$, $C_1=0$ and $T_1=100$. At the other endpoint $q=1$, all [probability mass](probability-mass.md) lies at $Z=\pm1$, so $C_1=\kappa=1$: central dominance is possible when [kurtosis](kurtosis.md) is small. More generally, the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $\kappa=\mathbb E[Z^4]\geq(\mathbb E[Z^2])^2=1$; the equally weighted outcomes $\pm1$ attain this minimum.

## ↑ Ancestors (7)

1. [Kurtosis](kurtosis.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
