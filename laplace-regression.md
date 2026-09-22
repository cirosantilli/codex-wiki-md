# Laplace regression

↑ **Parent:** [Laplace distribution](laplace-distribution.md)

For [linear regression](linear-regression-split.md) with fixed predictor vectors $X_i$, assume conditionally [independent](independent-random-variables.md) responses with a common scale $b>0$:

$$
Y_i\mid X_i\sim\operatorname{Laplace}(X_i^T\beta,b).
$$

Each conditional [median](median.md) and [mean](expected-value-split.md) is $X_i^T\beta$. The [log-likelihood function](log-likelihood.md) is $-n\log(2b)-S(\beta)/b$, so [maximum likelihood estimation](maximum-likelihood-estimation-split.md) minimizes the sum of absolute [regression residuals](regression-residual.md):

$$
S(\beta)=\sum_i|Y_i-X_i^T\beta|.
$$

This is [least absolute deviations](laplace-regression.md). With only an intercept, it reduces to the [Laplace location and scale maximum likelihood](laplace-location-and-scale-maximum-likelihood.md) problem, so a [sample median](sample-median.md) is a fitted intercept. Provided the minimum $S(\widehat\beta)>0$, the scale estimate is $\widehat b=S(\widehat\beta)/n$; the conditional [standard deviation](standard-deviation.md) is $\sqrt2\,b$. If the scale is denoted $\sigma$ instead of $b$, the conditional [standard deviation](standard-deviation.md) is $\sqrt2\,\sigma$.

Minimizing a sum of [absolute losses](absolute-error-loss.md) does not automatically give a unique coefficient vector. Even an intercept-only fit to an even [sample size](sample-size.md) can have an interval of solutions, and redundant predictor columns can introduce further nonuniqueness. If a fit makes every [regression residual](regression-residual.md) zero, the joint [likelihood function](likelihood-function.md) is unbounded as $b\downarrow0$, so there is no finite joint [maximum-likelihood estimate](maximum-likelihood-estimator.md) with positive scale.

The linear growth of [absolute loss](absolute-error-loss.md) limits sensitivity to an extreme response at fixed predictors compared with [squared-error loss](squared-error-loss.md). It does not protect against every [outlier](outlier.md): an extreme predictor can have large [regression leverage](regression-leverage.md). The numerical example above changes a response in an intercept-only problem, and makes no general claim of immunity to such predictor changes.

## ↑ Ancestors (8)

1. [Laplace distribution](laplace-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
