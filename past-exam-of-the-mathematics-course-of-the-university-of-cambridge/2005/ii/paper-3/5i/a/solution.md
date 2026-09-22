<h1 id="5i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [least-squares estimator](../../../../../../ordinary-least-squares-estimators.md) minimizes $\|Y-Xb\|^2$. Differentiating in $b$ gives $-2X^T(Y-Xb)=0$, hence $\boxed{X^TX\widehat\beta=X^TY}$. Full column rank makes $X^TX$ positive definite, so

$$
\widehat\beta=(X^TX)^{-1}X^TY=\beta+(X^TX)^{-1}X^T\epsilon.
$$

This is a [linear transformation](../../../../../../linear-map.md) of a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md). Its mean is $\beta$ and its [covariance](../../../../../../covariance.md) is $\sigma^2(X^TX)^{-1}$. Therefore $\boxed{\widehat\beta\sim N_p(\beta,\sigma^2(X^TX)^{-1})}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5I](../../5i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
