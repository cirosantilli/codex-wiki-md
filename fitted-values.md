# Fitted values

↑ **Parent:** [Linear regression](linear-regression-split.md)

[Fitted values](fitted-values.md) are the predictions at the predictor values used to fit a [regression model](regression-model.md). In [linear regression](linear-regression-split.md) with an explicit [regression intercept](regression-intercept.md),

$$
\widehat Y=\widehat\alpha\mathbf1+X\widehat\beta,\qquad r=Y-\widehat Y.
$$

Here $X$ is the slope [design matrix](design-matrix.md), and $r$ is the [regression residual](regression-residual.md) vector. The [fitted values](fitted-values.md) estimate the [regression function](regression-function.md) at the observed predictors; they need not equal the observed responses, which may also contain random errors. Prediction at a new predictor [vector](vector.md) $x_*$ uses $\widehat\alpha+x_*^T\widehat\beta$ with the same centering and scaling used in fitting. A [prediction interval](prediction-interval.md) addresses uncertainty in a new response rather than just displaying this point prediction.

For the five constructed observations in [linear regression](linear-regression-split.md), [ordinary least squares](ordinary-least-squares.md) gives [fitted values](fitted-values.md) $(4/5,9/5,14/5,19/5,24/5)$. The [ridge regression](ridge-regression.md) fit at $\lambda=10$ instead gives $(9/5,23/10,14/5,33/10,19/5)$. Both fitted vectors have [sample mean](sample-mean.md) $14/5$ because the [regression intercept](regression-intercept.md) is unpenalized; their [regression residuals](regression-residual.md) differ and their [residual sums of squares](residual-sum-of-squares.md) are $4/5$ and $33/10$, respectively.

For [ordinary least squares](ordinary-least-squares.md), the [fitted values](fitted-values.md) are the [orthogonal projection](orthogonal-projection.md) of $Y$ onto the [column space](column-space.md) of the complete [design matrix](design-matrix.md), including its [regression intercept](regression-intercept.md) column. They remain unique even in [rank-deficient ordinary least squares](rank-deficient-ordinary-least-squares.md), although the [regression coefficients](regression-coefficient.md) can be nonunique. The [regression residuals](regression-residual.md) are then [orthogonal](orthogonal-vectors.md) to every column.[slides 6–10: fitted values, hat matrix, projection and orthogonal residuals](data-mining-36-462-and-36-662/regression-1-different-perspectives.md) With centered slopes, [ridge regression](ridge-regression.md) instead satisfies $X_c^Tr=\lambda\widehat\beta_\lambda$, so the [regression residuals](regression-residual.md) need not be [orthogonal](orthogonal-vectors.md) to the slope columns. Their sum is still zero because the [regression intercept](regression-intercept.md) remains free.

For fixed predictors and scales and a fixed positive penalty, [ridge regression](ridge-regression.md) gives a [linear smoother](linear-smoother.md),

$$
\widehat Y_\lambda=H_\lambda Y,\qquad H_\lambda=\frac{\mathbf1\mathbf1^T}{n}+X_c(X_c^TX_c+\lambda I_p)^{-1}X_c^T.
$$

For $\lambda>0$ with at least one nonzero slope direction, this [matrix](matrix.md) is not an [orthogonal projection matrix](orthogonal-projection-matrix.md): applying it twice shrinks that direction again. Its [effective degrees of freedom](effective-degrees-of-freedom.md) are $1+\sum_{j=1}^r d_j^2/(d_j^2+\lambda)$, where $d_j$ are the positive [singular values](singular-value.md) of $X_c$; the extra $1$ counts the free [regression intercept](regression-intercept.md). If the penalty is selected using $Y$, the resulting fitting rule need not be a [linear smoother](linear-smoother.md), since its chosen $H_\lambda$ also depends on $Y$.

**Table of contents**

- [Linear smoother](linear-smoother.md)
  - [Effective degrees of freedom](effective-degrees-of-freedom.md)

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Fitted-residual orthogonality](fitted-residual-orthogonality.md)
- [Fitted values](fitted-values.md)
- [Linear regression](linear-regression-split.md)
- [Normal equations for linear least squares](normal-equations-for-linear-least-squares.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-218/2/a/solution.md)
- [Residual curvature diagnostic](residual-curvature-diagnostic.md)
- [Residual sum of squares](residual-sum-of-squares.md)
- [Ridge regression](ridge-regression.md)
- [Scale-location plot](scale-location-plot.md)
