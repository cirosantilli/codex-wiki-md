# Constant intensity does not imply independence

↑ **Parent:** [Intensity measure of a point process](intensity-measure-of-a-point-process.md)

The same [intensity measure](intensity-measure-of-a-point-process.md) can belong to very different [point processes](point-process.md). A [Poisson point process](poisson-point-process.md) with a locally finite [intensity measure](intensity-measure-of-a-point-process.md) $\mu$ adds two requirements: each finite-intensity window count has the [Poisson distribution](poisson-distribution.md) of mean $\mu(W)$, and counts in pairwise [disjoint observation windows](disjoint-observation-windows.md) are mutually [independent](independent-random-variables.md). These requirements determine its [probability law](probability-distribution.md); they do not follow from the formula for $\mu$.[Section 3.1, Definition 3.1 and Proposition 3.2, printed pp. 19-20: Poisson count laws, independence, and uniqueness](lectures-on-the-poisson-process-by-gunter-last-and-others.md)

A [randomly shifted lattice point process](randomly-shifted-lattice-point-process.md), a unit-rate [Poisson point process](poisson-point-process.md), and the [shared random rate gives dependent point counts](shared-random-rate-gives-dependent-point-counts.md) construction all satisfy $\mu(A)=|A|$ on the real line. Nevertheless, their counts in $[0,1)$ have respectively [variance](variance-split.md) zero, one, and two. Counts in the [disjoint observation windows](disjoint-observation-windows.md) $[0,1/2)$ and $[1/2,1)$ have respectively [covariance](covariance.md) $-1/4$, zero, and $1/4$. These exact calculations show why measuring mean density cannot identify a spacing or [statistical dependence](statistical-dependence.md) model.

<a id="image-equal-intensity-permits-regular-spacing-poisson-counts-and-shared-rate-dependence"></a>
![](point-process-equal-intensity-different-count-laws.png)

**[Figure 4](#image-equal-intensity-permits-regular-spacing-poisson-counts-and-shared-rate-dependence). Equal intensity permits regular spacing, Poisson counts, and shared-rate dependence**. All three laws have [intensity measure](intensity-measure-of-a-point-process.md) $\mu(A)=|A|$. Left: illustrative realizations of a [randomly shifted lattice point process](randomly-shifted-lattice-point-process.md), a unit-rate [Poisson point process](poisson-point-process.md), and the [shared random rate gives dependent point counts](shared-random-rate-gives-dependent-point-counts.md) construction conditional on rate two; the latter also has a completely empty outcome with [probability](probability.md) $1/2$. Right: exact [probability mass functions](probability-mass-function.md) of the count in $[0,1)$, with the axis displayed through seven. Equal [expected values](expected-value.md) of one coexist with [variances](variance-split.md) zero, one, and two. Realizations illustrate spacing; the bars describe laws, not frequencies estimated from those realizations.

**Table of contents**

- [Randomly shifted lattice point process](randomly-shifted-lattice-point-process.md)
- [Shared random rate gives dependent point counts](shared-random-rate-gives-dependent-point-counts.md)

## ↑ Ancestors (7)

1. [Intensity measure of a point process](intensity-measure-of-a-point-process.md)
2. [Point process](point-process.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
