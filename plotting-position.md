# Plotting position

↑ **Parent:** [Q-Q plot](q-q-plot.md)

A [plotting position](plotting-position.md) assigns a [probability](probability.md) level to an [order statistic](order-statistic.md) for a [Q-Q plot](q-q-plot.md). The displayed formula is one convention, not a universal definition. R's `ppoints` uses $p_i=(i-a)/(n+1-2a)$, with $a=1/2$ by default for $n>10$, which gives our choice at $n=19$; for $n\leq10$ its default is $a=3/8$. NIST's [normal probability plot](normal-q-q-plot.md) instead describes an approximation to [uniform distribution](continuous-uniform-distribution.md) [order statistic](order-statistic.md) medians. State the convention when comparing plots, especially their extreme [quantiles](quantile-function.md). [R stats documentation, ppoints](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/ppoints.html)[NIST/SEMATECH, Normal Probability Plot, definition](https://www.itl.nist.gov/div898/handbook/eda/section3/normprpl.htm)

## ↑ Ancestors (5)

1. [Q-Q plot](q-q-plot.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Normal Q-Q plot](normal-q-q-plot.md)
- [Plotting position](plotting-position.md)
- [Q-Q plot](q-q-plot.md)
