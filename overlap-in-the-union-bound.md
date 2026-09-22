# Overlap in the union bound

↑ **Parent:** [Boole's inequality](boole-s-inequality.md)

For a finite family, the [random variable](random-variable-split.md) $N=\sum_i\mathbf1_{A_i}$ counts the [events](event.md) that occur. [Linearity of expectation](linearity-of-expectation.md) gives $\mathbb E N=\sum_i\mathbb P(A_i)$, while $\mathbb P(N\geq1)$ is the exact [union](set-union.md) [probability](probability.md). Their difference is

$$
\sum_i\mathbb P(A_i)-\mathbb P\left(\bigcup_i A_i\right)=\mathbb E\left[N-\mathbf1_{\{N\geq1\}}\right].
$$

An outcome in exactly $k\geq1$ [events](event.md) contributes $k-1$ extra counts, weighted by its [probability](probability.md). This nonnegative difference vanishes exactly in [equality in Boole's inequality](equality-in-boole-s-inequality.md). For two [events](event.md) it is $\mathbb P(A\cap B)$, as the [inclusion-exclusion principle for probabilities](inclusion-exclusion-principle-for-probabilities.md) shows. For more [events](event.md), the [Bonferroni inequalities](bonferroni-inequalities.md) use pairwise and higher [intersection](set-intersection.md) information to bound the exact [union](set-union.md) [probability](probability.md); blindly subtracting pairwise [intersections](set-intersection.md) from the sum gives a lower bound, rather than a corrected upper bound.

Severe overlap can make the [union bound](boole-s-inequality.md) arbitrarily pessimistic. Let all $m$ [events](event.md) be the same [event](event.md) $A$ with [probability](probability.md) $1/m$, where $m\geq1$ is an [integer](integer-split.md). A concrete model is the [discrete uniform distribution](discrete-uniform-distribution.md) on $\{1,\ldots,m\}$ with $A=\{1\}$. The exact [union](set-union.md) [probability](probability.md) is $1/m$, whereas the sum and capped bound are both one. The ratio is $m$: adding more names for the same [event](event.md) does not create more ways to fail. The identity above describes the gap in the uncapped sum; capping at one can reduce that gap.

## ↑ Ancestors (7)

1. [Boole's inequality](boole-s-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Boole's inequality](boole-s-inequality.md)
