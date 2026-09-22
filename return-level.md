# Return level

↑ **Parent:** [Return period](return-period.md)

A [return level](return-level.md) answers the inverse question to a [return period](return-period.md): which threshold has the specified rarity? Let $F(z)=F_{\rm annual}(z)=\mathbb P(M_j\leq z)$ be the common [cumulative distribution function](cumulative-distribution-function.md) of annual [sample maxima](sample-maximum.md) in a model with [stationarity](stationary-process.md). For a continuous, strictly increasing $F$ and $T>1$, the $T$-year [return level](return-level.md) is

$$
z_T=F^{-1}\!\left(1-\frac1T\right),\qquad
F(z_T)=1-\frac1T,\qquad \mathbb P(M_j>z_T)=\frac1T.
$$

It has the same units as $M_j$, whereas $T$ is a count of annual blocks. [Independence](independent-random-variables.md) between years is unnecessary for this one-year [quantile](quantile-function.md) definition; it is needed for the geometric waiting and multi-year formulas under [return period](return-period.md). For a [discrete probability distribution](discrete-probability-distribution-split.md), use the generalized [quantile function](quantile-function.md) $F^{-1}(q)=\inf\{z:F(z)\geq q\}$. Then $\mathbb P(M_j>z_T)\leq1/T$, with equality not guaranteed at jumps; an exact requested exceedance [probability](probability.md) may be unattainable.

For a concrete standard model, choose the maxima convention of the [Gumbel distribution](gumbel-distribution.md), with location $\mu$ and scale $b>0$:

$$
F(z)=\exp\!\left[-\exp\!\left(-\frac{z-\mu}{b}\right)\right],\qquad
z_T=\mu-b\log\!\left[-\log\!\left(1-\frac1T\right)\right].
$$

The second formula follows by taking logarithms twice and solving $F(z_T)=1-1/T$. The maxima [cumulative distribution function](cumulative-distribution-function.md) and its inverse are given in [NIST: extreme value type I distribution, maximum case](https://www.itl.nist.gov/div898/handbook/eda/section3/eda366g.htm). With the deliberately chosen toy values $\mu=10$ and $b=2$ in arbitrary units, $z_{10}=14.501$, $z_{100}=19.200$, and $z_{1000}=23.815$, rounded to three decimals. In particular, $19.200$ is approximately the annual [quantile](quantile-function.md) at cumulative [probability](probability.md) $0.99$; it is not a prediction of the largest observation in the next 100 years. Under [independence](independent-random-variables.md), the [probability](probability.md) that all those annual [sample maxima](sample-maximum.md) stay below the exact $z_{100}$ is $0.99^{100}\approx0.366$.

The time block matters. If a toy year contains $m$ [independent](independent-random-variables.md) daily blocks, each with exceedance [probability](probability.md) $q$ at one fixed threshold, its annual exceedance [probability](probability.md) is $p=1-(1-q)^m$, giving annual [return period](return-period.md) $1/[1-(1-q)^m]$. The reciprocal $1/q$ counts daily blocks. Dependence among daily exceedances requires their joint law instead; a threshold crossed on several successive days still produces only one exceedance indicator for that year's [sample maximum](sample-maximum.md). The [peaks-over-threshold method](peaks-over-threshold-method.md) and [declustering of extremes](declustering-of-extremes.md) address a different choice of extreme-event sampling.

**Table of contents**

- [Return level plot](return-level-plot.md)

## ↑ Ancestors (7)

1. [Return period](return-period.md)
2. [Extreme value theory](extreme-value-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Declustering of extremes](declustering-of-extremes.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/4/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/4/g/solution.md)
- [Peaks-over-threshold method](peaks-over-threshold-method.md)
- [Return level](return-level.md)
- [Return level plot](return-level-plot.md)
