# Best linear unbiased prediction

↑ **Parent:** [Gaussian linear mixed model](gaussian-linear-mixed-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Best_linear_unbiased_prediction)

With known covariance parameters, best linear unbiased prediction minimizes prediction-error [variance](variance-split.md) over linear predictors that are unbiased over both observation errors and [random effects](random-effect.md), for every fixed-effect value. In a [Gaussian linear mixed model](gaussian-linear-mixed-model.md), the random-effect predictor is $DZ^TV^{-1}(Y-X\widehat\beta_{\mathrm{GLS}})$, where [generalized least squares](generalized-least-squares.md) estimates the fixed effects. Plugging in covariance estimates gives an empirical predictor; its uncertainty must also account for estimating those covariance parameters. It differs from a [best linear unbiased estimator](best-linear-unbiased-estimator.md) of an unknown fixed coefficient.

## ↑ Ancestors (9)

1. [Gaussian linear mixed model](gaussian-linear-mixed-model.md)
2. [Generalized linear mixed model](generalized-linear-mixed-model.md)
3. [Generalized linear model](generalized-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
