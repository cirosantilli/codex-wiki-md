<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

Put $z_i=x_i-\bar x$, so $\sum z_i=0$. The [ordinary least squares](../../../../../ordinary-least-squares.md) criterion is $S(\alpha,\beta)=\sum_i(Y_i-\alpha-\beta z_i)^2$. Setting both partial derivatives to zero gives $\sum_i(Y_i-\alpha-\beta z_i)=0$ and $\sum_i z_i(Y_i-\alpha-\beta z_i)=0$. Therefore, provided $S_{xx}=\sum z_i^2>0$, the [centred simple linear regression](../../../../../centred-simple-linear-regression.md) estimators are

$$
\boxed{\widehat\alpha=\bar Y,\qquad\widehat\beta=\frac{\sum_i(x_i-\bar x)Y_i}{\sum_i(x_i-\bar x)^2}.}
$$

The Hessian of $S$ is $2\operatorname{diag}(n,S_{xx})$, which is positive definite, so this stationary point is the unique minimum. From the mean-zero errors, both estimators are unbiased; independence and common error [variance](../../../../../variance-split.md) give $\operatorname{Var}\widehat\alpha=\sigma^2/n$, $\operatorname{Var}\widehat\beta=\sigma^2/S_{xx}$, and zero [covariance](../../../../../covariance.md). Normality is not needed for this derivation. If all $x_i$ coincide, the slope is not identifiable and only the intercept is determined.

Using the PDF data gives $\bar x=6.2$, $\bar y=42.4$, $S_{xx}=86.8$ and $S_{xy}=-257.4$. In particular, the fourth cost is 37 in the PDF; the TeX's 75 is a transcription error and would contradict the supplied covariance sum. The fitted [simple linear regression](../../../../../simple-linear-regression.md) is

$$
\boxed{\widehat y=42.4-\frac{1287}{434}(x-6.2).}
$$

Here the centred intercept estimate is 42.4; an intercept at $x=0$ would instead be $\widehat\alpha-\widehat\beta\bar x$. For eight units the predicted unit cost is

$$
\boxed{\widehat y(8)=42.4-\frac{1287}{434}(1.8)\approx37.06\ \text{pounds}.}
$$

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
