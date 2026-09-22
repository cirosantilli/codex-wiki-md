# Gaussian covariance diagonality likelihood-ratio test

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

For independent observations from a nonsingular [multivariate normal distribution](multivariate-normal-distribution.md) with unknown mean, let $S=n^{-1}\sum_i(y_i-\bar y)(y_i-\bar y)^T$. The unrestricted [maximum-likelihood estimator](maximum-likelihood-estimator.md) of covariance is $S$, while the diagonal restriction gives $D=\operatorname{diag}(S_{11},\ldots,S_{pp})$. The fitted trace terms both equal $p$, so twice the log-likelihood difference is $W=n\log(\det D/\det S)=-n\log\det R$, where $R$ is the [sample correlation matrix](sample-correlation-matrix.md). Under the diagonal null hypothesis and fixed dimension, the [Wilks theorem](wilks-theorem.md) gives $W\Rightarrow\chi^2_{p(p-1)/2}$.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30/1/ii/solution.md)
