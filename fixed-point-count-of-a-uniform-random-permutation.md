# Fixed point count of a uniform random permutation

↑ **Parent:** [Uniform random permutation](uniform-random-permutation.md)

For a [uniform random permutation](uniform-random-permutation.md) $\pi$ of $n\geq1$ objects, let $M_n$ count its [fixed points](fixed-point.md). Write $M_n=\sum_{i=1}^n\mathbf1_{\{\pi(i)=i\}}$. Each [indicator random variable](indicator-random-variable.md) has [expected value](expected-value.md) $1/n$, so [linearity of expectation](linearity-of-expectation.md) gives **$\mathbb E[M_n]=1$ for every $n\geq1$**. This average does not require [independence](independent-random-variables.md): for $n\geq2$, fixing two specified objects has [probability](probability.md) $1/[n(n-1)]$, greater than the product $1/n^2$ of their individual [probabilities](probability.md).

For four objects, exact enumeration gives counts $9,8,6,0,1$ for $0,1,2,3,4$ [fixed points](fixed-point.md) among the $24$ equally likely [permutations](permutation.md). Their weighted [arithmetic mean](arithmetic-mean.md) is $(0\cdot9+1\cdot8+2\cdot6+4\cdot1)/24=1$. Exactly three [fixed points](fixed-point.md) are impossible: the last object must then also be fixed.

<a id="image-the-fixed-point-count-of-a-uniform-random-permutation-averaged-over-all-24-permutations-of-four-objects"></a>
![](fixed-points-permutation-expectation.png)

**[Figure 24](#image-the-fixed-point-count-of-a-uniform-random-permutation-averaged-over-all-24-permutations-of-four-objects). The fixed point count of a uniform random permutation averaged over all $24$ permutations of four objects**. Each card lists $\pi(1),\pi(2),\pi(3),\pi(4)$. Green entries equal their positions and therefore mark [fixed points](fixed-point.md). The [probability mass function](probability-mass-function.md) on the right counts those cards; its [expected value](expected-value.md) is one.

Choose the $m$ fixed objects and derange the remaining $n-m$. Their count is $\binom nmD_{n-m}$ among $n!$ equally likely [permutations](permutation.md). The [inclusion-exclusion principle](inclusion-exclusion-principle.md) for $D_{n-m}$ proves the displayed law, valid for $0\le m\le n$ and zero otherwise. With $D_0=1$, it includes the all-fixed case and the impossibility of exactly $n-1$ fixed objects. For fixed $m$, the law tends to $e^{-1}/m!$, the [Poisson distribution](poisson-distribution.md) of mean one.

## ↑ Ancestors (6)

1. [Uniform random permutation](uniform-random-permutation.md)
2. [Permutation](permutation.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Fixed point count of a uniform random permutation](fixed-point-count-of-a-uniform-random-permutation.md)
- [Indicator random variable](indicator-random-variable.md)
- [Linearity of expectation](linearity-of-expectation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/9f/solution.md)
