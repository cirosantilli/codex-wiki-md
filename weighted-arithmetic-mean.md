# Weighted arithmetic mean

↑ **Parent:** [Sum](sum.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weighted_arithmetic_mean)

The [weighted arithmetic mean](weighted-arithmetic-mean.md) combines values according to how much each contributes to the quantity being summarized. For a finite list of [real numbers](real-number.md) $x_i$ and nonnegative weights $w_i$ with $W=\sum_iw_i>0$, define

$$
\boxed{\bar x_w=\frac{\sum_iw_ix_i}{W}.}
$$

Zero weights ignore an entry; at least one weight must be positive. Multiplying every weight by the same positive number leaves the result unchanged. Writing $p_i=w_i/W$ makes the [weighted mean](weighted-arithmetic-mean.md) a [convex combination](convex-combination.md), since $p_i\ge0$ and $\sum_i p_i=1$. It therefore lies between the smallest and largest input values. [NIST Dataplot reference manual: weighted mean](https://www.itl.nist.gov/div898/software/dataplot/refman2/ch2/weigmean.pdf)

For example, give the values $90$ and $60$ weights $2$ and $8$:

$$
\bar x_w=\frac{2\cdot90+8\cdot60}{2+8}=\boxed{66}.
$$

The larger weight pulls the result closer to $60$. The balancing identity

$$
\sum_i w_i(x_i-\bar x_w)=0
$$

explains a geometric interpretation: if the weights were masses placed at positions $x_i$, the [weighted mean](weighted-arithmetic-mean.md) would be their [center of mass](center-of-mass.md). Here $8(66-60)=2(90-66)=48$, so the two sides balance even though their distances from the mean differ.

Weights need an interpretation. They can represent numbers of observations, masses, or probabilities in a finite [probability distribution](probability-distribution-split.md). These meanings lead to the same formula, while answering different questions. For instance, [combining means of groups](combining-means-of-groups.md) uses group sizes as weights to recover the mean over individual observations. For a [function](function-split.md) $f$ and nonnegative weight function $w$, the analogous [integral](integral-split.md) is $\int wf/\int w$, provided $wf$ is integrable and the total weight $\int w$ is positive and finite.

**Table of contents**

- [Combining means of groups](combining-means-of-groups.md)
- [Weighted mean minimizes squared deviations](weighted-mean-minimizes-squared-deviations.md)
- [Arithmetic mean](arithmetic-mean.md)
  - [Harmonic mean](harmonic-mean.md)
    - [Weighted harmonic mean](weighted-harmonic-mean.md)

## ↑ Ancestors (7)

1. [Sum](sum.md)
2. [Summation](summation.md)
3. [Addition](addition.md)
4. [Arithmetic](arithmetic-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Average memory access time](average-memory-access-time.md)
- [Expected value](expected-value-split.md)
- [Isotopic abundance](isotopic-abundance.md)
- [Mixing calorimetry](mixing-calorimetry.md)
- [Normalizing extensive quantities](normalizing-extensive-quantities.md)
- [Synthetic insulin-glucagon response model](synthetic-insulin-glucagon-response-model.md)
- [Tail probability](tail-probability.md)
- [Weighted arithmetic mean](weighted-arithmetic-mean.md)
- [Weighted geometric mean](weighted-geometric-mean.md)
- [Weighted harmonic mean](weighted-harmonic-mean.md)
