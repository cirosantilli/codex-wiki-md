# Multivariate analysis of variance

↑ **Parent:** [Analysis of variance](analysis-of-variance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multivariate_analysis_of_variance)

Multivariate analysis of variance compares mean vectors of several groups while accounting for correlations between their response variables. In the one-way normal model, independent observations $Y_{ri}\sim N_p(\mu_r,\Sigma)$ share a positive-definite [covariance matrix](covariance-matrix.md). Put $E=\sum_{r,i}(Y_{ri}-\bar Y_r)(Y_{ri}-\bar Y_r)^T$ and $H=\sum_rn_r(\bar Y_r-\bar Y)(\bar Y_r-\bar Y)^T$. Under equal means, these matrices have independent [Wishart distributions](wishart-distribution.md) with degrees of freedom $N-g$ and $g-1$, respectively. This follows by separating the Gaussian data into orthogonal within-group and between-group projections. The [Wilks lambda statistic](wilks-lambda-statistic.md) tests equality of the means using both matrices, rather than independently testing each coordinate.

**Table of contents**

- [Within-group and between-group scatter decomposition](within-group-and-between-group-scatter-decomposition.md)
- [Wilks lambda statistic](wilks-lambda-statistic.md)

## ↑ Ancestors (9)

1. [Analysis of variance](analysis-of-variance.md)
2. [Linear regression](linear-regression-split.md)
3. [Normal linear model](normal-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46/4/i/solution.md)
