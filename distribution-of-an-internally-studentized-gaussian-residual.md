# Distribution of an internally studentized Gaussian residual

↑ **Parent:** [Standardized regression residual](standardized-regression-residual.md)

In a [normal linear model](normal-linear-model.md) with residual [degrees of freedom](degree-of-freedom.md) $\nu\geq2$, an [internally studentized residual](standardized-regression-residual.md) satisfies $|\eta_i|\leq\sqrt\nu$ and $\eta_i^2/\nu\sim\operatorname{Beta}(1/2,(\nu-1)/2)$, provided its [leverage](regression-leverage.md) is less than one. Choose an [orthonormal basis](orthonormal-basis.md) of the residual space with its first direction proportional to the projection of the $i$th coordinate vector. The [Gaussian](normal-distribution.md) coordinates in this basis are independent standard [normal random variables](gaussian-random-variable.md) $Z_1,\ldots,Z_\nu$, and $\eta_i=\sqrt\nu Z_1/(\sum_jZ_j^2)^{1/2}$. The [Beta distribution](beta-distribution.md) follows from the independent [chi-squared distributions](chi-squared-distribution.md) of $Z_1^2$ and $\sum_{j=2}^\nu Z_j^2$. The bounded residual is not exactly distributed according to [Student's t-distribution](student-s-t-distribution.md); it approaches the standard [normal distribution](normal-distribution.md) as $\nu\to\infty$.

## ↑ Ancestors (6)

1. [Standardized regression residual](standardized-regression-residual.md)
2. [Regression residual](regression-residual.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/5j/solution.md)
