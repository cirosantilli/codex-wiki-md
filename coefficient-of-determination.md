# Coefficient of determination

↑ **Parent:** [Linear regression](linear-regression-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coefficient_of_determination)

In an [ordinary least squares](ordinary-least-squares.md) regression with an intercept and a nonconstant response, $R^2=1-\mathrm{RSS}/\sum_i(Y_i-\overline Y)^2$. It measures the fitted proportion of sample variation relative to an intercept-only baseline. It increases when regressors are added, even if those regressors are unhelpful for prediction. A high value does not establish the assumptions of a [normal linear model](normal-linear-model-split.md) or rule out a systematic [regression residual](regression-residual.md) pattern.

For the five-point example in [linear regression](linear-regression-split.md), the total centered [sum of squares](sum-of-squares.md) is $10.8$ and the [residual sum of squares](residual-sum-of-squares.md) is $0.8$, so $R^2=25/27\approx0.926$. This summarizes the fitted reduction in squared error. It does not record the order or shape of the [regression residuals](regression-residual.md), which are worth examining in a [residual-versus-fitted plot](residual-versus-fitted-plot.md).

Here is a fully constructed illustration. Use $x=(-2,-1,0,1,2)$ and the same fitted line $3+x$ for both datasets. Add respectively the residual vectors

$$
r_{\rm curve}=0.2(2,-1,-2,-1,2),\qquad
r_{\rm alt}=0.2\sqrt{\frac75}(1,-2,0,2,-1).
$$

Both sum to zero, both have zero [inner product](inner-product-split.md) with $x$, and both have squared [norm](norm.md) $0.56$. Their [ordinary least squares](ordinary-least-squares.md) fit is therefore exactly the same line, with the same $R^2=10/(10+0.56)=125/132\approx0.947$. But the first residual is $0.2(x^2-2)$, a systematic quadratic shape, while the second changes direction across the predictor values. These examples show directly which information the scalar $R^2$ discards; neither constructed pattern proves a random-error model.

<a id="image-two-constructed-datasets-share-a-fitted-line-and-r-squared-but-have-different-residual-shapes"></a>
![](regression-residual-patterns.png)

**[Figure 2](#image-two-constructed-datasets-share-a-fitted-line-and-r-squared-but-have-different-residual-shapes). Two constructed datasets share a fitted line and R squared but have different residual shapes**.

**Table of contents**

- [Adjusted coefficient of determination](adjusted-coefficient-of-determination.md)

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Adjusted coefficient of determination](adjusted-coefficient-of-determination.md)
- [Cox–Snell likelihood pseudo-R-squared](cox-snell-likelihood-pseudo-r-squared.md)
- [Multiple linear regression](multiple-linear-regression.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/1/b/solution.md)
- [Residual-versus-fitted plot](residual-versus-fitted-plot.md)
