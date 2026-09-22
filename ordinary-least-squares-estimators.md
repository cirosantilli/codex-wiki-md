# Ordinary least squares estimators

↑ **Parent:** [Ordinary least squares](ordinary-least-squares.md)

For a [linear regression](linear-regression-split.md) design matrix $X$ with [full column rank](full-column-rank.md), the [ordinary least squares](ordinary-least-squares.md) coefficient vector is $\widehat\beta=(X^TX)^{-1}X^TY$. In a [normal linear model](normal-linear-model.md) with error [covariance matrix](covariance-matrix.md) $\sigma^2I$, it is an [unbiased estimator](unbiased-estimator.md) with [covariance matrix](covariance-matrix.md) $\sigma^2(X^TX)^{-1}$. Replacing $\sigma^2$ by the residual variance estimate gives the reported coefficient [standard errors](standard-error.md).

In simple [linear regression](linear-regression-split.md) with a nonconstant predictor,

$$
\widehat\beta=\frac{\sum_i(x_i-\bar x)(Y_i-\bar Y)}
{\sum_i(x_i-\bar x)^2},
\qquad
\widehat\alpha=\bar Y-\widehat\beta\bar x.
$$

**Table of contents**

- [Residual sum of squares in simple linear regression](residual-sum-of-squares-in-simple-linear-regression.md)

## ↑ Ancestors (8)

1. [Ordinary least squares](ordinary-least-squares.md)
2. [Normal linear model](normal-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Centred simple linear regression](centred-simple-linear-regression.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/19c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/13j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/10j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/5j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/30j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/30j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4/17h/a/solution.md)
