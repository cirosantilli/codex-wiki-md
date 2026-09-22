# Gaussian diagonal-covariance likelihood-ratio test

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

For independent [multivariate normal](multivariate-normal-distribution.md) observations with unrestricted [mean](expected-value.md) and positive-definite [sample covariance matrix](sample-covariance-matrix.md) $S=n^{-1}\sum_i(x_i-\bar x)(x_i-\bar x)^T$, the unrestricted [maximum-likelihood estimates](maximum-likelihood-estimator.md) are $\bar x,S$. Requiring a diagonal population [covariance matrix](covariance-matrix.md) gives the same mean and covariance estimate $D=\operatorname{diag}(S_{11},\ldots,S_{pp})$. Both fitted quadratic terms equal $np$, so their likelihood quotient is $(|S|/|D|)^{n/2}=|R|^{n/2}$, where $R=D^{-1/2}SD^{-1/2}$ is the [sample correlation matrix](sample-correlation-matrix.md). Small determinants give evidence against diagonality. For two variables this is a two-sided test of their [sample correlation](sample-correlation-coefficient.md).

## ↑ Ancestors (8)

1. [Likelihood-ratio test](likelihood-ratio-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42/1/iii/solution.md)
