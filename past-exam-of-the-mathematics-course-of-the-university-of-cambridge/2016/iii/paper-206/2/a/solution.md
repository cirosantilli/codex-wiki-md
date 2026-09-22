<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gaussian likelihood](../../../../../../gaussian-likelihood.md) has [log-likelihood](../../../../../../log-likelihood.md), apart from no omitted parameter-dependent terms,

$$
\ell(\beta,\sigma^2)
=-\frac n2\log(2\pi)-\frac n2\log\sigma^2
-\frac{1}{2\sigma^2}(Y-X\beta)^T(Y-X\beta).
$$

For fixed $\sigma^2$, maximizing it is [ordinary least squares](../../../../../../ordinary-least-squares.md). Differentiating with respect to $\beta$ gives the [normal equation](../../../../../../normal-equation.md) $X^TX\widehat\beta=X^TY$. [Full column rank](../../../../../../full-column-rank.md) makes the quadratic strictly convex, so

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

At this value, differentiating with respect to $v=\sigma^2$ gives $-n/(2v)+\mathrm{RSS}/(2v^2)=0$, so

$$
\boxed{\widehat\sigma^2_{\mathrm{ML}}=\frac{\|Y-X\widehat\beta\|^2}{n}.}
$$

For positive RSS this is the global likelihood maximum in $v>0$. RSS is positive almost surely under the model since $p<n$; an exactly zero observed RSS instead gives a boundary supremum as $v\downarrow0$.

As a [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md), the coefficient estimate satisfies

$$
\boxed{\widehat\beta\sim N_p\!\left(\beta,\sigma^2(X^TX)^{-1}\right).}
$$

Indeed, $\widehat\beta-\beta=(X^TX)^{-1}X^T\varepsilon$, and direct matrix multiplication gives its [covariance matrix](../../../../../../covariance-matrix.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
