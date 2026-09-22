# Simple linear regression

↑ **Parent:** [Linear regression](linear-regression-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_linear_regression)

Simple linear regression uses one predictor and an [intercept](regression-intercept.md), $Y_i=\alpha+\beta x_i+\varepsilon_i$, with $\mathbb E(\varepsilon_i\mid x_i)=0$. The [regression coefficients](regression-coefficient.md) describe a straight conditional-mean line: $\alpha$ is its value at zero and $\beta$ its rate of change per unit of the predictor. When zero is outside the observed range, [predictor centering](predictor-centering.md) can make the [intercept](regression-intercept.md) refer to a more representative predictor value.

For fixed predictors and uncorrelated mean-zero errors of common [variance](variance-split.md) $\sigma^2$, with $S_{xx}>0$,

$$
\operatorname{Var}(\widehat\beta)=\frac{\sigma^2}{S_{xx}},\qquad
\operatorname{Var}(\widehat\alpha)=\sigma^2\left(\frac1n+\frac{\bar x^2}{S_{xx}}\right).
$$

A larger predictor spread improves slope precision under this model. In the worked example $S_{xx}=10$ and $n=5$; the estimated error [variance](variance-split.md) is $s^2=\operatorname{RSS}/(n-2)=0.8/3$. A [normal linear model](normal-linear-model.md) gives the slope pivot $(\widehat\beta-\beta)/(s/\sqrt{S_{xx}})$ a [Student t-distribution](student-s-t-distribution.md) with $n-2$ [degrees of freedom](degree-of-freedom.md). The distinction between a fitted line and a reliable uncertainty statement is precisely the role of the error assumptions.

**Table of contents**

- [Centred simple linear regression](centred-simple-linear-regression.md)

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Centred simple linear regression](centred-simple-linear-regression.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/3h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/19h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-218/5/a/solution.md)
- [Predictor centering](predictor-centering.md)
