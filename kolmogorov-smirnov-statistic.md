# Kolmogorov-Smirnov statistic

↑ **Parent:** [Kolmogorov-Smirnov test](kolmogorov-smirnov-test.md)

For an [empirical distribution function](empirical-distribution-function.md) $F_n$ and a specified [cumulative distribution function](cumulative-distribution-function.md) $F_0$, the one-sample [Kolmogorov-Smirnov statistic](kolmogorov-smirnov-statistic.md) is their [Kolmogorov distance](kolmogorov-distance.md):

$$
F_n(x)=\frac1n\sum_{j=1}^n\mathbf1_{\{X_j\leq x\}},\qquad
D_n=\sup_{x\in\mathbb R}|F_n(x)-F_0(x)|.
$$

The displayed sum uses an [indicator function](indicator-function.md). With this convention, $F_n$ is [right-continuous](right-continuous-function.md). For distinct observations, its value and its left [one-sided limit](one-sided-limit.md) at the $i$th [order statistic](order-statistic.md) are $F_n(X_{(i)})=i/n$ and $F_n(X_{(i)}^-)=(i-1)/n$.

For [continuous](continuous-function.md) $F_0$, both jump sides matter. Define the two directional discrepancies by

$$
D_n^+=\sup_x(F_n(x)-F_0(x))
=\max_{1\leq i\leq n}\left\{\frac{i}{n}-F_0(X_{(i)})\right\},
$$



$$
D_n^-=\sup_x(F_0(x)-F_n(x))
=\max_{1\leq i\leq n}\left\{F_0(X_{(i)})-\frac{i-1}{n}\right\},\qquad
D_n=\max(D_n^+,D_n^-).
$$

Thus $D_n^+$ uses the [empirical distribution function](empirical-distribution-function.md) immediately after a jump, and $D_n^-$ uses its left [one-sided limit](one-sided-limit.md).[1.3.5.16. Kolmogorov-Smirnov Goodness-of-Fit Test](nist-and-sematech-e-handbook-of-statistical-methods/1-3-5-16-kolmogorov-smirnov-goodness-of-fit-test.md) A [supremum](supremum.md) need not be attained.

For $n=4$, $F_0(x)=x$ on $[0,1]$, and the stipulated [order statistics](order-statistic.md) $(1/10,2/5,4/5,9/10)$, the complete calculation is

$$
\begin{array}{c|c|c|c|c|c}
i&X_{(i)}&F_4(X_{(i)}^-)&F_4(X_{(i)})&i/4-F_0(X_{(i)})&F_0(X_{(i)})-(i-1)/4\\\hline
1&1/10&0&1/4&3/20&1/10\\
2&2/5&1/4&1/2&1/10&3/20\\
3&4/5&1/2&3/4&-1/20&3/10\\
4&9/10&3/4&1&1/10&3/20
\end{array}
$$

The last two columns give the signed directional gaps: $D_4^+=3/20$, $D_4^-=3/10$, and $D_4=3/10$. In contrast, checking only $|F_4(X_{(i)})-F_0(X_{(i)})|$ gives $3/20$ and misses the largest gap approached as $x\uparrow4/5$. At $x=4/5$ itself, the gap has already fallen to $1/20$.

<a id="image-both-jump-sides-determine-the-exact-kolmogorov-smirnov-statistic"></a>
![](kolmogorov-smirnov-ecdf-jump-gaps.png)

**[Figure 3](#image-both-jump-sides-determine-the-exact-kolmogorov-smirnov-statistic). Both jump sides determine the exact Kolmogorov-Smirnov statistic**. The [empirical distribution function](empirical-distribution-function.md) for four stipulated rational observations is compared with the [uniform distribution](continuous-uniform-distribution.md) on $[0,1]$. Open circles show left [one-sided limits](one-sided-limit.md); filled circles show values at jumps. The green gap is $D_4^+=3/20$ and the magenta gap is the limiting $D_4^-=3/10$.

The finite formula follows from the behavior between jumps: the [empirical distribution function](empirical-distribution-function.md) $F_n$ is constant and the [cumulative distribution function](cumulative-distribution-function.md) $F_0$ is [monotone](monotonic-function.md), so the largest directional gaps occur at the two interval ends, possibly as [one-sided limits](one-sided-limit.md). The two tails introduce no larger gap. Checking every jump side therefore gives the exact [supremum](supremum.md).

A common normalized [Kolmogorov-Smirnov statistic](kolmogorov-smirnov-statistic.md) is $\sqrt nD_n$, which equals $3/5$ in this example. Its large-sample reference law comes from the [Kolmogorov-Smirnov theorem](kolmogorov-smirnov-theorem.md). The unscaled $D_n$ remains the largest difference of cumulative [probabilities](probability.md), not a [p-value](p-value.md).

There is a useful exact exception to the usual warning about fitting [statistical parameters](statistical-parameter.md). Suppose $n\geq2$ [independent and identically distributed](independent-and-identically-distributed-random-variables.md) observations have the [uniform distribution](continuous-uniform-distribution.md) on $(0,\theta)$ with unknown $\theta>0$. Let $M=\max_iX_i$ and let $J$ be the label of its almost surely unique maximizing observation. Conditional on $M=m$ and $J=j$, the surviving labelled observations $(X_i)_{i\ne j}$ are [independent](independent-random-variables.md) with the [uniform distribution](continuous-uniform-distribution.md) on $(0,m)$; after division by $m$ they are [independent and identically distributed](independent-and-identically-distributed-random-variables.md) uniforms on $(0,1)$. These are [conditional distributions](conditional-distribution.md) defined by [probability density functions](probability-density-function.md), since the event $M=m$ has [probability](probability.md) zero.

To check this, the joint [probability density function](probability-density-function.md) of $M$ and $J=j$ is $m^{n-1}/\theta^n$ for $0<m<\theta$. Dividing the original joint [probability density function](probability-density-function.md) $\theta^{-n}$ by this factor gives the conditional survivor [probability density function](probability-density-function.md)

$$
m^{-(n-1)}\prod_{i\ne j}\mathbf1_{\{0<x_i<m\}}.
$$

This factorization proves the claimed [conditional independence](conditional-independence.md); scaling removes $m$. Keep the surviving labels in a fixed order, or apply an [independent](independent-random-variables.md) random [permutation](permutation.md). The sorted survivors instead have the joint law of [uniform order statistics](uniform-order-statistic.md) and exhibit [statistical dependence](statistical-dependence.md); sorting does not affect their [empirical distribution function](empirical-distribution-function.md). Delete the maximum itself, which would otherwise become a forced value $1$, and compute the [Kolmogorov-Smirnov statistic](kolmogorov-smirnov-statistic.md) using [sample size](sample-size.md) $n-1$ and jump heights $i/(n-1)$. This gives an exact conditional [Kolmogorov-Smirnov test](kolmogorov-smirnov-test.md) under the uniform-endpoint [statistical model](statistical-model-split.md). It does not justify fitting an arbitrary endpoint or other [statistical parameters](statistical-parameter.md) and using the ordinary $n$-sample calibration.

## ↑ Ancestors (6)

1. [Kolmogorov-Smirnov test](kolmogorov-smirnov-test.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Kolmogorov-Smirnov confidence band](kolmogorov-smirnov-confidence-band.md)
- [Kolmogorov-Smirnov statistic](kolmogorov-smirnov-statistic.md)
- [Kolmogorov-Smirnov test](kolmogorov-smirnov-test.md)
- [Lilliefors test](lilliefors-test.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/28j/solution.md)
