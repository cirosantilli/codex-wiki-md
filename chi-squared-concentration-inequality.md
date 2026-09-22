# Chi-squared concentration inequality

↑ **Parent:** [Chi-squared distribution](chi-squared-distribution.md)

For $V\sim\chi_n^2$ and $x>0$, the upper tail is at most $e^{-x}$ above $n+2\sqrt{nx}+2x$, and the lower tail is at most $e^{-x}$ below $n-2\sqrt{nx}$. Indeed $\log\mathbb E e^{s(V-n)}=-ns-(n/2)\log(1-2s)\leq ns^2/(1-2s)$ for $0<s<1/2$. The [Chernoff bound](chernoff-bound.md) with $s=\sqrt{x/n}/(1+2\sqrt{x/n})$ proves the upper estimate. For the lower estimate, $\log\mathbb E e^{-s(V-n)}\leq ns^2$ for $s>0$, and optimization gives the result. The lower threshold can be negative; the [chi-squared Chernoff lower-tail bound](chi-squared-chernoff-lower-tail-bound.md) provides an always-positive alternative.

**Table of contents**

- [Chi-squared Chernoff lower-tail bound](chi-squared-chernoff-lower-tail-bound.md)

## ↑ Ancestors (7)

1. [Chi-squared distribution](chi-squared-distribution.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Chi-squared Chernoff lower-tail bound](chi-squared-chernoff-lower-tail-bound.md)
- [Gaussian Gram matrix concentration on a fixed subspace](gaussian-gram-matrix-concentration-on-a-fixed-subspace.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-30/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/2/c/solution.md)
- [Quadratic scan statistic](quadratic-scan-statistic.md)
