<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Write $S_{xx}=\sum_i x_i^2$. When $S_{xx}>0$, minimizing $\sum_i(Y_i-bx_i)^2$ gives the strictly convex quadratic normal equation $bS_{xx}=\sum_ix_iY_i$. The [least-squares estimator](../../../../../ordinary-least-squares-estimators.md) is therefore

$$
\boxed{\widehat\beta=\frac{\sum_i x_iY_i}{\sum_i x_i^2}.}
$$

This is [linear regression through the origin](../../../../../linear-regression-through-the-origin.md), with no fitted intercept. For $n\geq2$, let $\mathrm{SSE}=\sum_i(Y_i-\widehat\beta x_i)^2$ and $s^2=\mathrm{SSE}/(n-1)$. An orthonormal change of coordinates in the [Gaussian vector](../../../../../gaussian-random-vector.md) $Y$ separates the unit design direction $x/\sqrt{S_{xx}}$ from its $n-1$ orthogonal residual directions. The first coordinate is normal with mean $\beta\sqrt{S_{xx}}$ and variance $\sigma^2$; the remaining coordinates are independent centered normals with that variance. Consequently

$$
\frac{(\widehat\beta-\beta)\sqrt{S_{xx}}}{\sigma}\sim N(0,1),
\qquad\frac{\mathrm{SSE}}{\sigma^2}\sim\chi^2_{n-1},
$$

and these variables are independent. Thus under the null, the [Student t test for regression through the origin](../../../../../student-t-test-for-regression-through-the-origin.md) statistic is

$$
\boxed{T=\frac{\widehat\beta\sqrt{S_{xx}}}{s}\sim t_{n-1}.}
$$

For a prescribed significance level $\eta$, reject the two-sided null when $|T|>t_{n-1,1-\eta/2}$. The two-sided p-value is $2[1-F_{t_{n-1}}(|T|)]$. There is one fitted coefficient, so the variance degrees of freedom are $n-1$, not $n-2$.

The assumptions $S_{xx}>0$ and $n\geq2$ matter. If all $x_i=0$, the distribution contains no information about $\beta$ and no informative test is possible. With one nonzero design observation there is no residual variance degree of freedom, so the stated unknown-variance t test cannot be constructed.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
