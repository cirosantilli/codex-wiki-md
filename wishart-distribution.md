# Wishart distribution

↑ **Parent:** [Random matrix](random-matrix.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wishart_distribution)

For integer $\nu$, the sum $\sum_{j=1}^{\nu}X_jX_j^T$ of independent $N_p(0,V)$ vectors has a Wishart distribution. Its positive-definite density extends to real $\nu>p-1$ and is proportional to $|W|^{(\nu-p-1)/2}\exp[-\operatorname{tr}(V^{-1}W)/2]$. It is a [conjugate prior](conjugate-prior.md) for the [precision matrix](precision-matrix.md) of a [multivariate normal distribution](multivariate-normal-distribution.md). Its mean is $\nu V$.

The [WinBUGS](winbugs.md) declaration `dwish(R, nu)` uses $R=V^{-1}$; the density convention is documented in [the NIMBLE BUGS-language manual](https://r-nimble.org/manual/cha-writing-models.html). For $\nu=p=3$ it is proper, while the expected inverse matrix does not exist: that expectation requires $\nu>p+1$. Specifying a Wishart prior on precision is therefore a substantive covariance assumption.

**Table of contents**

- [Inverse-Wishart distribution](inverse-wishart-distribution.md)

## ↑ Ancestors (6)

1. [Random matrix](random-matrix.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Hotelling's T-squared statistic](hotelling-s-t-squared-statistic.md)
- [Inverse-Wishart distribution](inverse-wishart-distribution.md)
- [Multivariate analysis of variance](multivariate-analysis-of-variance.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/4/d/solution.md)
