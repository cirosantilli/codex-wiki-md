# Covariance and bias of a ridge regression estimator

↑ **Parent:** [Ridge regression](ridge-regression.md)

For a fixed centered [design matrix](design-matrix.md) $X$, independent errors of [variance](variance-split.md) $\sigma^2$, and objective $\lVert Y-X\beta\rVert^2+a\lVert\beta\rVert^2$, put $G=X^TX$ and $M=G+aI$. The [ridge regression](ridge-regression.md) estimator has

$$
\operatorname{Cov}(\widehat\beta)=\sigma^2M^{-1}GM^{-1},\qquad \mathbb E\widehat\beta-\beta=-aM^{-1}\beta.
$$

Thus its standard error alone does not justify centering a [confidence interval](confidence-interval.md) for $\beta$ at the biased estimator. A penalty chosen from the responses also changes its [sampling distribution](sampling-distribution.md).

## ↑ Ancestors (9)

1. [Ridge regression](ridge-regression.md)
2. [Linear regression](linear-regression-split.md)
3. [Normal linear model](normal-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/6/e/solution.md)
