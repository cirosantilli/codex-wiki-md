<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [least-squares estimators](../../../../../../ordinary-least-squares-estimators.md) choose the intercept and slope to minimize the sum of squared [regression residuals](../../../../../../regression-residual.md):

$$
\boxed{(\widehat\alpha,\widehat\beta)\in
\operatorname*{arg\,min}_{a,b\in\mathbb R}\sum_{i=1}^n(Y_i-a-bx_i)^2.}
$$

After observation, replace $Y_i$ by $y_i$ to obtain the numerical [estimates](../../../../../../statistical-estimate.md). Their definition does not require a [normal distribution](../../../../../../normal-distribution.md) for the errors. A unique slope requires some variation in the fixed predictors; under $\sum_i x_i=0$, this is $S_{xx}=\sum_i x_i^2>0$, assumed below. If all $x_i=0$, the slope is unidentifiable.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
