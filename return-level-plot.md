# Return level plot

↑ **Parent:** [Return level](return-level.md)

A [return level plot](return-level-plot.md) graphs $T$ horizontally and $z_T$ vertically, often using a [logarithmic scale](logarithmic-scale.md) for $T$. To read it, choose a [return period](return-period.md), move up to the curve, and read the corresponding [return level](return-level.md). Conversely, a threshold's horizontal coordinate gives the reciprocal of its annual exceedance [probability](probability.md). The usual plot of fitted [quantiles](quantile-function.md) against [return periods](return-period.md), and optional pointwise [confidence intervals](confidence-interval.md), are documented in [Mathieu Ribatet, POT package: return level plot](https://search.r-project.org/CRAN/refmans/POT/html/retlev.html).

<a id="image-an-exact-toy-gumbel-return-level-curve-maps-rarity-to-a-threshold"></a>
![](gumbel-return-level-curve.png)

**[Figure 3](#image-an-exact-toy-gumbel-return-level-curve-maps-rarity-to-a-threshold). An exact toy Gumbel return-level curve maps rarity to a threshold**. The maxima [Gumbel distribution](gumbel-distribution.md) has chosen parameters $\mu=10$ and $b=2$ in arbitrary units. The upper axis shows annual exceedance [probability](probability.md) $1/T$. Markers are exact model [quantiles](quantile-function.md), not data or fitted estimates; the dotted line is the large-$T$ approximation $10+2\log T$.

The near-straight shape has a mathematical explanation: since $-\log(1-1/T)\sim1/T$ as $T\to\infty$, the [Gumbel distribution](gumbel-distribution.md) gives $z_T=\mu+b\log T+o(1)$. Multiplying a large [return period](return-period.md) by ten therefore increases the [return level](return-level.md) by approximately $b\log10$, about $4.605$ units for this toy curve. A curve indexed by rarity puts several thresholds on one common scale while retaining their measurement units.

For a fitted curve, a pointwise [confidence interval](confidence-interval.md) concerns uncertainty in the estimated [quantile](quantile-function.md) at a specified $T$; it is distinct from a [prediction interval](prediction-interval.md) for a future annual [sample maximum](sample-maximum.md), and pointwise intervals need not form a simultaneous [confidence band](confidence-band.md). A far-right curve value can also be an extrapolation beyond the observation record: extending the line adds no observations to support the chosen tail model. The diagram above uses fixed toy parameters, so it shows neither estimation uncertainty nor an observational record. Its interpretation throughout assumes the stated annual block and [stationarity](stationary-process.md).

## ↑ Ancestors (8)

1. [Return level](return-level.md)
2. [Return period](return-period.md)
3. [Extreme value theory](extreme-value-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/4/f/solution.md)
- [Return level plot](return-level-plot.md)
