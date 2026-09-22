# Training error

↑ **Parent:** [Statistical learning](statistical-learning-split.md)

Training error is the average [loss function](loss-function.md) evaluated on the observations used to fit the prediction rule. It is the [empirical risk](empirical-risk.md) of the fitted rule on its own [training data](training-data.md). With [squared-error loss](squared-error-loss.md), it is the average squared [regression residual](regression-residual.md), measuring fit to observed responses rather than performance on fresh responses. Flexible fitting usually makes it optimistically biased for [prediction error](prediction-error.md), as quantified by [prediction optimism](prediction-optimism.md).

For a reproducible [polynomial regression](polynomial-regression.md) example, take $x_i=-1+2i/11$, $i=0,\ldots,11$, and the known noiseless target $f(x)=1+x/2+2x^2$. Construct responses $y_i=f(x_i)+e_i$ with fixed disturbances

$$
(e_i)=(0.12,-0.17,0.10,0.18,-0.13,0.08,-0.16,0.11,-0.08,0.15,-0.12,0.06).
$$

[Ordinary least squares](ordinary-least-squares.md) over [polynomials](polynomial-split.md) of [polynomial degree](degree-of-a-polynomial.md) at most 1, 2, and 7 gives [training errors](training-error.md) $0.518937$, $0.015784$, and $0.009257$. The monotone improvement follows because these candidate families are nested: every smaller-degree fit remains available in the larger family. This argument concerns minimum [training error](training-error.md), not [generalization](generalization-in-statistical-learning.md), and assumes the fitting [mathematical optimization](mathematical-optimization-split.md) is solved. Degrees 2 and 7 fitted instead to the exact noiseless responses $f(x_i)$ have mathematically zero [training error](training-error.md); the script obtains approximately $5.31\times10^{-31}$ and $7.82\times10^{-31}$ from rounding. Extra flexibility alone does not force [overfitting](overfitting.md).

**Table of contents**

- [Prediction optimism](prediction-optimism.md)
  - [Covariance formula for prediction optimism](covariance-formula-for-prediction-optimism.md)

## ↑ Ancestors (7)

1. [Statistical learning](statistical-learning-split.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Cross-validation](cross-validation.md)
- [Generalization in statistical learning](generalization-in-statistical-learning.md)
- [Misclassification rate](misclassification-rate.md)
- [Overfitting](overfitting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-218/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-218/3/a/solution.md)
- [Prediction optimism](prediction-optimism.md)
- [Residual sum of squares](residual-sum-of-squares.md)
- [Statistical learning](statistical-learning-split.md)
- [Training error](training-error.md)
