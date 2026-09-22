# Extreme value theory

↑ **Parent:** [Probability theory](probability-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extreme_value_theory)

[Extreme value theory](extreme-value-theory.md) studies limiting [probability distributions](probability-distribution.md) of normalized [sample maxima](sample-maximum.md) and related extremes. The standard limits for maxima include the [Fréchet distribution](frechet-distribution.md), [negative Weibull distribution](negative-weibull-distribution.md), and [Gumbel distribution](gumbel-distribution.md).

The question is often practical: if a batch finishes only when its slowest task finishes, its completion time is a [sample maximum](sample-maximum.md). A typical individual delay or a [sample mean](sample-mean.md) does not answer that question. The [central limit theorem](central-limit-theorem.md) describes suitably normalized sums and [sample means](sample-mean.md) under its assumptions; it does not give a limit law for [sample maxima](sample-maximum.md). [Extreme value theory](extreme-value-theory.md) instead describes how the largest observation changes as the number of opportunities for a large observation grows.

For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) $X_1,X_2,\ldots$ with [distribution function](cumulative-distribution-function.md) $F$, define the [sample maximum](sample-maximum.md)

$$
M_n=\max_{1\leq i\leq n}X_i.
$$

The [event](event.md) $M_n\leq x$ means that every observation is at most $x$, so [independence](independent-random-variables.md) gives

$$
\mathbb P(M_n\leq x)=\prod_{i=1}^n\mathbb P(X_i\leq x)=F(x)^n.
$$

[Extreme value theory](extreme-value-theory.md) asks whether there are constants $a_n>0$ and $c_n\in\mathbb R$ for which $(M_n-c_n)/a_n$ has [convergence in distribution](convergence-in-distribution.md) to a [non-degenerate probability distribution](non-degenerate-probability-distribution.md). Equivalently, $F(c_n+a_nz)^n$ must tend to a limiting [distribution function](cumulative-distribution-function.md) at its continuity points. The [extremal types theorem](extremal-types-theorem.md) says that any such limit belongs, up to a change of location and positive scale, to the [Gumbel distribution](gumbel-distribution.md), [Fréchet distribution](frechet-distribution.md), or [negative Weibull distribution](negative-weibull-distribution.md). It does not guarantee that a limit exists for every $F$. [Smith and Weissman, Extreme Values, Section 1.2.1: the three types theorem](https://rls.sites.oasis.unc.edu/s834-2023/ExtremeValues.pdf).

The [maximum of independent exponential random variables](maximum-of-independent-exponential-random-variables.md) gives a particularly transparent worked example: its center grows as $(\log n)/\lambda$, and its fluctuations have a [Gumbel distribution](gumbel-distribution.md) limit on the scale $1/\lambda$. Here and below $\log$ denotes the [natural logarithm](natural-logarithm.md). This normalization depends on the [exponential distribution](exponential-distribution.md). Other [survival functions](survival-function.md) can lead to the [Fréchet distribution](frechet-distribution.md) or [negative Weibull distribution](negative-weibull-distribution.md), with different constants $a_n,c_n$; the [Gumbel distribution](gumbel-distribution.md) and the exponential example's normalization are not universal.

[Independence](independent-random-variables.md) is essential to the product calculation. If instead $X_1=X_2=\cdots=X$ for one rate-$\lambda$ [exponential random variable](exponential-distribution.md), then $M_n=X$ for every $n$. Its [distribution function](cumulative-distribution-function.md) stays $1-e^{-\lambda x}$ for $x\geq0$ and zero below zero, and its [median](median.md) stays $(\log2)/\lambda$. Perfect dependence creates no logarithmic growth: repeating the same [random variable](random-variable-split.md) supplies no new chance of a larger value.

A historical starting point is R. A. Fisher and L. H. C. Tippett's 1928 paper on limiting laws of the largest or smallest sample member, published in volume 24, issue 2, pages 180–190 of the Proceedings of the Cambridge Philosophical Society. Its abstract studies the possible limiting forms and emphasizes that approach to a limit can be slow. [Fisher and Tippett (1928), Limiting forms of the frequency distribution of the largest or smallest member of a sample: publisher metadata and abstract](https://www.cambridge.org/core/journals/mathematical-proceedings-of-the-cambridge-philosophical-society/article/abs/limiting-forms-of-the-frequency-distribution-of-the-largest-or-smallest-member-of-a-sample/7BE8DE65FCDFC3ABECFE1054DFB56CB5).

**Table of contents**

- [Maximum of independent exponential random variables](maximum-of-independent-exponential-random-variables.md)
- [Hill estimator](hill-estimator.md)
- [Extremal types theorem](extremal-types-theorem.md)
- [Max-stable distribution](max-stable-distribution.md)
- [Return period](return-period.md)
  - [Return level](return-level.md)
    - [Return level plot](return-level-plot.md)
- [Generalized Pareto distribution](generalized-pareto-distribution.md)
  - [Orthogonal shape and scale for a generalized Pareto distribution](orthogonal-shape-and-scale-for-a-generalized-pareto-distribution.md)
  - [Peaks-over-threshold method](peaks-over-threshold-method.md)
    - [Declustering of extremes](declustering-of-extremes.md)
  - [Pickands-Balkema-de Haan theorem](pickands-balkema-de-haan-theorem.md)
- [Gumbel distribution](gumbel-distribution.md)
  - [Moving Gumbel cutoff in an inverse-power tail](moving-gumbel-cutoff-in-an-inverse-power-tail.md)
  - [Gumbel limit for gamma maxima](gumbel-limit-for-gamma-maxima.md)
  - [Gumbel auxiliary function](gumbel-auxiliary-function.md)
- [Negative Weibull distribution](negative-weibull-distribution.md)
- [Fréchet distribution](frechet-distribution.md)
- [Maximum domain of attraction](maximum-domain-of-attraction.md)
  - [Logarithmic-tail Fréchet normalization](logarithmic-tail-frechet-normalization.md)
  - [Von Mises conditions for extreme values](von-mises-conditions-for-extreme-values.md)

## ↑ Ancestors (5)

1. [Probability theory](probability-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Extreme value theory](extreme-value-theory.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/3/solution.md)
- [Regular variation](regular-variation.md)
