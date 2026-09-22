# Rank of an observation

↑ **Parent:** [Order statistic](order-statistic.md)

The [rank of an observation](rank-of-an-observation.md) records where that observation lies among the [order statistics](order-statistic.md) of a [statistical sample](statistical-sample.md). When all values are distinct, $r_i=1+\#\{j:x_j<x_i\}$ and $x_i=x_{(r_i)}$. For $(0.7,0.1,0.9,0.4,0.2)$, the [ranks of observations](rank-of-an-observation.md) in original order are $(4,1,5,3,2)$: the first observation is fourth smallest, while the fourth observation is third smallest.

Ties require a convention. A tied block occupying sorted positions $a,\ldots,b$ can assign each member the average [rank of an observation](rank-of-an-observation.md) $(a+b)/2$, the minimum position $a$, or the maximum position $b$; an explicit rule can also break ties into distinct positions. R's official documentation describes these choices and uses average ranks by default. [R base documentation: sample ranks and tie methods](https://stat.ethz.ch/R-manual/R-devel/library/base/html/rank.html).

For example, $(0.1,0.4,0.4,0.9)$ has [order statistics](order-statistic.md) $(0.1,0.4,0.4,0.9)$. The two $0.4$ observations occupy positions $2$ and $3$; average [ranks of observations](rank-of-an-observation.md) are $(1,2.5,2.5,4)$, whereas minimum-position ranks are $(1,2,2,4)$. A fractional average rank is a summary of tied positions, rather than an index of one [order statistic](order-statistic.md). Without omissions, distinct ranks and average ranks sum to $n(n+1)/2$, since averaging each tied block preserves its sum; minimum-position ranks need not.

[Wilcoxon signed-rank tests](wilcoxon-signed-rank-test.md) rank the absolute nonzero paired differences, while [Wilcoxon rank sum tests](mann-whitney-u-test.md) rank the pooled observations from two samples; these are different rankings.

## ↑ Ancestors (6)

1. [Order statistic](order-statistic.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Rank of an observation](rank-of-an-observation.md)
