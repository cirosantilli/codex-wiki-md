# Quantile function

↑ **Parent:** [Probability distribution](probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantile_function)

The [quantile function](quantile-function.md) converts a cumulative probability level into a value. For a [cumulative distribution function](cumulative-distribution-function.md) $F$ and $0<p<1$, use the generalized inverse

$$
Q(p)=\inf\{x:F(x)\geq p\}.
$$

It selects the first threshold reaching the requested level. The [infimum](infimum.md) handles jumps and flat portions, so this construction does not require an ordinary [inverse function](inverse-function.md). Other endpoint conventions are possible at $p=0$ or $p=1$; the open probability [interval](interval-mathematics.md) avoids those issues. NIST introduces the inverse-direction question as the percent point function. [NIST: cumulative distribution and percent point functions](https://itl.nist.gov/div898/handbook/eda/section3/eda362.htm).

For the finite example under [probability distribution](probability-distribution-split.md),

$$
Q_X(p)=\begin{cases}
0,&0<p\leq0.2,\\
1,&0.2<p\leq0.7,\\
3,&0.7<p<1.
\end{cases}
$$

Thus $Q_X(0.1)=0$, $Q_X(0.5)=1$, $Q_X(0.9)=3$. The value at $p=0.2$ is still zero, because $F_X(0)=0.2$ already reaches that level. For $F_Y(y)=y^2$ on $[0,1]$, the [quantile function](quantile-function.md) is $Q_Y(p)=\sqrt p$, giving $Q_Y(0.5)=1/\sqrt2\approx0.70710678$.

<a id="image-quantile-functions-map-probability-levels-to-outcomes-including-repeated-outcomes"></a>
![](quantile-generalized-inverse.png)

**[Figure 10](#image-quantile-functions-map-probability-levels-to-outcomes-including-repeated-outcomes). Quantile functions map probability levels to outcomes, including repeated outcomes**. Left: the three probability bands of widths $0.2$, $0.5$ and $0.3$ map to outcomes $0$, $1$ and $3$. Right: the [quantile function](quantile-function.md) $\sqrt p$ maps the same probability levels to the continuous density example. The marked levels are $0.1$, $0.5$ and $0.9$. Endpoints at $p=0$ and $p=1$ are shown open because the stated [quantile function](quantile-function.md) convention uses $0<p<1$.

A [median](median.md) is a central threshold; $Q(1/2)$ supplies one, though a [median](median.md) need not be unique. The same [quantile function](quantile-function.md) becomes a sampling algorithm through [inverse transform sampling](inverse-transform-sampling.md). Jumps in $F$ become flat bands in $Q$, precisely the mechanism needed to assign positive probability to one outcome.

**Table of contents**

- [Percentile](percentile.md)
- [Probable error](probable-error.md)
- [Sample quantile](sample-quantile.md)
- [Quantile endpoint at probability one](quantile-endpoint-at-probability-one.md)
- [Left continuity of the quantile function](left-continuity-of-the-quantile-function.md)
- [Quantile derivative identity](quantile-derivative-identity.md)
- [Inverse transform sampling](inverse-transform-sampling.md)
  - [Recycling a uniform random variable after discrete sampling](recycling-a-uniform-random-variable-after-discrete-sampling.md)
- [Quantile coupling for convergence in distribution](quantile-coupling-for-convergence-in-distribution.md)

## ↑ Ancestors (6)

1. [Probability distribution](probability-distribution-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (35)

- [Arcsine quantiles and moments](arcsine-quantiles-and-moments.md)
- [Gumbel distribution](gumbel-distribution.md)
- [Inverse transform sampling](inverse-transform-sampling.md)
- [Left continuity of the quantile function](left-continuity-of-the-quantile-function.md)
- [Maximum of independent exponential random variables](maximum-of-independent-exponential-random-variables.md)
- [Monotone rearrangement](monotone-rearrangement.md)
- [Monotonic function](monotonic-function.md)
- [Nondecreasing function](nondecreasing-function.md)
- [Normal Q-Q plot](normal-q-q-plot.md)
- [Pareto distribution](pareto-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/2/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/26k/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-210/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/28l/a/solution.md)
- [Probability distribution](probability-distribution-split.md)
- [Probability integral transform](probability-integral-transform.md)
- [Probable error](probable-error.md)
- [Q-Q plot](q-q-plot.md)
- [Quantile derivative identity](quantile-derivative-identity.md)
- [Quantile endpoint at probability one](quantile-endpoint-at-probability-one.md)
- [Quantile function](quantile-function.md)
- [Quartile](quartile.md)
- [Rayleigh radial thresholds and quantiles](rayleigh-radial-thresholds-and-quantiles.md)
- [Return level](return-level.md)
- [Sampling a discrete uniform distribution](sampling-a-discrete-uniform-distribution.md)
- [Tail probability](tail-probability.md)
