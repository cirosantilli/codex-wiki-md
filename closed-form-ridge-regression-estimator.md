# Closed-form ridge regression estimator

↑ **Parent:** [Ridge regression](ridge-regression.md)

For $\lambda>0$, the [ridge regression](ridge-regression.md) objective $\lVert Y-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_2^2$ has [gradient](gradient.md) $2(X^TX+\lambda I)\beta-2X^TY$. The matrix $X^TX+\lambda I$ is [positive definite](positive-definite-matrix.md), so the unique minimizer is $\widehat\beta_\lambda=(X^TX+\lambda I)^{-1}X^TY$.

**Table of contents**

- [Vanishing-penalty ridge limit](vanishing-penalty-ridge-limit.md)
- [Primal-dual identity for ridge regression](primal-dual-identity-for-ridge-regression.md)
- [Principal-component shrinkage by ridge regression](principal-component-shrinkage-by-ridge-regression.md)

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

## ← Incoming links (7)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/29j/b/solution.md)
