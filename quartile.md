# Quartile

↑ **Parent:** [Descriptive statistics](descriptive-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quartile)

[Quartiles](quartile.md) are the [quantiles](quantile-function.md) at [probability](probability.md) levels $1/4,1/2,3/4$; $Q_2$ is a [median](median.md). For a population we can use its [quantile function](quantile-function.md), $Q_r=Q(r/4)$ for $r=1,2,3$. Finite-sample conventions differ. Our [box plot](box-plot.md) uses linear interpolation between [order statistics](order-statistic.md): for $n\geq2$ and $0<p<1$, set

$$
h=1+(n-1)p,\qquad j=\lfloor h\rfloor,\qquad g=h-j,\qquad \widetilde Q(p)=(1-g)x_{(j)}+g x_{(j+1)}.
$$

Then $Q_r=\widetilde Q(r/4)$. This is R's type-7 convention, described in the documentation authored by Ivan Frohne and Rob J Hyndman. It differs from the generalized-inverse [sample quantile](sample-quantile.md) defined elsewhere in this wiki: for the twelve toy values, that rule selects ranks $3,6,9$ and gives $2,4,6$, rather than $2.75,4.5,6.25$. These are different stated conventions, not arithmetic disagreements. [Frohne and Hyndman, R stats documentation, sample quantile types](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/quantile.html)

**Table of contents**

- [Interquartile range](interquartile-range.md)

## ↑ Ancestors (5)

1. [Descriptive statistics](descriptive-statistics.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Arcsine quantiles and moments](arcsine-quantiles-and-moments.md)
- [Box plot](box-plot.md)
- [Histogram](histogram.md)
- [Interquartile range](interquartile-range.md)
- [Quartile](quartile.md)
