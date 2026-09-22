# Cameron-Martin theorem for a Gaussian measure

↑ **Parent:** [Gaussian measure](gaussian-measure.md)

For $\mu=\mathcal N(0,\Sigma)$ with injective [covariance operator of a Gaussian measure](covariance-operator-of-a-gaussian-measure.md), its translated law $\mu_h=\mathcal N(h,\Sigma)$ is an [equivalent probability measure](equivalent-probability-measure.md) to $\mu$ if and only if $h\in E_\mu$, the [Cameron-Martin space of a Gaussian measure](cameron-martin-space-of-a-gaussian-measure.md). For such $h$,

$$
\frac{d\mu_h}{d\mu}(x)=\exp\left(\ell_h(x)-\tfrac12\|h\|_{E_\mu}^2\right),\qquad
\ell_h(x)=\sum_j\frac{h_jx_j}{\lambda_j}.
$$

The series has [mean-square convergence](convergence-in-l2.md) and converges [almost surely](almost-sure-convergence.md) under $\mu$, with [normal distribution](normal-distribution.md) $\mathcal N(0,\|h\|_{E_\mu}^2)$. Its exponential density has [expected value](expected-value.md) one by the [moment-generating function of a normal distribution](moment-generating-function-of-a-normal-distribution.md). Finite-dimensional projections give the formula by ratios of [multivariate normal densities](multivariate-normal-density.md); convergence of these likelihood ratios gives the infinite-dimensional result. The expression $\langle h,x\rangle_{E_\mu}$ is only formal when the sample is outside $E_\mu$. For $h\notin E_\mu$, translation gives [mutually singular measures](mutually-singular-measures.md).

**Table of contents**

- [Symmetric Gaussian translation lower bound](symmetric-gaussian-translation-lower-bound.md)

## ↑ Ancestors (8)

1. [Gaussian measure](gaussian-measure.md)
2. [Gaussian process](gaussian-process.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Cameron-Martin space of a Gaussian measure](cameron-martin-space-of-a-gaussian-measure.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/3/b/solution.md)
- [Symmetric Gaussian translation lower bound](symmetric-gaussian-translation-lower-bound.md)
- [White-noise likelihood for a square-integrable shift](white-noise-likelihood-for-a-square-integrable-shift.md)
