# Prediction interval in a normal linear model

↑ **Parent:** [Prediction interval](prediction-interval.md)

For the full-rank [normal linear model](normal-linear-model.md) $Y=X\beta+\varepsilon$ and an independent future response $Y^*=x^{*T}\beta+\varepsilon^*$, put

$$
s^2=\frac{\operatorname{RSS}}{n-p},
\qquad
h^*=x^{*T}(X^TX)^{-1}x^*.
$$

Then an exact $(1-\alpha)$ prediction interval is

$$
x^{*T}\widehat\beta
\mathbin\pm t_{n-p,1-\alpha/2}s\sqrt{1+h^*}.
$$

The additional one inside the square root is the future observation's irreducible error variance; a confidence interval for its mean omits it.

**Table of contents**

- [Zero-residual degeneracy of regression prediction](zero-residual-degeneracy-of-regression-prediction.md)

## ↑ Ancestors (6)

1. [Prediction interval](prediction-interval.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/5i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/5j/solution.md)
