# Gaussian posterior in the zero-noise limit

↑ **Parent:** [Gaussian conjugacy for a normal linear model](gaussian-conjugacy-for-a-normal-linear-model.md)

For $m=Au+\eta$, with independent $u\sim\mathcal N(0,I_d)$ and $\eta\sim\mathcal N(0,\delta^2I_k)$, the [multivariate normal distribution](multivariate-normal-distribution.md) of the [Bayesian posterior](bayesian-posterior.md) has [posterior mean](posterior-mean.md) $b_\delta=(A^TA+\delta^2I_d)^{-1}A^Tm$ and [covariance matrix](covariance-matrix.md) $C_\delta=\delta^2(A^TA+\delta^2I_d)^{-1}$. The [singular value decomposition](singular-value-decomposition.md) shows that the variance on a right singular vector of nonzero [singular value](singular-value.md) $s$ is $\delta^2/(s^2+\delta^2)$, while the variance along the [null space](kernel-of-a-linear-map.md) is one. Thus, for fixed data, the mean tends to the [minimum-norm least-squares solution](minimum-norm-least-squares-solution.md) and the covariance tends to the [orthogonal projection](orthogonal-projection.md) onto the [null space](kernel-of-a-linear-map.md). Unobserved components retain their [prior distribution](prior-probability.md) even as the noise vanishes.

## ↑ Ancestors (8)

1. [Gaussian conjugacy for a normal linear model](gaussian-conjugacy-for-a-normal-linear-model.md)
2. [Normal linear model](normal-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/1/b/solution.md)
