# Adjusted coefficient of determination

↑ **Parent:** [Coefficient of determination](coefficient-of-determination.md)

In a [normal linear model](normal-linear-model.md) with an intercept, $n$ observations and $p$ independent mean coefficients, adjusted $R^2$ is

$$
\overline R^2=1-\frac{\operatorname{RSS}/(n-p)}{\operatorname{SST}/(n-1)}.
$$

It compares the residual [variance](variance-split.md) estimate with the unmodelled [sample variance](sample-variance.md), adjusting the raw [coefficient of determination](coefficient-of-determination.md) for fitted dimension. It can be negative and is not guaranteed to increase when another regressor is added. In penalized regression a related convention uses the fit's [effective degrees of freedom](effective-degrees-of-freedom.md) instead of $p$; the precise smoothing-software [variance](variance-split.md) convention should be specified.

## ↑ Ancestors (9)

1. [Coefficient of determination](coefficient-of-determination.md)
2. [Linear regression](linear-regression-split.md)
3. [Normal linear model](normal-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/5/e/solution.md)
