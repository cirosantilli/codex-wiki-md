# Student t test for regression through the origin

↑ **Parent:** [Linear regression through the origin](linear-regression-through-the-origin.md)

For independent $Y_i\sim N(\beta x_i,\sigma^2)$ with $n\geq2$ and $\sum x_i^2>0$, the [least-squares estimator](ordinary-least-squares-estimators.md) is $\widehat\beta=\sum x_iY_i/\sum x_i^2$. The projection of the isotropic [Gaussian vector](gaussian-random-vector.md) onto the design direction is independent of its orthogonal residual; hence $\widehat\beta\sqrt{\sum x_i^2}/\sigma$ is standard normal under $\beta=0$ and $\mathrm{SSE}/\sigma^2$ is independent chi-squared with $n-1$ degrees of freedom. The displayed statistic therefore has [Student's t-distribution](student-s-t-distribution.md) with $n-1$ degrees of freedom. A two-sided test rejects at the corresponding upper/lower quantiles. The zero design has no information about the slope; with one observation there is no residual variance degree of freedom.

## ↑ Ancestors (9)

1. [Linear regression through the origin](linear-regression-through-the-origin.md)
2. [Ordinary least squares](ordinary-least-squares.md)
3. [Normal linear model](normal-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/3d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/9h/solution.md)
