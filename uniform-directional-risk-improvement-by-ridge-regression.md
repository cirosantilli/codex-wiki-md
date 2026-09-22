# Uniform directional risk improvement by ridge regression

↑ **Parent:** [Ridge regression](ridge-regression.md)

For a full-rank centred design, unscaled [ridge regression](ridge-regression.md) and zero-mean errors with covariance $\sigma^2I$, put $S=X^{\mathsf T}X$ and $A=(S+\lambda I)^{-1}$. The ordinary-least-squares risk matrix minus the ridge risk matrix is $\lambda A(2\sigma^2I+\lambda\sigma^2S^{-1}-\lambda\beta^0\beta^{0\mathsf T})A$. It is positive definite whenever $\lambda\|\beta^0\|_2^2<2\sigma^2$, including every positive $\lambda$ when $\beta^0=0$. Thus one signal-dependent small penalty improves every nonzero-direction [mean squared error](mean-squared-error.md).

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
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32/2/solution.md)
