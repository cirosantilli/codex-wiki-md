# Residual sum of squares in simple linear regression

↑ **Parent:** [Ordinary least squares estimators](ordinary-least-squares-estimators.md)

For a nonconstant predictor, put

$$
S_{xx}=\sum_i(x_i-\bar x)^2,
\quad
S_{xy}=\sum_i(x_i-\bar x)(y_i-\bar y),
\quad
S_{yy}=\sum_i(y_i-\bar y)^2.
$$

The minimized residual sum of squares is

$$
\operatorname{RSS}=S_{yy}-\frac{S_{xy}^2}{S_{xx}}.
$$

Each centered sum can be recovered in constant time from the five raw sums $\sum x_i$, $\sum y_i$, $\sum x_i^2$, $\sum x_iy_i$, and $\sum y_i^2$.

## ↑ Ancestors (9)

1. [Ordinary least squares estimators](ordinary-least-squares-estimators.md)
2. [Ordinary least squares](ordinary-least-squares.md)
3. [Normal linear model](normal-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/30j/d/solution.md)
