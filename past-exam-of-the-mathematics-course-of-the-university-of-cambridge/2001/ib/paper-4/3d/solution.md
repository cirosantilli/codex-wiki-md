<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

Assume $S_{xx}=\sum_i x_i^2>0$, so the slope in this [linear regression through the origin](../../../../../linear-regression-through-the-origin.md) is identifiable. Expanding the residual sum of squares gives

$$
\sum_i(Y_i-bx_i)^2=\sum_iY_i^2-2b\sum_i x_iY_i+b^2S_{xx}.
$$

Differentiation gives the unique [least-squares estimator](../../../../../ordinary-least-squares-estimators.md) and its [normal distribution](../../../../../normal-distribution.md):

$$
\boxed{\widehat\beta=\frac{\sum_i x_iY_i}{S_{xx}},\qquad
\widehat\beta\sim N\left(\beta,\frac{\sigma^2}{S_{xx}}\right).}
$$

For $n\ge2$, estimate the unknown variance by

$$
s^2=\frac1{n-1}\sum_i(Y_i-\widehat\beta x_i)^2.
$$

The fitted component and orthogonal residual of the [Gaussian vector](../../../../../gaussian-random-vector.md) are independent, and $(n-1)s^2/\sigma^2$ has the [chi-squared distribution](../../../../../chi-squared-distribution.md) with $n-1$ degrees of freedom. Under the null hypothesis,

$$
T=\frac{(\widehat\beta-\beta_0)\sqrt{S_{xx}}}{s}\sim t_{n-1}.
$$

The [Student t test for regression through the origin](../../../../../student-t-test-for-regression-through-the-origin.md) rejects at significance level $\alpha$ when **$|T|>t_{n-1,1-\alpha/2}$**, where the subscript denotes the corresponding quantile of [Student's t-distribution](../../../../../student-s-t-distribution.md). If all $x_i=0$, the data contain no information about $\beta$; if $n=1$, no residual degree of freedom is available for this unknown-variance test.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
