# Residual sum of squares

↑ **Parent:** [Linear regression](linear-regression-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Residual_sum_of_squares)

The [residual sum of squares](residual-sum-of-squares.md) measures how far the observed responses lie from their [fitted values](fitted-values.md). If $r_i=Y_i-\widehat Y_i$ is the $i$th [regression residual](regression-residual.md), then

$$
\operatorname{RSS}=\sum_{i=1}^n(Y_i-\widehat Y_i)^2=\|Y-\widehat Y\|_2^2.
$$

It is the [squared Euclidean norm](squared-euclidean-norm.md) of the [regression residual](regression-residual.md) vector. Squaring prevents positive and negative deviations from cancelling and gives large deviations more weight. In the constructed five-point example in [linear regression](linear-regression-split.md), the [regression residuals](regression-residual.md) are $(1/5,1/5,-4/5,1/5,1/5)$, so the [residual sum of squares](residual-sum-of-squares.md) is $4/5$.

[Ordinary least squares](ordinary-least-squares.md) minimizes the [residual sum of squares](residual-sum-of-squares.md) over the chosen [linear regression](linear-regression-split.md) family; [ridge regression](ridge-regression.md) minimizes the [residual sum of squares](residual-sum-of-squares.md) plus a penalty. Consequently the [ridge regression](ridge-regression.md) fit can have a larger [residual sum of squares](residual-sum-of-squares.md) than the [ordinary least squares](ordinary-least-squares.md) fit on exactly the same [design matrix](design-matrix.md). For the one-predictor construction in [ridge regression](ridge-regression.md), the [residual sum of squares](residual-sum-of-squares.md) rises from $4/5$ to $33/10$ when the penalty changes from $0$ to $10$; that increase is the cost of shrinking the fitted slope.

Dividing the [residual sum of squares](residual-sum-of-squares.md) by $n$ gives the [training error](training-error.md) for [squared-error loss](squared-error-loss.md), not an estimate based on fresh responses. Its units are squared response units, and it adds across observations, so raw totals need not be comparable across different response scales or sample sizes. Comparing fits to the same responses is useful, but choosing a [ridge regression](ridge-regression.md) penalty by minimum training [residual sum of squares](residual-sum-of-squares.md) favors the unpenalized fit. Assess [prediction error](prediction-error.md) using a [validation set](validation-set.md) or [cross-validation](cross-validation.md) instead.[slides 6–8 and 11–14: fresh-response error, training error and held-out scoring](data-mining-36-462-and-36-662/model-selection-and-validation-1-cross-validation.md)

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (46)

- [Coefficient of determination](coefficient-of-determination.md)
- [Equal-cell replication variance formula](equal-cell-replication-variance-formula.md)
- [Extra sum of squares](extra-sum-of-squares.md)
- [Factor-level pooling test](factor-level-pooling-test.md)
- [Franck-Hertz spacing fit and contact offset](franck-hertz-spacing-fit-and-contact-offset.md)
- [Linear regression](linear-regression-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/19c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/19c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-44/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/19h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-218/5/c/solution.md)
- [Pure error](pure-error.md)
- [Residual estimate of Gaussian noise variance](residual-estimate-of-gaussian-noise-variance.md)
- [Residual sum of squares](residual-sum-of-squares.md)
- [Ridge regression](ridge-regression.md)
- [Saturation of an unreplicated two-factor regression](saturation-of-an-unreplicated-two-factor-regression.md)
- [Scaled deviance](scaled-deviance.md)
- [Sum of squares](sum-of-squares.md)
- [Unknown-variance risk estimation in a saturated Gaussian model](unknown-variance-risk-estimation-in-a-saturated-gaussian-model.md)
